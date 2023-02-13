---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 将XD画板作为文档上传到Workfront
description: 您可以将画板上传为文档，以便快速审核和批准，或者只是存储在Adobe Workfront中。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# 上传 [!DNL XD] 将画板作为文档 [!DNL Workfront]

您可以将画板上传为文档，以便快速审核和批准，或者只是存储在中 [!DNL Adobe Workfront].

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td>您必须具有 [!DNL Adobe Creative Cloud] 除 [!DNL Workfront] 许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对[!UICONTROL Documents]的访问</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL视图]对要上载文档的对象具有访问权限或更高权限。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

* 您必须安装 [!DNL Adobe Workfront for XD] 插件，然后您才能将XD画板作为文档上传到Workfront。

有关说明，请参阅 [安装 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 添加新文档

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/menu-350x440.png)

1. 转到要上传文档的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 中。

1. 单击 **[!UICONTROL 新建文件]** 在插件底部附近。
1. 选择要上传的画板。

   >[!TIP]
   >
   >要选择多个画板，请单击鼠标并将其拖动到所需的画板上。
1. （可选）在 **[!UICONTROL 更新]** 的上界。
1. 选择 **[!UICONTROL 资产类型]** 从下拉菜单中：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL导出格式]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>画板将作为PNG上传到 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>画板将作为JPG上传到 [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>画板将作为SVG上传到 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>选择是否希望将选定的画板作为 <strong>单个PDF文件</strong> 或 <strong>多个PDF文件</strong>. 画板作为PDF上传到 [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. 单击 **[!UICONTROL 上传]**.\
   文档将显示在 [!UICONTROL 文档] 区域。

## 添加新版本

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/menu-350x440.png)

1. 转到要上传文档的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png)中。

1. 单击要向其添加新版本的文档。
1. 单击 **[!UICONTROL 新版本]** 在插件底部附近。
1. 选择要上传的画板。

   >[!NOTE]
   >
   >如果要上传新版本的SVG、PNG或JPG，则只能上传一个画板。

1. （可选）在 **[!UICONTROL 更新]** 的上界。

1. 选择 **[!UICONTROL 资产类型]** 从下拉菜单中：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">导出格式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>画板将作为PNG上传到中工作项的[!UICONTROL Documents]选项卡 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>画板将作为JPG上载到 [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>画板将作为SVG上传到 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>画板将作为PDF上传到 [!DNL Workfront].</p>
      <p><strong>注意</strong>:对于新文档版本，只能上传一个画板。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 单击 **[!UICONTROL 上传]**.\
   文档将显示在 [!UICONTROL 文档] 区域。
