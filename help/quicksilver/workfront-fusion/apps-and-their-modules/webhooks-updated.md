---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Webhook是由事件触发的HTTP调用。 您可以使用Web挂接来激活即时触发器模块。 任何连接到Internet并允许HTTP请求的应用程序都可以将Webhook发送到Adobe Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1391'
ht-degree: 0%

---

# Webhooks

Webhook是由事件触发的HTTP调用。 您可以使用Web挂接来激活即时触发器模块。 任何连接到Internet并允许HTTP请求的应用程序都可以将Webhook发送到Adobe Workfront Fusion。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr>
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

&#42;&#42;有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 在中使用网页挂接 [!DNL Workfront Fusion]

>[!NOTE]
>
>要调用第三方Webhook（传出Webhook），请使用其中一个HTTP模块。 有关更多信息，请参阅 [HTTP模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

使用Webhook将应用程序连接到 [!DNL Workfront Fusion]:

1. 添加 **[!UICONTROL Webhooks]** >**[!UICONTROL 自定义Webhook]** 即时触发模块。

1. 单击 **[!UICONTROL 添加]** 在Webhook字段旁边，输入新Webhook的名称。
1. （可选）单击 **[!UICONTROL 高级设置]**.
1. 在 **[!UICONTROL IP限制]** 字段中，输入模块可从中接受数据的IP地址列表（以逗号分隔）。
1. 单击 **[!UICONTROL 保存]**

创建Webhook后，会显示一个唯一的URL。 这是Webhook发送数据的地址。 Workfront Fusion将验证发送到此地址的数据，然后将其传递到该地址，以便在情景中进行处理。

>[!NOTE]
>
>创建Webhook后，您可以一次在多个方案中使用它。

### 配置Webhook的数据结构 {#configure-the-webhook-s-data-structure}

为了识别传入有效载荷的数据结构， [!DNL Workfront Fusion] 解析您发送到显示地址的示例数据。 您可以通过在服务或应用程序中进行更改以使该服务或应用程序调用Webhook来提供示例数据。 例如，您可以删除文件。

或者，您也可以按照以下步骤通过 [!UICONTROL HTTP] > [!UICONTROL 请求] 模块。

1. 使用 **[!UICONTROL HTTP]** > **[!UICONTROL 请求]** 模块

1. 使用以下值配置模块：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>输入Webhook的URL。 您可以在[!UICONTROL Webhooks]模块中找到此URL，您以前使用它来设置Webhook。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL方法] </td> 
      <td><p>[!UICONTROLPOST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL内容类型]</td> 
      <td><p> JSON(application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL请求内容]</td> 
      <td><p>Webhook中应为原始JSON</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. 使用 [!UICONTROL Webhooks] 模块。
1. 在Web挂接模块中，单击 **[!UICONTROL 重新确定数据结构]**.

   您无需从Web挂接模块中取消其他模块的链接。

1. 使用 [!UICONTROL HTTP] 模块并运行它。
1. 使用Webhooks模块切换回方案。

   A &quot;[!UICONTROL 已成功确定]“消息表示模块已成功确定数据结构。

   ![](assets/successfully-determined-350x175.png)

1. 单击 **[!UICONTROL 确定]** 以保存数据结构。

   现在，Webhook的项目可在映射面板中用于方案中的后续模块。

## 队列

如果Webhook收到数据，并且没有预期该数据的活动方案，则数据将存储在队列中。 激活方案后，它会按顺序处理队列中等待的所有包。

>[!IMPORTANT]
>
>Webhook队列在采用相同Webhook的场景之间共享。 如果其中一个方案处于禁用状态，则所有传入数据都将保留在队列中。

## 支持的传入数据格式

[!DNL Workfront Fusion] 支持3种传入数据格式： [!UICONTROL 查询字符串], [!UICONTROL 表单数据] 和 [!UICONTROL JSON].

[!DNL Workfront Fusion] 根据选定的数据结构验证所有传入数据。 然后，根据方案的设置，数据将存储在待处理的队列中，或立即进行处理。

如果数据的任何部分未通过验证， [!DNL Workfront Fusion] 返回400 HTTP状态代码，并在HTTP响应正文中指定传入数据失败验证检查的原因。 如果传入数据的验证成功，则Workfront Fusion会返回“[!UICONTROL 200已接受]“ ”状态。

* [[!UICONTROL 查询字符串]](#query-string)
* [[!UICONTROL 表单数据]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL 查询字符串]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL 表单数据]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### 多部分表单数据

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

为了接收使用 `multipart/form-data`，则必须使用 `collection` 包含嵌套字段的类型字段 `name`, `mime`和 `data`. 字段 `name` 是 `text` 类型并包含已上传文件的名称。 的 `mime` 是 `text` 类型并包含MIME格式的文件。 字段 `data` 是 `buffer` 类型并包含所传输文件的二进制数据。

有关MIME格式的更多信息，请参阅 [MIME模块](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>如果要访问原始JSON，请在设置Webhook时启用JSON传递。
>
>1. 单击 **[!UICONTROL 添加]** 添加新网页挂钩。
>1. 单击 **[!UICONTROL 显示高级设置]**.
>1. 单击 **[!UICONTROL JSON传递]**.

>


## Webhook头

要访问Webhook的标头，请在设置Webhook时启用获取请求标头。

1. 单击 **[!UICONTROL 添加]** 添加新网页挂钩。
1. 单击 **[!UICONTROL 显示高级设置]**.
1. 单击 **[!UICONTROL 获取请求标头]**.

您可以通过 `map()` 和 `get()` 函数。

>[!INFO]
>
>**示例:**
>
>以下示例显示了一个公式，该公式会提取 `authorization` 标题 `Headers[]` 数组。 该公式用在过滤器中，该过滤器将提取的值与给定文本进行比较，以便仅在存在匹配项时才传递网页挂钩。
>
>![](assets/set-up-a-filter-350x169.png)
>
>有关使用给定键获取数组元素的更多信息，请参阅 [使用给定键映射数组的元素](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) 在文章中 [在Adobe Workfront Fusion中，将信息从一个模块映射到另一个模块](../../workfront-fusion/mapping/map-information-between-modules.md).

## 响应Web挂接

对Webhook调用的默认响应为文本“已接受”。 在执行自定义Webhook模块期间，响应会返回到调用Webhook的应用程序。

* [测试对网页挂钩的响应](#test-the-response-to-a-webhook)
* [HTML响应示例](#html-response-example)
* [重定向示例](#redirect-example)

### 测试对网页挂钩的响应

1. 包括 **[!UICONTROL 自定义Webhook]** 模块。
1. 向模块中添加新网页挂接。
1. 将Webhook URL复制到剪贴板。
1. 运行方案。

   在 [!UICONTROL 自定义Webhook] 模块更改为旋转点。 这表示模块现在正在等待Webhook调用。

1. 打开新的浏览器窗口，将复制的URL粘贴到地址栏中，然后按 **[!UICONTROL 输入]**.

   的 [!UICONTROL 自定义Webhook] 模块触发，浏览器将显示一个新页面。

如果要自定义Webhook的响应，请使用模块“Webhook响应”。

模块的配置包含两个字段： [!UICONTROL 状态] 和 [!UICONTROL 正文].

* 的 [!UICONTROL 状态] 字段包含HTTP响应状态代码，如“成功”的2xx(例如， `200` 对于“确定”，为3xx表示重定向(例如， `307` 对于临时重定向)，对于客户端错误，为4xx(例如， `400` 请求错误)等。

* 的 [!UICONTROL 正文] 字段中包含将被webhook调用接受的任何内容。 它可以是简单的文本、HTML、XML、JSON等。

   >[!TIP]
   >
   >我们建议将 `Content-Type` 标头到相应的MIME类型： `text/plain` 对于纯文本， `text/html` 对于HTML, `application/json` 对于JSON、 `application/xml` for XML，等等。 有关MIME类型的更多信息，请参阅 [MIME模块](../../workfront-fusion/apps-and-their-modules/mime.md).

发送响应的超时为40秒。 如果响应在该时间段内不可用，则Workfront Fusion会返回“200已接受”状态。

### HTML响应示例

>[!INFO]
>
>**示例:**
>
>配置 [!UICONTROL Webhook响应] 模块如下：
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL状态] </td> 
&gt;   <td> <p>2xx成功HTTP状态代码，例如200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL主体] </td> 
&gt;   <td> <p>HTML代码</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL自定义标题]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>键</strong>:内容类型</li> 
&gt;     <li><strong>值</strong>:text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>这将产生一个HTML响应，该响应显示在Web浏览器中：
>
>![](assets/html-response-350x70.png)

### 重定向示例

>[!INFO]
>
>**示例：** 配置 [!UICONTROL Webhook响应] 模块如下：
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL状态] </td> 
&gt;   <td> <p>3xx重定向HTTP状态代码，例如303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL自定义标题]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL密钥]</strong>:位置</li> 
&gt;     <li><strong>[!UICONTROL值]</strong>:要重定向到的URL。</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook停用

如果出现以下任一情况，将自动停用Web挂接：

* 网页挂接已超过5天未连接到任何方案
* Webhook仅用于不活动情景（已处于非活动状态超过30天）。

如果已停用的Web挂接未连接到任何方案并且处于停用状态超过30天，则会自动删除和取消注册这些挂接。


## 疑难解答

### 映射面板中缺少项

如果映射面板中缺少某些项目，则在 [!UICONTROL Webhooks] > [!UICONTROL 自定义Webhook] 模块，单击 **[!UICONTROL Webhooks] > [!UICONTROL 自定义Webhook]** 打开其设置并单击 **[!UICONTROL 重新确定数据结构]**:

![](assets/redetermine-data-structure-btn-350x195.png)

然后，按照部分中描述的步骤操作 [配置Webhook的数据结构](#configure-the-webhook-s-data-structure) 在本文中。
