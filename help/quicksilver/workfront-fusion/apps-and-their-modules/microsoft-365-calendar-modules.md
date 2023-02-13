---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365日历
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Microsoft Office 365日历的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Microsoft Office 365 Calendar]，并将其连接到多个第三方应用程序和服务。

为了使用 [!DNL Office 365 Calendar] with [!DNL Adobe Workfront Fusion]，则需要具有 [!DNL Office 365 Excel] 帐户。 您可以在 [www.office.com](http://www.office.com/).

有关将Office 365帐户连接到 [!DNL Workfront Fusion]，请参阅 [创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

在您同意后，系统会将您重定向回 [!UICONTROL Workfront Fusion] 管理页面，您可以在该页面中继续创建方案。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Microsoft Office 365 Calendar] 模块，您必须 [!DNL Microsoft Office 365 Calendar] 帐户。

## [!DNL Microsoft Office 365 Calendar] 模块及其字段

配置 [!DNL Microsoft Office 365 Calendar] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Microsoft Office 365 Calendar] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Event](#event)
* [日历](#calendar)
* [其他](#other)

### Event

* [[!UICONTROL 观看事件]](#watch-events)
* [[!UICONTROL 搜索事件]](#search-events)
* [[!UICONTROL 获取事件]](#get-an-event)
* [[!UICONTROL 创建事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 删除事件]](#delete-an-event)

#### [!UICONTROL 观看事件]

当在选定的日历中创建、更新、删除、启动或结束事件时，此触发器模块会检索该事件的详细信息。

>[!NOTE]
>
>要监视某个事件系列的已删除发生次数，请选择 [!UICONTROL 按更新时间] 在 [!UICONTROL 观看事件] 字段。 此模块不会监视已删除的单个事件或已删除的事件系列。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch事件]</td> 
   <td> <p>选择您希望如何观看事件。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By Created Time]</strong> </p> <p>请留意新事件。</p> </li> 
     <li> <p><strong>[!UICONTROL By Updated Time]</strong> </p> <p>关注更新的事件。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历组ID]</td> 
   <td>选择[!UICONTROL日历组]，其中包含要在其中观看事件的日历。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历]</td> 
   <td> <p>选择要观看的特定日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td>设置筛选条件以按主题、事件ID或正文筛选结果。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入消息的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索事件]

此搜索模块会检索在选定日历中创建、更新、删除、启动或结束事件时该事件的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历组ID]</td> 
   <td>选择[!UICONTROL日历组]，其中包含要在其中观看事件的日历。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历]</td> 
   <td> <p>选择要观看的特定日历。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td> <p>设置筛选条件以筛选结果。 您可以按以下属性进行过滤：</p> 
    <ul> 
     <li>[!UICONTROL主题]</li> 
     <li>[!UICONTROL事件ID]</li> 
     <li>[!UICONTROL创建日期时间]</li> 
     <li>[!UICONTROL上次修改日期时间]</li> 
     <li>[!UICONTROL主体预览]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>选择结果的排序方式。</p> 
    <ul> 
     <li><strong>[!UICONTROL主题]</strong>、升序或降序</li> 
     <li><strong>[!UICONTROL创建日期时间]</strong>、升序或降序</li> 
     <li><strong>[!UICONTROL上次修改日期时间]</strong>、升序或降序</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入最大事件数 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取事件]

此操作模块可检索指定事件的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>输入或映射要检索相关详细信息的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建事件]

此操作模块会创建新事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题]</td> 
   <td> <p>输入或映射创建事件的标题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL开始日期]</td> 
   <td> 以合并的日期和时间表示形式输入事件开始的单个时间点。 使用格式 <code>({date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结束日期]</td> 
   <td> 输入事件以合并的日期和时间表示形式结束的单个时间点。 使用格式 <code>{date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒开]</td> 
   <td>选择是否要激活此事件的提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒]</td> 
   <td>输入或映射应触发提醒的事件开始前的分钟数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>选择此事件的重要性。</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>选择此事件的敏感性。</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Personal]”消息。</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Private]”消息。 此事件不会由收件人的收件箱规则转发或重定向。</p> </li> 
     <li> <p><strong>[!UICONTROL机密]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Confidential]”消息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>选择正文内容是纯文本还是HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体内容]</td> 
   <td>输入或映射与事件关联的消息正文。 它可以是HTML格式或文本格式（如上面[!UICONTROL Body Content Type]字段中指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置]</td> 
   <td> <p>输入事件位置详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！请求的UICONTROL响应]</td> 
   <td>选择 <strong>[!UICONTROL Yes]</strong> 请求被邀请者发送对事件邀请的响应。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示为]</td> 
   <td> <p>选择您希望事件向查看日历的人员显示的方式。</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL暂定]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL已停职]</li> 
     <li>[!UICONTROL在其他位置工作]</li> 
     <li>[!UICONTROL未知]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL与会者]</p> </td> 
   <td> <p>添加活动的与会者。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入与会者的姓名。</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件]</strong> </p> <p>输入与会者的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL类别]</td> 
   <td>输入或映射希望事件在日历中显示为的类别。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此操作模块会更新现有事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td>输入、映射或选择要更新的事件的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题]</td> 
   <td> <p>输入或映射创建事件的标题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL开始日期]</td> 
   <td> 以合并的日期和时间表示形式输入事件开始的单个时间点。 使用格式 <code>{date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结束日期]</td> 
   <td> 输入事件以合并的日期和时间表示形式结束的单个时间点。 使用格式 <code>({date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒开]</td> 
   <td>选择是否要激活此事件的提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒]</td> 
   <td>输入或映射应触发提醒的事件开始前的分钟数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>选择此事件的重要性。</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>选择此事件的敏感性。</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Personal]”消息。</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Private]”消息。 此事件不会由收件人的收件箱规则转发或重定向。</p> </li> 
     <li> <p><strong>[!UICONTROL机密]</strong> </p> <p>收件人看到“[!UICONTROL Please this as Confidential]”消息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>选择与事件关联的消息正文内容是纯文本还是HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体内容]</td> 
   <td>输入或映射与事件关联的消息正文。 它可以是HTML格式或文本格式（如上面[!UICONTROL Body Content Type]字段中指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置]</td> 
   <td> <p>输入事件位置详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！请求的UICONTROL响应]</td> 
   <td>选择 <strong>[!UICONTROL Yes]</strong> 请求被邀请者发送对事件邀请的响应。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示为]</td> 
   <td> <p>选择您希望事件向查看日历的人员显示的方式。</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL暂定]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL已停职]</li> 
     <li>[!UICONTROL在其他位置工作]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL与会者]</p> </td> 
   <td> <p>添加活动的与会者。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入与会者的姓名。</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件]</strong> </p> <p>输入与会者的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL类别]</td> 
   <td>输入或映射希望事件在日历中显示为的类别。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除事件]

此操作模块会删除现有事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>输入或映射要删除的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 日历

* [[!UICONTROL 列出日历]](#list-calendars)
* [[!UICONTROL 获取日历]](#get-a-calendar)
* [[!UICONTROL 创建日历]](#create-a-calendar)
* [[!UICONTROL 更新日历]](#update-a-calendar)
* [[!UICONTROL 删除日历]](#delete-a-calendar)

#### [!UICONTROL 列出日历]

此搜索模块可检索经过身份验证的用户所有日历的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历组ID]</td> 
   <td>选择包含要列出的日历的[!UICONTROL日历组]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入最大日历数 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取日历]

此操作模块检索有关单个日历的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td> <p>输入或映射要检索相关详细信息的日历ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建日历]

此操作模块会在您的Google帐户中创建新日历。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历名称]</td> 
   <td> <p>输入新日历的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新日历]

此操作模块编辑现有日历。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td>输入要更新的日历的[!UICONTROL日历ID]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新日历名称]</td> 
   <td> <p>输入新日历的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除日历]

此操作模块会删除现有日历。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日历ID]</td> 
   <td>输入要删除的日历的[!UICONTROL Calendar] ID。</td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于 <code>https://graph.microsoft.com</code>. 示例:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:   <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
