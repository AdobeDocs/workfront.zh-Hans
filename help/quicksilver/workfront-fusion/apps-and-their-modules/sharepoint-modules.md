---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: SharePoint模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用SharePoint的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2850'
ht-degree: 0%

---

# [!DNL SharePoint] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL SharePoint]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL SharePoint] 模块，您必须具有 [!DNL SharePoint] 帐户。

## Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帐户](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion] 使用高级设置](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帐户

您可以使用 [!DNL Microsoft] 用于创建连接的帐户 [!DNL SharePoint]. 有关连接 [!DNL Sharepoint] 目标帐户 [!DNL Workfront Fusion]，请参见 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion] 使用高级设置

连接 [!DNL SharePoint] 到 [!DNL Workfront Fusion] 没有 [!DNL Microsoft] 帐户，您需要客户端ID、客户端密钥和租户ID。

1. 单击 **[!UICONTROL 添加]** 在顶部附近 **[!DNL SharePoint]** 框以打开 **[!UICONTROL 创建连接]** 盒子。

1. （可选）更改默认值 **[!UICONTROL 连接名称]**.
1. 单击 **[!UICONTROL 显示高级设置]**.
1. 输入 [!DNL SharePoint] **[!UICONTROL 客户端ID]** 和 **[!UICONTROL 客户端密码]**.

1. 单击 **[!UICONTROL 继续]**.
1. 在显示的登录窗口中，输入您的凭据以登录到应用程序（如果尚未登录）。
1. （视情况而定）如果 **[!UICONTROL 允许]** 按钮时，单击按钮以将应用程序连接到 [!DNL Workfront Fusion].

## [!DNL SharePoint] 模块及其字段

配置时 [!DNL SharePoint] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL SharePoint] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [驱动器项目](#drive-item)
* [项](#item)
* [列表](#list)
* [页面（测试版）](#page-beta)
* [站点](#site)
* [其他](#other)

### 驱动器项目

* [创建文件](#create-a-file)
* [创建文件夹](#create-a-folder)
* [获取文件](#get-a-file)
* [监视文件夹项目](#watch-folder-items)

#### 获取更改

此模块返回已在SharePoint中进行的更改。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点、驱动器和文件夹ID]</td> 
   <td> <p>选择您希望如何标识要检索更改的文件夹的位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL文件夹ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择要检索更改的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL令牌]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### 创建文件夹

此操作模块在SharePoint中创建新文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点、驱动器和文件夹ID]</td> 
   <td> <p>选择您希望如何标识要创建的文件夹的位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL文件夹ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择要创建文件夹的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹名称]</td> 
   <td>输入或映射新文件夹的名称。</td> 
  </tr>
  </tbody> 
</table>

#### 获取文件

此操作模块可检索指定的SharePoint文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点、驱动器和文件夹ID]</td> 
   <td> <p>选择您希望如何标识要获取的文件位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL文件ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择文件的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### 监视文件夹项目

当您选择的文件夹中更新了某个项目时，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点、驱动器和文件夹ID]</td> 
   <td> <p>选择您希望如何标识要获取的文件位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL文件夹ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择要监视的文件夹的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入物料的最大数量 [!DNL Workfront Fusion] 应在一个场景执行周期中返回。</td> 
  <tr>
  </tr>
</tbody> 
</table>

### 项

* [[!UICONTROL 复制项目]](#copy-an-item)
* [[!UICONTROL 创建项目]](#create-an-item)
* [[!UICONTROL 删除项目]](#delete-an-item)
* [[!UICONTROL 获取项目]](#get-an-item)
* [[!UICONTROL 列表项]](#list-items)
* [[!UICONTROL 移动项目]](#move-an-item)
* [[!UICONTROL 更新项目]](#update-an-item)
* [[!UICONTROL 监视项目] （已计划）](#watch-items-scheduled)


#### [!UICONTROL 复制项目]

此操作模块复制SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">输入站点、驱动器和文件夹ID</td> 
   <td> <p>选择您希望如何标识站点以及包含要复制项目的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL项目ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>在“项目类型”字段中，选择是移动字段还是文件夹。  选择包含要复制项目的站点，然后选择列表，然后选择项目。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目标ID]</td> 
   <td> 输入或映射项目复制目标文件夹的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名称]</td> 
   <td>输入或映射项目新副本的名称。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建项目]

此操作模块在SharePoint列表中创建新项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL创建项目]</td> 
   <td> <p>选择您希望如何标识站点以及您希望创建项目的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 和 <strong>[！UICONTROL列表ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要创建项目的列表的站点，然后选择列表。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段]</td> 
   <td>对于要为新项目设置的每个字段，输入该字段的键（标识该字段），以及您希望新项目在该字段中的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除项目]

此操作模块删除SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新项]</td> 
   <td> <p>选择您希望如何标识站点以及包含要删除的项目的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL项目ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要删除的项目的站点，然后选择列表，然后选择该项目。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取项目]

此操作模块返回指定项的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取项]</td> 
   <td> <p>选择您希望如何标识网站以及包含您要获取的项目列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL项目ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要从中检索项目的列表的站点，然后选择该列表，然后选择该项目。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表项]

此操作模块检索指定列表中所有项目的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表项]</td> 
   <td> <p>选择您希望如何标识要从中检索项目的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 和 <strong>[！UICONTROL列表ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要从中检索项目的列表的站点，然后选择列表。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大项目数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动项目]

此操作模块复制SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">输入站点、驱动器和文件夹ID</td> 
   <td> <p>选择您要如何标识站点以及包含要移动项目的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL项目ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>在“项目类型”字段中，选择是移动字段还是文件夹。 选择包含要复制项目的站点，然后选择列表，然后选择项目。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目标ID]</td> 
   <td> 输入或映射要将项目移动到的文件夹的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名称]</td> 
   <td>输入或映射已移动项目的名称。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新项目]

此操作模块更新SharePoint列表中的现有项目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新项]</td> 
   <td> <p>选择您要如何标识包含要更新的项目的站点和列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL列表ID]</strong>、和 <strong>[！UICONTROL项目ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新的项目的地点，然后选择列表，然后选择项目。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段]</td> 
   <td>对于要更新新项目的每个字段，请输入该字段的键值（标识该字段），以及希望项目为该字段提供的新值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视项目] （已计划）

此触发器模块在创建或修改项目时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视列表]</td> 
   <td>选择是要按创建时间（新项目）还是按修改时间（更新项目）监视列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点和列表ID]</td> 
   <td> <p>选择您希望如何识别要观看的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 和 <strong>[！UICONTROL列表ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择要监视的站点，然后选择列表。 这些下拉列表仅检索关注的网站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大项目数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 列表

* [[!UICONTROL 创建列表]](#create-a-list)
* [[!UICONTROL 获取列表]](#get-a-list)
* [[!UICONTROL 列表列表]](#list-lists)
* [[!UICONTROL 观察列表]](#watch-lists)

#### [!UICONTROL 创建列表]

此操作模块在SharePoint中创建新列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点ID]</td> 
   <td> <p>选择您希望如何标识站点以及要在其中创建列表的列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 要在其中创建列表的位置。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择要创建列表的站点。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示名称]</td> 
   <td>输入或映射新列表的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL描述]</td> 
   <td>输入或映射新列表的说明。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL添加列]</td> 
   <td>对于要为新列表设置的每一列，输入 <strong>[！UICONTROL名称]</strong> ，然后选择 <strong>[！UICONTROL类型]</strong> 您希望新列具有的值。</td> 
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
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取列表]</td> 
   <td> <p>选择您希望如何标识网站以及包含您要获取的项目列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 和 <strong>列表编号</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的列表的站点，然后选择该列表。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表列表]

此操作模块检索指定列表中所有项目的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列表列表]</td> 
   <td> <p>选择您希望如何标识要从其中检索列表的站点。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的列表的站点。 下拉列表只会检索您关注的站点。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大列表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观察列表]

此触发器模块会在创建或修改列表时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视列表]</td> 
   <td>选择是要按创建时间（新项目）还是按修改时间（更新项目）监视列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点和列表ID]</td> 
   <td> <p>选择您希望如何识别要观看的网站和列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong> 您要观看的列表所在的位置。</p> </li> 
     <li> <p><strong>[！UICONTROL从您关注的列表中选择]</strong> </p> <p>选择要监视的站点。 下拉列表只会检索您关注的站点。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大列表数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 页面（测试版）

>[!NOTE]
>
>中的API `beta` 中的版本 [!DNL Microsoft Graph] 随时可能更改。 不支持在生产应用程序中使用这些API。

#### [!UICONTROL 获取页面]

此操作模块返回指定页面的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取页面]</td> 
   <td> <p>选择您希望如何标识要检索的页面。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>和 <strong>[！UICONTROL页面ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要检索的页面的站点，然后选择该页面。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 站点

* [[!UICONTROL 获取站点]](#get-a-site)
* [[!UICONTROL 搜索站点]](#search-sites)

#### [!UICONTROL 获取站点]

此操作模块返回指定站点的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取站点]</td> 
   <td> <p>选择您希望如何标识要检索的页面。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择要检索的站点。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索站点]

此操作模块按您指定的参数搜索站点。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">显示名称的[！UICONTROL关键字]</td> 
   <td> <p>输入或映射要搜索网站的搜索词。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大站点数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### 获取更改

此模块可检索在SharePoint文件夹中所做的添加、更新和删除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入站点、驱动器和文件夹ID]</td> 
   <td> <p>选择您要如何标识包含要更新的项目的站点和列表。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射 <strong>[！UICONTROL站点ID]</strong>， <strong>[！UICONTROL驱动器ID]</strong>、和 <strong>[！UICONTROL文件夹ID]</strong> 在显示的字段中。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新的项目的站点，然后选择驱动器，然后选择文件夹。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL令牌]</td> 
   <td> 令牌标识模块应从何时开始检索更改。  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL SharePoint] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对路径 <code>https://graph.microsoft.com</code>. 示例:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型]</td> 
   <td>选择您要在API调用中发送的数据类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 观看活动

在SharePoint中添加、更新或删除项目时，此即时触发器模块会启动一个场景。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择现有的webhook，或单击“添加”创建新的webhook。</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

