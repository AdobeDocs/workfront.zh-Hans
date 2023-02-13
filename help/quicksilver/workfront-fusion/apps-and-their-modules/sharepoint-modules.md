---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: SharePoint模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用SharePoint的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1951'
ht-degree: 0%

---

# [!DNL SharePoint] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL SharePoint]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL SharePoint] 模块，您必须 [!DNL SharePoint] 帐户。

## 连接 [!DNL SharePoint] to [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [连接 [!DNL SharePoint] to [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帐户](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [连接 [!DNL SharePoint] to [!DNL Workfront Fusion] 使用高级设置](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### 连接 [!DNL SharePoint] to [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帐户

您可以使用 [!DNL Microsoft] 帐户以创建连接 [!DNL SharePoint]. 有关连接 [!DNL Sharepoint] 帐户 [!DNL Workfront Fusion]，请参阅 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

### 连接 [!DNL SharePoint] to [!DNL Workfront Fusion] 使用高级设置

连接 [!DNL SharePoint] to [!DNL Workfront Fusion] 没有 [!DNL Microsoft] 帐户时，您需要客户端ID、客户端密钥和租户ID。

1. 单击 **[!UICONTROL 添加]** 在 **[!DNL SharePoint]** 框 **[!UICONTROL 创建连接]** 框中。

1. （可选）更改默认 **[!UICONTROL 连接名称]**.
1. 单击 **[!UICONTROL 显示高级设置]**.
1. 输入 [!DNL SharePoint] **[!UICONTROL 客户端ID]** 和 **[!UICONTROL 客户端密钥]**.

1. 单击 **[!UICONTROL 继续]**.
1. 在显示的登录窗口中，输入您的凭据以登录到应用程序（如果尚未登录）。
1. （视情况而定）如果 **[!UICONTROL 允许]** 按钮，单击按钮以将应用程序连接到 [!DNL Workfront Fusion].

## [!DNL SharePoint] 模块及其字段

配置 [!DNL SharePoint] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL SharePoint] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [项](#item)
* [列表](#list)
* [页面（测试版）](#page-beta)
* [网站](#site)
* [其他](#other)

### 项

* [[!UICONTROL 监视项目]](#watch-items)
* [[!UICONTROL 列表项]](#list-items)
* [[!UICONTROL 获取项目]](#get-an-item)
* [[!UICONTROL 创建项目]](#create-an-item)
* [[!UICONTROL 更新项目]](#update-an-item)
* [[!UICONTROL 删除项目]](#delete-an-item)

#### [!UICONTROL 监视项目]

此触发器模块会在创建或修改项目时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL监视列表]</td> 
   <td>按创建时间（新项目）还是修改时间（更新项目）选择您要监视列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入站点和列表ID]</td> 
   <td> <p>选择您希望如何识别要监视的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 和 <strong>[!UICONTROL列表ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从您所关注的列表中选择]</strong> </p> <p>选择要监视的网站，然后选择列表。 这些下拉列表仅检索后跟的网站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大项目数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表项]

此操作模块可检索指定列表中所有项目的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL列表项]</td> 
   <td> <p>选择您希望如何标识要从中检索项目的列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 和 <strong>[!UICONTROL列表ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要从中检索项目的列表的网站，然后选择该列表。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大项目数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取项目]

此操作模块会返回指定项目的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL获取项目]</td> 
   <td> <p>选择您希望如何识别包含要获取的项目的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>, <strong>[!UICONTROL列表ID]</strong>和 <strong>[!UICONTROL项目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要从中检索项目的列表的网站，然后选择该列表，然后选择该项目。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建项目]

此操作模块会在SharePoint列表中创建新项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL创建项目]</td> 
   <td> <p>选择您希望如何识别网站并列出要创建项目的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 和 <strong>[!UICONTROL列表ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要创建项目的列表的网站，然后选择该列表。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL字段]</td> 
   <td>对于要为新项目设置的每个字段，输入字段的键（标识字段）以及您希望新项目对该字段具有的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新项目]

此操作模块会更新SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新项目]</td> 
   <td> <p>选择您希望如何识别包含要更新项目的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>, <strong>[!UICONTROL列表ID]</strong>和 <strong>[!UICONTROL项目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新项目的网站，然后选择列表，然后选择项目。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL字段]</td> 
   <td>对于要为新项目更新的每个字段，输入字段的键（标识字段）以及您希望该项目在该字段中具有的新值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除项目]

此操作模块会删除SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新项目]</td> 
   <td> <p>选择您希望如何识别包含要删除项目的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>, <strong>[!UICONTROL列表ID]</strong>和 <strong>[!UICONTROL项目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要删除的项目的网站，然后选择列表，然后选择该项目。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 列表

* [[!UICONTROL 监视列表]](#watch-lists)
* [[!UICONTROL 列表列表]](#list-lists)
* [[!UICONTROL 获取列表]](#get-a-list)
* [[!UICONTROL 创建列表]](#create-a-list)

#### [!UICONTROL 监视列表]

创建或修改列表时，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL监视列表]</td> 
   <td>按创建时间（新项目）还是修改时间（更新项目）选择您要监视列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入站点和列表ID]</td> 
   <td> <p>选择您希望如何识别要监视的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 要监视的列表所在的位置。</p> </li> 
     <li> <p><strong>[!UICONTROL从您所关注的列表中选择]</strong> </p> <p>选择要监视的网站。 下拉列表仅检索您关注的网站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大列表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表列表]

此操作模块可检索指定列表中所有项目的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL列表]</td> 
   <td> <p>选择您希望如何识别要从中检索列表的网站。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的列表的网站。 下拉列表仅检索您关注的网站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大列表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取列表]

此操作模块返回指定列表的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL获取列表]</td> 
   <td> <p>选择您希望如何识别包含要获取的项目的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 和 <strong>列表ID</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的列表的网站，然后选择该列表。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建列表]

此操作模块会在SharePoint中创建新列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入网站ID]</td> 
   <td> <p>选择您希望如何识别网站并列出要创建列表的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong> 创建列表。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择要创建列表的网站。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示名称]</td> 
   <td>输入或映射新列表的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td>输入或映射新列表的描述。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Add Columns]</td> 
   <td>对于要为新列表设置的每列，输入 <strong>[!UICONTROL名称]</strong> ，然后选择 <strong>[!UICONTROL Type]</strong> 的值。</td> 
  </tr> 
 </tbody> 
</table>

### 页面（测试版）

>[!NOTE]
>
>中的API `beta` 版本 [!DNL Microsoft Graph] 可能会发生变化。 不支持在生产应用程序中使用这些API。

#### [!UICONTROL 获取页面]

此操作模块会返回指定页面的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL获取页面]</td> 
   <td> <p>选择要如何标识要检索的页面。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>和 <strong>[!UICONTROL页面ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的页面的网站，然后选择该页面。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 网站

* [[!UICONTROL 搜索站点]](#search-sites)
* [[!UICONTROL 获取网站]](#get-a-site)

#### [!UICONTROL 搜索站点]

此操作模块会按您指定的参数搜索站点。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！显示名称的UICONTROL关键字]</td> 
   <td> <p>输入或映射要搜索网站的搜索词。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大站点数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取网站]

此操作模块会返回指定站点的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL获取站点]</td> 
   <td> <p>选择要如何标识要检索的页面。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>输入或映射 <strong>[!UICONTROL网站ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择要检索的网站。</p> </li> 
    </ul> </td> 
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
   <td> <p>有关连接 [!DNL SharePoint] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">连接 [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于 <code>https://graph.microsoft.com</code>. 示例:<code> /beta/sites</code></p> </td> 
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
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>选择要在API调用中发送的数据类型。</td> 
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

