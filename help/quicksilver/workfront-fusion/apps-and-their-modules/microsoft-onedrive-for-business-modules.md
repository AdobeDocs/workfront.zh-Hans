---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动使用 [!DNL Microsoft OneDrive for Business]的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Microsoft OneDrive for Business]的工作流，并将其连接到多个第三方应用程序和服务。

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

若要将[!DNL Microsoft OneDrive for Business]与[!DNL Adobe Workfront Fusion]一起使用，您需要一个[!DNL Microsoft]帐户。

有关将[!DNL OneDrive for Business]帐户连接到[!DNL Workfront Fusion]的说明，请参阅[创建与Adobe的连接 [!DNL Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)



## 正在将[!DNL Microsoft OneDrive for Business]服务连接到[!DNL Workfront Fusion]

有关将[!DNL Microsoft OneDrive for Business]帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅[创建与[!UICONTROL Adobe Workfront Fusion]的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>某些Microsoft应用程序使用相同的连接，该连接与单个用户权限相关联。 因此，在创建连接时，权限同意屏幕除了显示当前应用程序所需的任何新权限外，还会显示以前授予此用户连接的任何权限。
>
>例如，如果用户拥有通过Excel Connector授予的“读取表”权限，然后在Outlook Connector中创建连接以读取电子邮件，则权限同意屏幕将显示已授予的“读取表”权限和新要求的“写入电子邮件”权限。

## [!DNL Microsoft OneDrive for Business]模块及其字段

配置[!DNL Microsoft OneDrive for Business]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Microsoft OneDrive for Business]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL 监视文件]](#watch-files)
* [[!UICONTROL 监视文件夹]](#watch-folders)

#### [!UICONTROL 监视文件]

在被监视的文件夹中添加或更新新文件时，此触发器模块将激活。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL驱动器ID]</p> </td> 
   <td> <p>选择要监视的驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹]</td> 
   <td> <p> 选择要监视的文件夹。 在场景中，您只能监视一个文件夹。</p> <p>提示：要跟踪多个文件夹，请为每个文件夹创建一个独立的方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL我要观看]</p> </td> 
   <td> <p>选择是要监视新文件和所有更改，还是只监视新文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大行数]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内可处理的最大结果数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视文件夹]

在将新文件夹添加到受监视的文件夹时，此触发器模块将激活。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL驱动器ID]</p> </td> 
   <td> <p>选择要监视的驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹]</td> 
   <td> <p> 选择要监视的文件夹。 在场景中，您只能监视一个文件夹。</p> <p>提示：要跟踪多个文件夹，请为每个文件夹创建一个独立的方案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL我要观看]</p> </td> 
   <td> <p>选择是要监视新文件夹和所有更改，还是只监视新文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回的最大行数]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内可处理的最大结果数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上载文件]](#upload-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 删除文件夹]](#delete-a-folder)
* [[!UICONTROL 获取共享链接]](#get-a-sharing-link)

#### [!UICONTROL 上载文件]

此操作模块会将二进制文件或文本文件上传到指定的文件夹

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL驱动器ID]</td> 
   <td> <p>选择要将文件上传到的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择驱动器中的文件夹。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source File]</p> </td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL如果存在同名文件]</td> 
   <td> <p> 选择当与正在尝试上载的文件同名的文件已存在时要执行的操作。</p> 
    <ul> 
     <li>[！UICONTROL替换现有文件]</li> 
     <li>[！UICONTROL重命名新文件]</li> 
     <li>[！UICONTROL以错误结尾]</li> 
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
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中删除文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p>输入要删除的文件的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块会检索具有给定ID的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中检索文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td> <p>输入要检索的文件的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定的父文件夹内创建一个文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[！UICONTROL连接]</strong> </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL驱动器ID]</strong> </td> 
   <td> <p>选择要创建新文件夹的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL文件夹]</strong> </td> 
   <td> <p>选择要在其中创建新文件夹的文件夹。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL文件夹名称]</strong> </td> 
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
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL驱动器ID]</td> 
   <td> <p>选择要从中删除文件的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹ID]</td> 
   <td> <p>输入或映射要删除的文件夹的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取共享链接]

此模块会检索可共享的链接，以授予对指定文件的访问权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL驱动器ID]</td> 
   <td> <p>选择要将文件上传到的驱动器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Enter]</td> 
   <td> <p>选择是要使用“文件ID”还是“文件”路径选择文件。 在显示的字段中输入文件ID或路径。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL权限类型]</p> </td> 
   <td> <p>选择您希望接收链接的人员具有读/写权限还是只读权限。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL作用域]</td> 
   <td> <p> 选择您希望拥有链接的任何人都可以访问文件，还是希望只有贵组织的成员才能访问文件。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
