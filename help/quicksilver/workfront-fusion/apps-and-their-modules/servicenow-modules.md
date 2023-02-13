---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: ServiceNow模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL ServiceNow]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# [!DNL ServiceNow] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL ServiceNow]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL ServiceNow] 模块，您必须 [!DNL ServiceNow] 帐户。

## 连接 [!DNL ServiceNow] to [!DNL Workfront Fusion]

为 [!DNL ServiceNow] 模块：

1. 单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 框中，选择要在首次 [!DNL ServiceNow] 模块。
1. 输入以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL连接名称]</p> </td> 
      <td>输入新 [!DNL ServiceNow] 连接</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL用户名]</p> </td> 
      <td>输入 [!DNL ServiceNow] 用户名。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL密码]</p> </td> 
      <td>输入ServiceNow密码。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL实例]</p> </td> 
      <td> <p>输入的地址 [!DNL ServiceNow] 无帐户 <code>https://</code> (通常 <code>&lt;company>.service-now.com</code>)。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] 模块及其字段

配置 [!DNL ServiceNow] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL ServiceNow] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>如果在“[!UICONTROL 记录类型]“ ”字段，则加载自定义字段可能需要一些时间。
>
>如果没有自定义记录，则下拉列表将为空。

* [[!UICONTROL 监视记录]](#watch-records)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 停用用户]](#deactivate-a-user)
* [[!UICONTROL 下载附件]](#download-an-attachment)
* [[!UICONTROL 上传附件]](#upload-an-attachment)
* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 搜索记录]](#search-for-records)

### [!UICONTROL 监视记录]

创建或更新记录时，此触发器模块会激活方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表类型]</td> 
   <td>选择要监视的表是自定义表还是标准表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要观看的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>选择要显示的值类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择希望模块输出的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td>选择您是要观看新记录还是更新记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL ServiceNow] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL ServiceNow] 模块。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL相对URL]</td> 
   <td> <p>在Web服务器上键入您希望模块与之交互的地址。</p> <p>您可以键入一个相对URL，这意味着您不必包含协议(例如 <code>http://</code>)。 这向Web服务器建议，交互正在服务器上发生。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 读取记录]

此操作模块读取 [!DNL ServiceNow] 使用系统ID进行记录。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录系统ID]</td> 
   <td>输入或映射唯一 [!DNL ServiceNow] 您希望模块读取的记录的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表类型]</td> 
   <td>选择要读取的记录是在自定义表还是标准表中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择 [!DNL ServiceNow] 记录您希望模块读取的内容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>选择要显示的值类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择希望模块输出的字段。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 停用用户]

此操作模块可停用 [!DNL ServiceNow] 使用系统ID。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用户系统ID]</td> 
   <td> 输入或映射唯一 [!DNL ServiceNow] 您希望模块停用的用户ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 下载附件]

此操作模块将下载 [!DNL ServiceNow] 记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附件系统ID]</td> 
   <td> 输入或映射唯一 [!DNL ServiceNow] 要下载模块的附件的ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上传附件]

此操作模块将附件上传到 [!DNL ServiceNow] 记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表名称]</td> 
   <td>输入或映射要上载附件的表的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系统ID]</td> 
   <td>输入或映射唯一 [!DNL ServiceNow] 要上载附件的系统ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td>输入或映射附件的名称</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件内容]</td> 
   <td>输入或映射要上传到的文件 [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 创建记录]

此操作模块会创建一个 [!DNL ServiceNow] 记录。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表类型]</td> 
   <td>选择是要在自定义表或标准表中创建记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择 [!DNL ServiceNow] 记录您希望模块创建的内容。 然后，您可以填写此记录类型的可用字段。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新记录]

此操作模块会创建一个 [!DNL ServiceNow] 记录。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录系统ID]</td> 
   <td>输入或映射唯一 [!DNL ServiceNow] 要更新模块的记录的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表类型]</td> 
   <td>选择要更新的记录是在自定义表还是标准表中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择 [!DNL ServiceNow] 记录您希望模块更新。 然后，您可以填写此记录类型的可用字段。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除记录]

此操作模块会删除事件或用户。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择是要删除事件还是用户。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系统ID]</td> 
   <td>输入或映射唯一 [!DNL ServiceNow] 您希望模块删除的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索记录]

此模块会使用您选择的条件搜索记录。

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将ServiceNow帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">连接 [!DNL ServiceNow] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表类型]</td> 
   <td>选择要搜索的表是自定义表还是标准表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要搜索的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL结果集]</td> 
   <td>选择是希望模块返回与标准匹配的所有记录，还是仅返回与标准匹配的第一个记录。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录的最大计数]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索类型]</td> 
   <td> <p>选择您希望模块执行的搜索类型</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL高级查询]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL搜索查询]</p> <p>输入自定义搜索查询。 有关 [!DNL ServiceNow] 自定义搜索查询，请参阅 <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow查询文档</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL搜索条件]</p> <p>输入您希望模块搜索的标准。 有关设置搜索过滤器的更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中为方案添加过滤器</a>.</p> </li> 
       <li> <p>[!UICONTROL排序依据]</p> <p>指示您希望模块按哪个字段对结果进行排序，以及应按升序还是降序排序。</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>选择要显示的值类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td>选择希望模块输出的字段。</td> 
  </tr> 
 </tbody> 
</table>
