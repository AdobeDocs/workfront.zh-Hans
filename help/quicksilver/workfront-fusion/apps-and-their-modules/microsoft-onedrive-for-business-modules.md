---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Microsoft OneDrive for Business]，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Microsoft OneDrive for Business]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Microsoft OneDrive for Business] with [!DNL Adobe Workfront Fusion]，您将需要 [!DNL Microsoft] 帐户。

有关连接 [!DNL OneDrive for Business] 帐户 [!DNL Workfront Fusion]，请参阅 [创建连接到Adobe [!DNL Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] 模块及其字段

配置 [!DNL Microsoft OneDrive for Business] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Microsoft OneDrive for Business] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL 监视文件]](#watch-files)
* [[!UICONTROL 监视文件夹]](#watch-folders)

#### [!UICONTROL 监视文件]

在正在监视的文件夹中添加或更新新文件时，此触发器模块会激活。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL驱动器ID]</p> </td> 
   <td> <p>选择要监视的驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td> <p> 选择要监视的文件夹。 在方案中，您只能监视一个文件夹。</p> <p>提示：要跟踪多个文件夹，请为每个文件夹创建独立方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL，我要观看]</p> </td> 
   <td> <p>选择是要监视新文件和所有更改，还是仅监视新文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回行数的最大值]</td> 
   <td> <p> 设置 [!DNL Workfront Fusion] 可在一个周期内使用。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视文件夹]

当向正在监视的文件夹中添加新文件夹时，此触发器模块会激活。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL驱动器ID]</p> </td> 
   <td> <p>选择要监视的驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td> <p> 选择要监视的文件夹。 在方案中，您只能监视一个文件夹。</p> <p>提示：要跟踪多个文件夹，请为每个文件夹创建独立方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL，我要观看]</p> </td> 
   <td> <p>选择是要监视新文件夹和所有更改，还是仅监视新文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回行数的最大值]</td> 
   <td> <p> 设置 [!DNL Workfront Fusion] 可在一个周期内使用。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 删除文件夹]](#delete-a-folder)
* [[!UICONTROL 获取共享链接]](#get-a-sharing-link)

#### [!UICONTROL 上传文件]

此操作模块将二进制文件或文本文件上传到指定的文件夹

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要将文件上传到的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择驱动器中的文件夹。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源文件]</p> </td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL如果存在同名文件]</td> 
   <td> <p> 如果已存在与您尝试上传的文件同名的文件，请选择要执行的操作。</p> 
    <ul> 
     <li>[!UICONTROL替换现有文件]</li> 
     <li>[!UICONTROL重命名新文件]</li> 
     <li>[!UICONTROL结束时出错]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

此操作模块将指定的文件移动到回收站。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中删除文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p>输入要删除的文件的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块检索具有给定ID的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中检索文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p>输入要检索的文件的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定的父文件夹内创建文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL连接]</strong> </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL驱动器ID]</strong> </td> 
   <td> <p>选择要创建新文件夹的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL文件夹]</strong> </td> 
   <td> <p>选择要在中创建新文件夹的文件夹。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL文件夹名称]</strong> </td> 
   <td>输入或映射新文件夹的名称。</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件夹]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中删除文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹ID]</td> 
   <td> <p>输入或映射要删除的文件夹的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取共享链接]

此模块将检索可共享以访问指定文件的链接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驱动器ID]</td> 
   <td> <p>选择要将文件上传到的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>选择是使用文件ID还是文件路径选择文件。 在显示的字段中输入文件ID或路径。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL权限类型]</p> </td> 
   <td> <p>选择您希望收到链接的人员具有读/写权限还是只读权限。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL范围]</td> 
   <td> <p> 选择您希望任何具有链接的人员是否可以访问该文件，还是仅让您的组织成员可以访问该文件。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
