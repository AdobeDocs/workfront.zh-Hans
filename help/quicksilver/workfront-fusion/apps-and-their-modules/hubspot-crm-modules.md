---
title: HubSpot CRM模块
description: 的 [!DNL Adobe Workfront Fusion] HubSpot CRM模块让您能够监控事件、记录、联系人、参与、文件和表单提交，或者创建、检索、更新和删除记录、联系人、参与、事件或文件 [!DNL HubSpot CRM] 帐户。
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2485'
ht-degree: 0%

---

# [!DNL HubSpot CRM] 模块

的 [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] 通过模块，您可以监控事件、记录、联系人、参与、文件和表单提交，或者创建、检索、更新和删除记录、联系人、参与、事件或文件 [!DNL HubSpot CRM] 帐户。

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

使用 [!DNL HubSpot CRM] 模块，您必须 [!DNL HubSpot CRM] 帐户。

## 连接 [!DNL Adobe Workfront Fusion] to [!DNL HubSpot CRM]

有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] 模块及其字段

配置 [!DNL Hubspot CRM] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Hubspot CRM] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM对象](#crm-objects)
* [记录（交易、联系人和公司）](#records-deals-contacts-and-companies)
* [联系人](#contacts)
* [交易](#deals)
* [公司](#companies)
* [文件](#files)
* [票证](#tickets)
* [进行API调用](#make-an-api-call)

### CRM对象

#### [!UICONTROL 搜索CRM对象]

此搜索模块按自定义属性或按查询搜索CRM对象。 要搜索产品或行项目，请使用具有所需自定义范围的特殊连接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>输入或映射模块在一个执行周期中将返回的最大项目数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！要搜索的UICONTROL对象类型]</td> 
   <td>选择要搜索的Hubspot CRM对象的类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出属性]</td> 
   <td>选择要在模块输出中显示的属性。 可用字段取决于您选择的对象。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL筛选依据] </td> 
   <td> <p>选择要筛选搜索的方式</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL查询]</strong> </p> <p>输入或映射查询</p> </li> 
     <li> <p><strong>[!UICONTROL属性]</strong> </p> <p>输入搜索的组或过滤器。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依据]</td> 
   <td> <p>如果要对结果进行排序，请单击。 如果选择对结果排序，将显示以下字段。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL属性名称]</strong> </p> <p>选择要对结果排序的属性</p> </li> 
     <li> <p><strong>[!UICONTROL方向]</strong> </p> <p>选择要按升序还是降序方向对结果进行排序。</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### 记录（交易、联系人和公司）

* [[!UICONTROL 创建记录（旧版）]](#create-a-record-legacy)
* [[!UICONTROL 获取记录]](#get-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 获取记录资产]](#get-a-record-property)
* [[!UICONTROL 监视记录]](#watch-records)

#### [!UICONTROL 创建记录（旧版）]

此操作模块可创建联系人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL属性]</td> 
   <td>填写您要为记录设置的任何属性。 可用字段取决于要创建的记录类型。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取记录]

此操作模块可获取联系人、公司或交易的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>选择记录类型。</p> 
    <ul> 
     <li>[!UICONTROL联系人]</li> 
     <li>[!UICONTROL公司] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索类型]</td> 
   <td>如果您收到联系人，请选择是要按ID还是按电子邮件地址进行标识。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入要检索的联系人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子邮件]</td> 
   <td>输入要检索其详细信息的联系人的电子邮件地址。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块可更新联系人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要更新的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索类型]</td> 
   <td> <p>如果您有联系人，请选择要识别记录的方式：</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL电子邮件]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入要更新的联系人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子邮件]</td> 
   <td>输入要更新其详细信息的联系人的电子邮件地址。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL属性]</td> 
   <td>填写您要为记录设置的任何属性。 可用字段取决于要创建的记录类型。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块会删除联系人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要删除的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入您要删除的联系人、公司或交易的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取记录资产]

此操作模块通过其（内部）名称获取特定记录属性的元数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要为其检索元数据的属性的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL属性名称]</td> 
   <td>选择要为其检索元数据的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选项ID]</td> 
   <td> <p> 某些属性具有一组可用选项，用户可以选择这些选项作为属性值。 输入表示要检索的属性值的选项的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视记录]

此触发器模块会在最近30天内修改或创建联系人、公司或交易时启动一个方案。 输出限制为10,000条记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择包含要监视的属性的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>选择您是要查看最近修改的记录还是最近创建的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出属性]</td> 
   <td>选择要包含在模块输出中的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 联系人

* [[!UICONTROL 创建/更新联系人（旧版）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 创建/更新一组联系人]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 将联系人添加到列表]](#add-contacts-to-a-list)
* [[!UICONTROL 从列表中删除联系人]](#remove-a-contact-from-a-list)
* [[!UICONTROL 合并联系人]](#merge-contacts)
* [[!UICONTROL 搜索联系人]](#search-for-contacts)
* [[!UICONTROL 列出联系人]](#list-contacts)
* [[!UICONTROL 公司联系人列表]](#list-contacts-of-a-company)

#### [!UICONTROL 创建/更新联系人（旧版）]

如果门户中不存在联系人，则创建该联系人；如果门户中存在联系人，则使用最新的属性值对其进行更新。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL属性]</td> 
   <td>填写您要为联系人设置或更新的任何属性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建/更新一组联系人]

创建一组联系人或更新他们（如果他们已存在）。 当批量大小限制为100个或更少联系人时，性能最佳。 通过此端点所做的更改会异步处理，因此可能需要几分钟时间才能将更改应用到联系记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要创建/更新的联系人批次] </td> 
   <td> <p>添加批联系人。</p> <p>单击 <strong>[!UICONTROL添加项目]</strong> 添加新联系人。 在出现的窗口中，输入或映射以下信息：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL搜索类型]</strong> </p> <p>选择您希望如何识别联系人：</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>输入要创建或更新的联系人的ID。 </p> </li> 
       <li> <p>[!UICONTROL电子邮件]</p> <p>输入要创建或更新的联系人的电子邮件地址。 </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL属性]</strong> </p> <p>填写要为联系人设置或更新的任何属性。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将联系人添加到列表]

此模块将系统中已创建的联系人记录添加到联系人列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL列表ID] </td> 
   <td>选择要将联系人添加到的列表的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID/电子邮件] </td> 
   <td> <p>选择您希望如何标识要添加到列表的联系人：</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> <p>添加要添加到列表的联系人的ID。</p> </li> 
     <li> <p>[!UICONTROL电子邮件]</p> <p>添加要添加到列表的联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从列表中删除联系人]

从联系人列表中删除联系人。

>[!NOTE]
>
>您无法从动态列表中手动删除联系人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL列表ID] </td> 
   <td>选择要从中删除联系人的列表的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL联系人ID] </td> 
   <td>输入要从列表中删除的联系人的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合并联系人]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>输入要合并的其中一个联系人的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>输入要合并的其他联系人的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索联系人]

使用搜索查询检索联系人列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询]</td> 
   <td>输入搜索查询。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td>输入或映射最大联系人数 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出联系人]

返回在门户中创建的所有联系人。 输出限制为5000个联系人。 要列出前一个或下一个联系人，可使用 [!UICONTROL 高级] 用于偏移列表的参数。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>最大联系人数 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出属性]</td> 
   <td>选择要在模块输出中显示的属性。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 公司联系人列表]

检索公司中的联系人列表。 输出限制为5000个联系人。 要列出前一个或下一个联系人，可使用 [!UICONTROL 高级] 用于偏移列表的参数。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入要列出其联系人的公司的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>最大联系人数 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 监视联系人已添加到列表]

当将新联系人添加到列表时，此触发模块会启动一个方案。 此设置仅适用于具有付费营销帐户的用户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL列表ID]</td> 
   <td>输入或映射包含要监视的联系人的列表ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出属性]</td> 
   <td>选择要包含在模块输出中的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 交易

* [[!UICONTROL 列出交易/票证管道]](#list-dealticket-pipelines)
* [[!UICONTROL 获取交易的CRM管道]](#get-a-deals-crm-pipeline)

#### [!UICONTROL 列出交易/票证管道]

返回给定门户的所有交易和票证管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL对象类型] </td> 
   <td>选择要列出交易还是票证。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取交易的CRM管道]

返回特定交易管道……

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL管线ID] </td> 
   <td>输入或映射要检索其详细信息的管道的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL阶段ID] </td> 
   <td>输入或映射要检索其详细信息的阶段的ID。 </td> 
  </tr> 
 </tbody> 
</table>

### 公司

#### [!UICONTROL 按域搜索公司]

根据与域属性的完全匹配项检索公司列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL域] </td> 
   <td>输入要搜索的公司的域，例如 <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>公司的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出属性]</td> 
   <td>选择要在模块输出中显示的属性。 </td> 
  </tr> 
 </tbody> 
</table>

### 文件

* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 删除文件夹]](#delete-a-folder)
* [[!UICONTROL 移动文件]](#move-a-file)

#### [!UICONTROL 创建文件夹]

此模块会创建一个文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹名称] </td> 
   <td>输入或映射新文件夹的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL父文件夹ID] </td> 
   <td>选择要创建的文件夹的父文件夹的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件夹]

将文件夹标记为已删除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入要删除的文件夹的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动文件]

将文件移动到其他文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件ID] </td> 
   <td>输入或映射要移动的文件的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹ID] </td> 
   <td>选择要移动文件的文件夹的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名称]</td> 
   <td>输入已移动文件的名称。</td> 
  </tr> 
 </tbody> 
</table>

### 票证

#### [!UICONTROL 删除票证]

按其ID删除现有票证。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入要删除的票证的ID。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 进行API调用]

允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL HubSpot CRM] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于https://api.hubapi.com/的路径。 例如， /contacts/v1/lists/all/contacts/all</p> <p>有关可用端点的列表，请参阅 <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API文档</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>选择要使用的HTTP方法：</p> <p>[!UICONTROLGET]</p> <p>检索条目的信息。</p> <p>[!UICONTROLPOST]</p> <p>创建新条目。</p> <p>[!UICONTROLPUT]</p> <p>更新/替换现有条目。</p> <p>[!UICONTROLPATCH]</p> <p>进行部分条目更新。</p> <p>[!UICONTROLDELETE]</p> <p>删除条目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p> 输入所需的请求标头。 您无需添加授权标头；我们已经为你做了。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。使用条件语句(例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 以下API调用会返回 [!DNL HubSpot] 帐户：
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**方法**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>搜索的匹配项可在模块的输出下找到 [!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL 联系人].
>
>在本例中，返回了3个联系人：
>
>![](assets/hubspot-api-output.png)

## 创建新应用程序

1. 登录到 [!DNL HubSpot] 开发人员帐户。
1. 选择 **[!UICONTROL 创建应用程序]** 选项。
1. 输入应用程序名称和 [!UICONTROL 保存] 对话框。
1. 选择您的WebHook所需的范围。

   例如，添加联系人范围，以在创建或删除新联系人时触发模块。

   的 [!UICONTROL 联系范围] 是接收联系人、交易和公司事件webhook所需的全部内容。

   >[!IMPORTANT]
   >
   >请勿在 [!UICONTROL 重定向URL] 字段。
