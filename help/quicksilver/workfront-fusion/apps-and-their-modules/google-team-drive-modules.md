---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google Team Drive模块
description: 通过 [!DNL Adobe Workfront Fusion Google Team Drive] 模块，您可以在 [!DNL Google Shared] 驱动器中监视、上传、更新、复制、删除或检索文件和创建文件夹。
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# [!DNL Google Team Drive]模块

通过[!DNL Adobe Workfront Fusion] [!DNL Google Team Drive]模块，您可以在[!DNL Google Shared Drive]中监视、上传、更新、复制、删除或检索文件和创建文件夹。

要将[!DNL Google Team Drive]与[!DNL Adobe Workfront Fusion]一起使用，需要具有[!DNL Google Workspace]帐户。 如果您没有帐户，则可以在[[!DNL Google Workspace] 注册站点](https://workspace.google.com/business/signup/welcome)创建一个[!DNL Google Workspace]帐户。

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Google Team Drive]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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

要使用[!DNL Google Team Drive]模块，您必须具有[!DNL Google Team Drive]。

## [!DNL Google Team Drive]模块及其字段

配置[!DNL Google Team Drive]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Google Team Drive]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

以&#x200B;**bold**（在[!DNL Workfront Fusion]方案中，此文档文章中为&#x200B;**not**）显示的模块对话框字段是必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 触发器

#### [!UICONTROL 监视文件]

在指定的文件夹中添加和/或修改新文件时，返回文件详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道]</td> 
   <td> <p> 选择要监视的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要查看的文件]</td> 
   <td> <p> 选择要监视的文件类型。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Documents]文件转换为格式] </td> 
   <td> <p>选择要将观察的[!DNL Google Documents]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Sheets]文件转换为格式] </td> 
   <td> <p>选择要将观察的[!DNL Google Sheets]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Slides]文件转换为格式] </td> 
   <td> <p>选择要将观察的[!DNL Google Slides]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Drawings]文件转换为格式] </td> 
   <td> <p>选择要将观察的[!DNL Google Drawings]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL监视]</td> 
   <td> <p> 选择是要监视文件夹中是否有新的和修改的文件，还是只监视新文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大下载文件数]</td> 
   <td> <p> 设置在一个执行周期内将返回的最大文件数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上载文件]](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 复制文件]](#copy-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 将文件移动到垃圾桶]](#move-a-file-to-trash)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 获取文件列表]](#get-a-file-list)
* [[!UICONTROL 创建文件夹]](#create-a-folder)

#### [!UICONTROL 上载文件]

将文件上载到指定的共享驱动器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道] </td> 
   <td> <p>选择要将文件上传到的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source File]</p> </td> 
   <td> <p>指定要上载到共享驱动器的文件。</p> <p>映射您要从上一个模块上传的文件(例如，[！UICONTROL HTTP] &gt;[！UICONTROL获取文件]或[！UICONTROLDropbox] &gt;[！UICONTROL获取文件)]，或手动输入文件名和文件数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标题]</td> 
   <td> <p> 输入将在共享文件夹中显示的文件标题。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换文件]</td> 
   <td> <p> 启用此选项以将文件转换为共享文件夹中相应的Google格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新文件]

允许您更改文件名和/或文件内容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道]</td> 
   <td> <p> 选择包含要更新的文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p> 输入（映射）要更新的文件ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source File]</p> </td> 
   <td>从上一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标题] </td> 
   <td> <p>为更新后的文件输入新标题。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换文件]</td> 
   <td> <p> 启用此选项以将文件转换为共享文件夹中相应的[!DNL Google]格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制文件]

将指定的文件复制到选定的文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道]</td> 
   <td> <p> 选择包含要复制文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要将文件复制到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p> 输入（映射）要复制的文件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL复制文件的名称]</p> </td> 
   <td> <p>如果要在目标位置更改新文件名，请输入新文件名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

删除指定的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p> 输入或映射要删除文件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将文件移动到垃圾桶]

将指定的文件移至垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p> 输入要移动到垃圾桶的文件的ID，或将其映射到垃圾桶。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

检索有关指定文件的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Documents]文件转换为格式] </td> 
   <td> <p>选择您希望将[!DNL Google Documents]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Sheets]文件转换为格式] </td> 
   <td> <p>选择您希望将[!DNL Google Sheets]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Slides]文件转换为格式] </td> 
   <td> <p>选择您希望将[!DNL Google Slides]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL将[!DNL Google Drawings]文件转换为格式] </td> 
   <td> <p>选择您希望将[!DNL Google Drawings]文件转换为的格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p> 输入或映射要检索的文件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件列表]

根据搜索词检索文件和/或文件夹详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道]</td> 
   <td> <p> 选择要从中列出文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要从中列出文件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索] </td> 
   <td> <p>选择要执行的搜索类型 — 请参阅下文。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Query]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[！UICONTROL在文件名中搜索]</p> <p style="font-weight: normal;">在选择[！UICONTROL搜索精确搜索词]选项时输入文件名（包括文件扩展名），或在选择[！UICONTROL搜索包含搜索词的名称]选项时输入名称的一部分。</p> </li> 
     <li> <p style="font-weight: bold;">[！UICONTROL全文搜索]</p> <p>输入搜索词以搜索文件名、说明和内容。</p> </li> 
     <li> <p style="font-weight: bold;">[！UICONTROL自定义搜索查询]</p> <p>输入[!DNL Google]搜索查询词。 有关详细信息，请参阅[!DNL Google]的<a href="https://developers.google.com/drive/api/v2/ref-search-terms">搜索查询文档</a>。 示例： <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Retrieve]</td> 
   <td>选择是要检索文件、文件夹还是两者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回结果的最大数目]</td> 
   <td> <p> 设置在一个执行周期内[!DNL Workfront Fusion]将返回的最大文件或文件夹数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

创建新文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google Team Drive]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL团队通道]</td> 
   <td> <p> 选择要创建文件夹的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要在其中创建文件夹的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新文件夹的名称]</td> 
   <td> <p> 输入新文件夹的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>
