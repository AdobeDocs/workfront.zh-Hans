---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: 过滤事件订阅消息
description: 过滤事件订阅消息
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# 过滤事件订阅消息

您可以构建中介处理组件，以帮助您仅过滤和处理业务所需的事件订阅消息。

要了解事件订阅，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md).

## 过滤事件消息

此部分包含过滤的代码片段，您可以实施这些代码片段来减少事件订阅消息的负载。  为了帮助显示不同语言语法中的差异，这些代码片段说明了以下语言编写的同一组过滤器：

您可以在以下位置查看筛选示例 [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)，您可以从中查看每种语言的语法以及与AWS SDK交互的方式之间的差异。这些示例编写为AWS Lambdas，这是采用中间筛选和处理组件的常用方法。

以下代码片段近乎于部署就绪，可用作帮助您编写自己的更复杂的过滤器以及处理组件的起点。

### Java

以下Java示例显示了如何根据项目的组ID筛选项目负载，如中所示 [ProjectGroupFiltering.java：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. 建立您要查找的组ID，并将其创建为一个静态常量。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   在此示例中，handleRequest方法(一个AWS Lambda标准方法名称)将Map类型作为第一个参数（即事件订阅消息内容）。\
   它采用的第二个参数是当前Lambda代理请求的上下文。\
   Context对象用于获取Lambda记录器，该记录器用于将消息写入CloudWatchLogs。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. 调用handleRequest方法时，获取事件订阅消息的“newState”属性，该属性表示资源的更新状态。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   要了解newState格式，请参阅 [事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

3. 在从消息中解析“newState”映射后，请确保对象的组ID与您在第1步中标识的组ID匹配。

4. （视情况而定）如果ID **不要** 匹配，删除消息以返回空响应。

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
   >返回空的成功响应至关重要。 除200级响应之外的任何响应均被视为投放失败。

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

   AWS SDK用于调用另一个Lambda，后者负责将过滤的消息传递到我们的所需端点。

   将消息投放给另一个Lambda的责任推掉是为了避免来自事件订阅服务的投放请求超时。 目前，允许的投放超时设置为5秒。 如果过滤器处理时间超过设置所允许的时间，则可以处理请求，但事件订阅服务将超时并进入重试循环，直到在超时时段内收到200级响应。

   要了解有关管理消息投放的更多信息，请参阅 [改进报文传送，同时适应超时](#improving-message-delivery-while-accommodating-timeouts).

### Python

Java示例和Python示例之间的主要区别在于，在Java示例中，接收事件订阅消息作为第一个参数，而在Python示例中，第一个参数是Lambda代理“事件”，其中包含事件订阅消息以及有关AWS Lambda代理请求的信息。

以下Python示例显示了如何根据项目的组ID筛选项目负载，如中所示  [projectGroupFiltering.py：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. 建立您要查找的组ID，并将其创建为一个静态常量。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   第一个参数是Lambda代理“事件”，其中包含事件订阅消息和一些需要解析的其他信息。\
   第二个参数是当前Lambda代理请求的上下文。\
   在此示例中，Context对象用于获取Lambda记录器，该记录器用于将消息写入CloudWatchLogs。

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. 解析来自事件的消息。

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. 获取事件订阅消息的“newState”属性。\
   newState属性表示资源的更新状态。

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   要了解newState格式，请参阅 [事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

1. 在从消息中解析“newState”映射后，请确保对象的组ID与您在第1步中标识的组ID匹配。

1. （视情况而定）如果ID不匹配，请删除消息以返回空响应。

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
   >返回空的成功响应至关重要。 除200级响应之外的任何响应均被视为投放失败。

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

   AWS SDK用于调用另一个Lambda，后者负责将过滤的消息传递到我们的所需端点。

   将消息投放给另一个Lambda的责任推掉是为了避免来自事件订阅服务的投放请求超时。 目前，投放超时设置为5秒。 如果过滤器处理时间超过设置所允许的时间，则可以处理请求，但事件订阅服务将超时并进入重试循环，直到在超时时段内收到200级响应。


### Node.js

项目组ID筛选的Node.js示例与Java和Python示例类似。 与Python示例一样，第一个参数是Lambda代理事件，第二个参数是Lambda Context。

Node.js中的以下示例显示如何根据项目的组ID筛选项目负载，如中所示  [projectGroupFiltering.js：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. 建立您要查找的组ID，并将其创建为一个静态常量。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   第一个参数是Lambda代理“事件”，其中包含事件订阅消息和一些需要解析的其他信息。\
   第二个参数是当前Lambda代理请求的上下文。\
   在此示例中，Context对象用于获取Lambda记录器，该记录器用于将消息写入CloudWatchLogs。

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. 解析来自事件的消息。

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. 从事件订阅消息的“newState”属性中获取projectGroupID，然后将其与您在第1步中标识的组的组ID进行匹配。

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   要了解newState格式，请参阅 [事件订阅的出站消息格式](../../wf-api/api/message-format-event-subs.md).

4. （视情况而定）如果ID不匹配，请删除消息以返回空响应。\
   以下示例显示了匹配的组ID：

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
   >返回空的成功响应至关重要。 除200级响应之外的任何响应均被视为投放失败。

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

   AWS SDK用于调用另一个Lambda，后者负责将过滤的消息传递到我们的所需端点。\
   将消息投放给另一个Lambda的责任推掉是为了避免来自事件订阅服务的投放请求超时。 目前，投放超时设置为5秒。 如果过滤器处理时间超过设置所允许的时间，则可以处理请求，但事件订阅服务将超时并进入重试循环，直到在超时时段内收到200级响应。\
   要了解如何管理消息投放，请参阅 [改进报文传送，同时适应超时](#improving-message-delivery-while-accommodating-timeouts).

## 改进报文传送，同时适应超时

事件订阅服务的严格超时为 **5秒** 用于所有投放请求。 如果消息的投放超过允许的时间，事件订阅服务将开始该消息的重试周期。

例如，您构建的项目组ID过滤器类似于中的示例之一 [过滤事件消息](#filtering-event-messages) 并包括数据库查找以确定是否需要该消息。 数据库查找以及所需的处理和Lambda冷启动所需的时间可能超过五秒，从而导致事件订阅服务重试传递消息。

您可以将流程中耗时的部分与负责确定消息是否是要处理和投放的逻辑分开，以避免重试。 这样，您就可以接受消息并向事件订阅服务发送200级响应，同时异步继续在后台处理或过滤消息（请参阅中的步骤5） [Java](#java) 例如)。


即使您的处理或筛选未超过五秒超时，将消息筛选或处理的第一个接触点与客户端上的其他处理或投放步骤分离出来仍然有好处。 这样，将消息从事件订阅服务切换到目标将对双方的时间和性能影响最小。

要了解有关重试机制的更多信息，请参阅 [事件订阅重试](../../wf-api/api/event-sub-retries.md).

## 在无云架构中实施托管过滤器

如果您无法利用云架构进行事件订阅过滤，则仍可以使用中的示例 [过滤事件消息](#filtering-event-messages) 作为有关如何实施您自己的托管过滤器或处理组件的路线图。

### 调整独立服务的过滤示例

在无云环境中使用过滤示例之前，请执行以下操作：

* 省略示例中特定于Lambda的部分，例如Context参数。

* 更改示例中其他Lambda的调用，以便向其他过滤器发出额外的异步HTTP请求或处理您托管的组件。

* 如果引用Python和Node.js示例，请将第一个事件参数替换为Java示例中显示的第一个有效负载参数。 请参阅中的步骤1 [Java](#java).

* 使用基于Web的API部署过滤器或处理器。

### 防止错过事件订阅消息

有时，在无云体系结构中，负责接收事件订阅消息的服务可能无法访问。 在这种情况下，消息可能会超过重试限制并丢失，无法检索消息中的信息。

我们建议您在启动服务时，实施一个查询，查询可能包含在未接留言中的所有资源的最新状态。 如以下示例所示，您可以使用筛选条件查询符合该条件的资源，然后处理其当前状态。

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

中的所有示例 [过滤事件消息](#filtering-event-messages) 部分将过滤的邮件传递到另一个AWS Lambda。 这样做是为了避免超过投放请求中的五秒超时，该超时由发出请求的事件订阅服务强制执行。

在无云架构中，您可能需要实施异步处理机制，该机制与AWS SDK允许对其他AWS Lambda进行异步调用的方式类似。 大多数现代编程语言都有处理异步处理的第三方或核心库，从而允许您利用在我们的示例中实现的异步样式处理。
