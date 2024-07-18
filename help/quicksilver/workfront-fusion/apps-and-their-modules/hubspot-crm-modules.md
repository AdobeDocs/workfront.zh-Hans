---
title: HubSpot CRM模块
description: 通过 [!DNL Adobe Workfront Fusion] HubSpot CRM模块，您可以监视 [!DNL HubSpot CRM] 帐户中的事件、记录、联系人、预约、文件和表单提交，或者创建、检索、更新和删除记录、联系人、预约、事件或文件。
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM]模块

通过[!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM]模块，您可以监视事件、记录、联系人、预约、文件和表单提交，或者创建、检索、更新和删除您[!DNL HubSpot CRM]帐户中的记录、联系人、预约、事件或文件。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL HubSpot CRM]模块，您必须具有[!DNL HubSpot CRM]帐户。

## 将[!DNL Adobe Workfront Fusion]连接到[!DNL HubSpot CRM]

有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅[创建与 [!DNL Adobe Workfront Fusion] 的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>配置连接时，请选择&#x200B;**HubSpot CRM**&#x200B;连接类型。 HubSpot CRM（已弃用）类型支持现有连接，但我们不建议使用它来创建新连接。

## [!DNL HubSpot CRM]模块及其字段

配置[!DNL Hubspot CRM]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Hubspot CRM]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

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

此搜索模块按自定义属性或查询搜索CRM对象。 要搜索产品或行项目，请使用具有所需自定义范围的特殊连接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射模块在一个执行周期中返回的最大项数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要搜索的对象类型]</td> 
   <td>选择要搜索的Hubspot CRM对象的类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出属性]</td> 
   <td>选择要显示在模块输出中的属性。 可用字段取决于您选择的对象。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL过滤方式] </td> 
   <td> <p>选择您希望如何筛选搜索</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL查询]</strong> </p> <p>输入或映射查询</p> </li> 
     <li> <p><strong>[！UICONTROL属性]</strong> </p> <p>输入搜索的组或筛选器。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方式]</td> 
   <td> <p>如果要对结果进行排序，请单击。 如果选择对结果进行排序，则会显示以下字段。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL属性名称]</strong> </p> <p>选择要按其排序结果的属性</p> </li> 
     <li> <p><strong>[！UICONTROL方向]</strong> </p> <p>选择是否要以升序或降序方向对结果进行排序。</p> </li> 
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
* [[!UICONTROL 获取记录属性]](#get-a-record-property)
* [[!UICONTROL 观看记录]](#watch-records)

#### [!UICONTROL 创建记录（旧版）]

此操作模块创建联系人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL属性]</td> 
   <td>填写要为记录设置的任何属性。 可用字段取决于您要创建的记录类型。</td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择记录类型。</p> 
    <ul> 
     <li>[！UICONTROL联系人]</li> 
     <li>[！UICONTROL Company] </li> 
     <li>[！UICONTROL交易]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索类型]</td> 
   <td>如果您正在获取联系人，请选择是要通过ID还是电子邮件地址来识别联系人。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入要检索的联系人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL电子邮件]</td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择要更新的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索类型]</td> 
   <td> <p>如果您要获得联系人，请选择您希望如何识别记录：</p> 
    <ul> 
     <li> <p>[！UICONTROL ID]</p> </li> 
     <li> <p>[！UICONTROL电子邮件]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入要更新的联系人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL电子邮件]</td> 
   <td>输入要更新其详细信息的联系人的电子邮件地址。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL属性]</td> 
   <td>填写要为记录设置的任何属性。 可用字段取决于您要创建的记录类型。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块可删除联系人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择要删除的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入要删除的联系人、公司或交易的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取记录属性]

此操作模块通过特定记录属性的（内部）名称获取该属性的元数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择具有您要为其检索元数据的属性的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL属性名称]</td> 
   <td>选择要为其检索元数据的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选项ID]</td> 
   <td> <p> 某些属性具有一组可用选项，用户可以选择这些选项作为属性值。 输入表示要检索的属性值的选项的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看记录]

此触发器模块会在联系人、公司或交易在过去30天内被修改或创建时启动场景。 输出限制为10,000条记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td>选择具有要监视的属性的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索]</td> 
   <td>选择您要监视最近修改的记录还是最近创建的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出属性]</td> 
   <td>选择要包含在模块输出中的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 联系人

* [[!UICONTROL 创建/更新联系人（旧版）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 创建/更新联系人组]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 将联系人添加到列表]](#add-contacts-to-a-list)
* [[!UICONTROL 从列表中删除联系人]](#remove-a-contact-from-a-list)
* [[!UICONTROL 合并联系人]](#merge-contacts)
* [[!UICONTROL 搜索联系人]](#search-for-contacts)
* [[!UICONTROL 列出联系人]](#list-contacts)
* [[!UICONTROL 列出公司的联系人]](#list-contacts-of-a-company)

#### [!UICONTROL 创建/更新联系人（旧版）]

如果门户中不存在联系人，则创建联系人；如果门户中不存在联系人，则使用最新属性值更新联系人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL属性]</td> 
   <td>填写您要为联系人设置或更新的任何属性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建/更新联系人组]

创建联系人组或更新他们（如果已经存在）。 当批次大小限制为100个或更少联系人时，性能最佳。 通过此端点进行的更改是异步处理的，因此可能需要几分钟才能将更改应用到联系人记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要创建/更新的联系人批次] </td> 
   <td> <p>添加联系人批次。</p> <p>单击<strong>[！UICONTROL添加项]</strong>以添加新联系人。 在出现的窗口中，输入或映射以下信息：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL搜索类型]</strong> </p> <p>选择您希望如何识别联系人：</p> 
      <ul> 
       <li> <p>[！UICONTROL ID]</p> <p>输入要创建或更新的联系人的ID。 </p> </li> 
       <li> <p>[！UICONTROL电子邮件]</p> <p>输入要创建或更新的联系人的电子邮件地址。 </p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL属性]</strong> </p> <p>填写您要为联系人设置或更新的任何属性。</p> </li> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID] </td> 
   <td>选择要向其添加联系人的列表的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID/电子邮件] </td> 
   <td> <p>选择您希望如何识别要添加到列表中的联系人：</p> 
    <ul> 
     <li> <p>[！UICONTROL IDs]</p> <p>添加要添加到列表中的联系人的ID。</p> </li> 
     <li> <p>[！UICONTROL电子邮件]</p> <p>添加要添加到列表中的联系人的电子邮件地址。</p> </li> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID] </td> 
   <td>选择要从中删除联系人的列表的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL联系人ID] </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID 1] </td> 
   <td>输入要合并的联系人的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID 2] </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Query]</td> 
   <td>输入搜索查询。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>输入或映射在一个方案执行周期内应返回的最大联系人数[!DNL Workfront Fusion]。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出联系人]

返回在门户中创建的所有联系人。 输出限制为5000个联系人。 若要列出上一个或下一个联系人，您可以使用[!UICONTROL advanced]参数偏移列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>在一个方案执行周期内应返回的最大联系人数[!DNL Workfront Fusion]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出属性]</td> 
   <td>选择要显示在模块输出中的属性。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 列出公司的联系人]

检索公司中的联系人列表。 输出限制为5000个联系人。 若要列出上一个或下一个联系人，您可以使用[!UICONTROL advanced]参数偏移列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入要列出其联系人的公司的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>在一个方案执行周期内应返回的最大联系人数[!DNL Workfront Fusion]。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 观看添加到列表中的联系人]

此触发器模块会在向列表添加新联系人后启动方案。 这仅适用于拥有付费营销帐户的用户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表ID]</td> 
   <td>输入或映射包含要监视的联系人的列表ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出属性]</td> 
   <td>选择要包含在模块输出中的属性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL对象类型] </td> 
   <td>选择您要列出交易还是票证。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取交易的CRM管道]

返回特定的交易管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL管道ID] </td> 
   <td>输入或映射要检索其详细信息的管道ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL阶段ID] </td> 
   <td>输入或映射要检索其详细信息的阶段的ID。 </td> 
  </tr> 
 </tbody> 
</table>

### 公司

#### [!UICONTROL 按域搜索公司]

根据与域属性的完全匹配检索公司列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL域] </td> 
   <td>输入要搜索公司的域，如<code>[!DNL hubspot].com</code>。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>在一个方案执行周期内应返回的最大公司数[!DNL Workfront Fusion]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出属性]</td> 
   <td>选择要显示在模块输出中的属性。 </td> 
  </tr> 
 </tbody> 
</table>

### 文件

* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 删除文件夹]](#delete-a-folder)
* [[!UICONTROL 移动文件]](#move-a-file)

#### [!UICONTROL 创建文件夹]

此模块创建一个文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹名称] </td> 
   <td>输入或映射新文件夹的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父文件夹ID] </td> 
   <td>为要创建的文件夹选择父文件夹的ID。 </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID] </td> 
   <td>输入或映射要移动的文件的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID] </td> 
   <td>选择要将文件移动到的文件夹的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称]</td> 
   <td>输入已移动文件的名称。</td> 
  </tr> 
 </tbody> 
</table>

### 票证

#### [!UICONTROL 删除票证]

按票证ID删除现有票证。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入要删除的票证ID。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 进行API调用]

允许您执行自定义API调用。

>[!NOTE]
>
>以下端点已于2023年8月31日在HubSpot API中弃用，并且在Fusion模块中无法再使用。
>
>* 列出内容事件
>* 列出社交事件
>* 列出日历任务事件
>* 列出所有日历事件
>* 创建日历任务
>* 按ID获取日历任务
>* 更新日历任务
>* 删除日历任务

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL HubSpot CRM]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对于https://api.hubapi.com/的路径。 例如， /contacts/v1/lists/all/contacts/all</p> <p>有关可用端点的列表，请参阅<a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API文档</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择要使用的HTTP方法：</p> <p>[！UICONTROLGET]</p> <p>检索条目的信息。</p> <p>[！UICONTROLPOST]</p> <p>以创建新条目。</p> <p>[！UICONTROLPUT]</p> <p>更新/替换现有条目。</p> <p>[！UICONTROLPATCH]</p> <p>更新部分条目。</p> <p>[！UICONTROLDELETE]</p> <p>以删除条目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p> 输入所需的请求标头。 您无需添加授权标头；我们已经为您添加了这些标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：**&#x200B;以下API调用返回您[!DNL HubSpot]帐户中的所有联系人：
>
>**URL**： `/contacts/v1/lists/all/contacts/all`
>
>**方法**： `GET`
>
>![](assets/hubspot-api-config.png)
>
>在[!UICONTROL 包] > [!UICONTROL 正文] > [!UICONTROL 联系人]下的模块输出中可以找到搜索匹配项。
>
>在我们的示例中，返回了3个联系人：
>
>![](assets/hubspot-api-output.png)

## 创建新应用程序

1. 登录到您的[!DNL HubSpot]开发人员帐户。
1. 选择&#x200B;**[!UICONTROL 创建应用程序]**&#x200B;选项。
1. 输入应用程序名称并[!UICONTROL 保存]对话框。
1. 选择webhook所需的范围。

   例如，添加联系人范围，以便在创建或删除新联系人时触发模块。

   [!UICONTROL 联系人范围]是接收联系人、交易和公司活动Webhook所需的所有内容。

   >[!IMPORTANT]
   >
   >请勿填写[!UICONTROL 重定向URL]字段。
