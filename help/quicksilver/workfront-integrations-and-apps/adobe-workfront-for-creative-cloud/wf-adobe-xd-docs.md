---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 将XD画板作为文档上传到Workfront
description: 您可以将画板作为文档上传，以供快速审阅和审批，或只需将其存储在Adobe Workfront中。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 1%

---


# 将[!DNL XD]画板作为文档上载到[!DNL Workfront]

您可以将画板作为文档上传，以供快速审阅和审批，或仅将其存储在[!DNL Adobe Workfront]中。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">产品</td> 
   <td>除了[!DNL Workfront]许可证，您还必须具有[!DNL Adobe Creative Cloud]许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对[!UICONTROL 文档]的访问权限</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL 视图]对要上载文档的对象的访问权限或更高版本。</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

+++

## 先决条件

* 必须先安装[!DNL Adobe Workfront for XD]插件，然后才能将XD艺术展示板作为文档上传到Workfront。

有关说明，请参阅[安装 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md)。

## 添加新文档

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![菜单图标](assets/menu-350x440.png)

1. 转到要上载文档的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新建文件]**。
1. 选择要上载的画板。

   >[!TIP]
   >
   >要选择多个画板，请单击并将鼠标拖动到所需的画板上。
1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。
1. 从下拉菜单中选择&#x200B;**[!UICONTROL 资源类型]**：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL 导出格式]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>画板将作为PNG上载到[!DNL Workfront]中的工作项的[!UICONTROL 文档]选项卡。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>画板将作为JPG上载到[!DNL Workfront]中的工作项的[!UICONTROL 文档]选项卡。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>画板将作为SVG上载到[!DNL Workfront]中的工作项的[!UICONTROL Documents]选项卡。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>选择希望所选画板上载为<strong>单个PDF文件</strong>还是<strong>多个PDF文件</strong>。 画板将作为PDF上载到[!DNL Workfront]中的工作项的[!UICONTROL Documents]选项卡。</td>
     </tr>
    </tbody>
   </table>


1. 单击&#x200B;**[!UICONTROL 上传]**。\
   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。

## 添加新版本

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![菜单图标](assets/menu-350x440.png)

1. 转到要上载文档的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击要向其添加新版本的文档。
1. 单击插件底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 选择要上载的画板。

   >[!NOTE]
   >
   >如果要上传SVG、PNG或JPG的新版本，则只能上传一个画板。

1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

1. 从下拉菜单中选择&#x200B;**[!UICONTROL 资源类型]**：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">导出格式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>画板将作为PNG上载到[!DNL Workfront]中的工作项的[!UICONTROL 文档]选项卡。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>画板将作为JPG上载到[!DNL Workfront]中的工作项的[!UICONTROL Documents]选项卡。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>画板将作为SVG上载到[!DNL Workfront]中的工作项的[!UICONTROL Documents]选项卡。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>画板将作为PDF上载到[!DNL Workfront]中的工作项的[!UICONTROL Documents]选项卡。</p>
      <p><strong>注意</strong>：对于新文档版本，您只能上传一个画板。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 单击&#x200B;**[!UICONTROL 上传]**。\
   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。
