---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: 过滤事件订阅消息
description: 过滤事件订阅消息
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# 过滤事件订阅消息

您可以构建中介处理组件，这些组件可以帮助您过滤和处理业务所需的事件订阅消息。

要了解事件订阅，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md).

## 过滤事件消息

此部分包含过滤的代码片段，您可以实施这些代码片段来减少事件订阅消息的负载。  为了帮助显示各种语言语法的差异，这些片段说明了用下列语言编写的相同过滤器集：

您可以在 [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)，您可以从中查看每种语言的语法差异以及与AWS SDK的交互方式。这些示例以AWS Lambdas编写，这是使用中间过滤和处理组件的常用方法。

以下代码片段在部署就绪后即可使用，可用作帮助您编写更复杂的过滤器和处理组件的起点。

### Java

Java中的以下示例显示了如何根据项目的组ID筛选项目负载，如 [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. 建立要查找的组ID，并将其创建为静态常量。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   在此示例中，handleRequest方法(一种AWS Lambda标准方法名称)采用Map类型作为其第一个参数，即事件订阅消息内容。\
   它采用的第二个参数是当前Lambda代理请求的上下文。\
   上下文对象用于获取Lambda记录器，该记录器用于向CloudWatchLogs写入消息。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. 在调用handleRequest方法时，获取事件订阅消息的“newState”属性，该属性表示资源的更新状态。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   要了解newState格式，请参阅 [用于事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

3. 从消息中解析“newState”映射后，确保对象的组ID与您在步骤1中标识的组ID匹配。

4. （视情况而定）如果ID **不** 匹配，请删除消息以返回空响应。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >返回空的成功响应至关重要。 除200级响应之外的任何其他内容都被视为失败的投放。

5. 处理消息。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK用于调用另一个Lambda，Lambda负责将过滤的消息传送到我们所需的端点。

   传递消息给另一个Lambda的责任的目的是避免来自事件订阅服务的投放请求超时。 当前，允许的交付超时设置为5秒。 如果过滤器所花费的时间超过设置所允许的时间，您可以处理请求，但事件订阅服务将超时并陷入重试循环，直到它在超时时间段内收到200级响应为止。

   要了解有关管理消息投放的更多信息，请参阅 [在适应超时的同时改进消息投放](#improving-message-delivery-while-accommodating-timeouts).

### Python

Java和Python示例的主要区别在于，在Java示例中，事件订阅消息作为第一个参数接收，在Python示例中，第一个参数是Lambda代理“event”，其中包含事件订阅消息以及有关AWS Lambda代理请求的信息。

Python中的以下示例显示如何根据项目的组ID筛选项目负载，如  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. 建立要查找的组ID，并将其创建为静态常量。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   第一个参数是Lambda代理“event”，其中包含事件订阅消息和一些需要解析的其他信息。\
   第二个参数是当前Lambda代理请求的上下文。\
   在此示例中，上下文对象用于获取Lambda记录器，该记录器用于向CloudWatchLogs写入消息。

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. 解析事件中的消息。

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. 获取事件订阅消息的“newState”属性。\
   newState属性表示资源的更新状态。

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   要了解newState格式，请参阅 [用于事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

1. 从消息中解析“newState”映射后，确保对象的组ID与您在步骤1中标识的组ID匹配。

1. （视情况而定）如果ID不匹配，请删除消息，以返回空响应。

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >返回空的成功响应至关重要。 除200级响应之外的任何其他内容都被视为失败的投放。

1. 处理消息。

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK用于调用另一个Lambda，Lambda负责将过滤的消息传送到我们所需的端点。

   传递消息给另一个Lambda的责任的目的是避免来自事件订阅服务的投放请求超时。 当前，投放的超时设置为五秒。 如果过滤器所花费的时间超过设置所允许的时间，您可以处理请求，但事件订阅服务将超时并陷入重试循环，直到它在超时时间段内收到200级响应为止。


### Node.js

项目组ID筛选的Node.js示例读取的内容与Java和Python示例类似。 与Python示例一样，第一个参数是Lambda代理事件，第二个参数是Lambda上下文。

Node.js中的以下示例显示了如何根据项目的组ID筛选项目负载，如  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. 建立要查找的组ID，并将其创建为静态常量。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   第一个参数是Lambda代理“event”，其中包含事件订阅消息和一些需要解析的其他信息。\
   第二个参数是当前Lambda代理请求的上下文。\
   在此示例中，上下文对象用于获取Lambda记录器，该记录器用于向CloudWatchLogs写入消息。

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. 解析事件中的消息。

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. 从事件订阅消息的“newState”属性中获取projectGroupID，然后将其与您在步骤1中标识的组的组ID进行匹配。

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   要了解newState格式，请参阅 [用于事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

4. （视情况而定）如果ID不匹配，请删除消息，以返回空响应。\
   以下示例显示匹配的组ID:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >返回空的成功响应至关重要。 除200级响应之外的任何其他内容都被视为失败的投放。

5. 处理消息。

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK用于调用另一个Lambda，Lambda负责将过滤的消息传送到我们所需的端点。\
   传递消息给另一个Lambda的责任的目的是避免来自事件订阅服务的投放请求超时。 当前，投放的超时设置为五秒。 如果过滤器所花费的时间超过设置所允许的时间，您可以处理请求，但事件订阅服务将超时并陷入重试循环，直到它在超时时间段内收到200级响应为止。\
   要了解有关管理消息投放的信息，请参阅 [在适应超时的同时改进消息投放](#improving-message-delivery-while-accommodating-timeouts).

## 在适应超时的同时改进消息投放

事件订阅服务的严格超时为 **五秒** 所有投放请求。 如果消息投放超过允许的时间，事件订阅服务将开始该消息的重试周期。

例如，您会构建一个项目组ID过滤器，它类似于 [过滤事件消息](#filtering-event-messages) 并且您还包含数据库查找，以确定是否需要该消息。 数据库查找以及所需处理和Lambda冷启动所需的时间可能需要超过五秒钟，从而导致事件订阅服务重试投放消息。

您可以避免重试，方法是将流程中耗时的部分与负责确定是否是要处理和传递的消息的逻辑分开。 这样，您就可以接受消息并向事件订阅服务发送200级响应，同时异步继续在后台处理或过滤消息(请参阅 [Java](#java) 例如)。


即使您的处理或过滤未超过五秒超时，仍有利于将消息过滤或处理的首个接触点与客户端的其他处理或投放步骤分开。 这样，消息从事件订阅服务切换到目的地对双方的时间和性能影响最小。

要详细了解重试机制，请参阅 [事件订阅重试](../../wf-api/api/event-sub-retries.md).

## 在无云架构中实施托管过滤器

如果您无法利用云架构进行事件订阅过滤，则仍可以使用 [过滤事件消息](#filtering-event-messages) 作为如何实施您自己的托管过滤器或处理组件的路线图。

### 调整独立服务的过滤示例

在无云环境中使用过滤示例之前，请执行以下操作：

* 省略特定于Lambda的示例段，如Context参数。

* 更改示例中其他Lambda的调用，以便对您托管的其他过滤器或处理组件发出其他异步HTTP请求。

* 如果引用Python和Node.js示例，请将第一个事件参数替换为Java示例中显示的第一个有效负荷参数。 请参阅 [Java](#java).

* 使用基于Web的API部署过滤器或处理器。

### 防止遗漏的事件订阅消息

有时，在无云架构中，负责接收事件订阅消息的服务可能无法访问。 在这种情况下，消息可能会超出重试限制并丢失，无法检索消息中的信息。

我们建议您在服务启动期间实施一个查询，要求获取可能包含在未接消息中的所有资源的最新状态。 如以下示例所示，您可以使用筛选条件查询符合该条件的资源，然后处理其当前状态。

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

通过查询资源，您可以确保集成系统具有最新版本的资源。

### 在投放消息中实施异步处理

中的所有示例 [过滤事件消息](#filtering-event-messages) 部分传递将过滤消息传送到其他AWS Lambda的责任。 这样做是为了避免超过投放请求中的五秒超时，发出请求的事件订阅服务将强制执行该超时。

在无云架构中，您可能需要实施异步处理机制，这与AWS SDK允许对其他AWS Lambdas进行异步调用的方式类似。 大多数现代编程语言都具有可处理异步处理的第三方或核心库，允许您利用我们示例中实施的异步式处理。
