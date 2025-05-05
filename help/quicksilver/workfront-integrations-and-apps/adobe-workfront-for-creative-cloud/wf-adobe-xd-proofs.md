---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: 将XD画板作为验证上传到Workfront
description: 您可以将画板作为验证直接上传到Adobe Workfront以进行彻底审阅和批准。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---

# 将[!DNL XD]画板作为验证上载到[!DNL Workfront]

您可以将画板作为验证直接上传到[!DNL Adobe Workfront]以进行彻底审阅和批准。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>当前计划： [!UICONTROL Pro]或更高版本</p> <p>或</p> <p>旧版计划： [!UICONTROL Premium]</p> <p>有关验证不同规划的访问权限的更多信息，请参阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>当前计划： [!UICONTROL Work]或[!UICONTROL Proof]</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>除了[!DNL Workfront]许可证，您还必须具有[!DNL Adobe Creative Cloud]许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对[!UICONTROL 文档]的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的[!DNL Workfront]或[!DNL Workfront Proof]管理员。

+++

## 先决条件

* 必须先安装[!DNL Adobe Workfront for XD]插件，然后才能在[!DNL Adobe XD]中上传校样。

  有关说明，请参阅[安装 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md)。

## 上传静态校对

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![菜单图标](assets/menu-350x440.png)

1. 转到要上载静态校样的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新建文件]**。
1. 选择要上载的画板。

   >[!TIP]
   >
   >* 画板将按其选定顺序出现在验证中。 第一个选定的画板将是验证中的第一页，依此类推。
   >* 要快速选择多个画板，请单击并将鼠标拖动到所需的画板上。 这不允许您控制验证中画板的顺序。

1. 启用&#x200B;**[!UICONTROL 创建验证]**。

1. 为验证命名。

1. 选择所需的验证审批类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本审批流程是临时性的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）将<strong>审批者</strong>添加到框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动批准流程由管理员预先构建，并包括特定的审阅人和阶段。 有关详细信息，请参阅<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>。</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL 工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

   在XD中![校对审批](assets/proof-approvals-xd-350x396.png)

1. 从&#x200B;**[!UICONTROL 资源类型]**&#x200B;下拉菜单中选择导出格式。


1. （可选）如果您选择PDF作为资源类型并且选择了多个画板，请选择您要将画板导出为&#x200B;**[!UICONTROL 单个PDF文件]s**&#x200B;还是&#x200B;**M[!UICONTROL 多个PDF文件]**。

1. （可选）为PDF命名。

   ![PDF选项](assets/pdf-options.png)

1. 单击&#x200B;**[!UICONTROL 上传]**。\
   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。

## 上传交互式验证 {#upload-an-interactive-proof}

您可以使用[!DNL Workfront for Adobe]插件为画板创建交互式验证。 此过程分为两步。 首先，您需要创建交互式链接，然后您需要将验证上传到工作项。

### 为画板创建交互式链接  {#create-an-interactive-link-for-your-art-board}

1. 打开画板，然后单击屏幕左上角区域中的&#x200B;**[!UICONTROL 共享]**。
1. 指定链接设置：

   1. 命名链接。
   1. 选择视图设置。
   1. 在&#x200B;**[!UICONTROL 链接访问]**&#x200B;部分中，确保已选择具有此链接的&#x200B;**[!UICONTROL 任何人]**。

      必须启用此类型的访问才能生成交互式验证。

   1. 单击&#x200B;**[!UICONTROL 创建链接]**。

1. 在屏幕的左上角区域单击回到&#x200B;**[!UICONTROL 设计]**。 继续下面的上传[交互式校对](#upload-an-interactive-proof)部分。

   >[!NOTE]
   >
   >您可能需要重新打开屏幕左下角的插件面板。

### 上传交互式验证

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![菜单图标](assets/menu-350x440.png)

1. 转到要在其中上载交互式验证的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新建文件]**。
1. 启用&#x200B;**[!UICONTROL 创建验证]**。

1. 选择所需的验证审批类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本审批流程是临时性的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）将<strong>审批者</strong>添加到框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动批准流程由管理员预先构建，并包括特定的审阅人和阶段。 有关详细信息，请参阅<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>。</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL 工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

   在XD中![校对审批](assets/proof-approvals-xd-350x396.png)

1. 在&#x200B;**[!UICONTROL 资产类型]**&#x200B;下拉菜单中，在&#x200B;**共享链接**&#x200B;选项卡下选择您刚刚创建的链接。 有关详细信息，请参阅[为画板创建交互式链接](#create-an-interactive-link-for-your-artboard)。\
   ![在XD中共享链接](assets/shared-links-xd-350x870.png)

1. 单击&#x200B;**[!UICONTROL 上传]**。

   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。

   >[!IMPORTANT]
   >
   >用户必须有权访问[!UICONTROL 桌面验证查看器]，才能查看和批准交互式验证。 有关详细信息，请参阅[安装[!UICONTROL 桌面校对查看器]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)。

## 上传新验证版本

您可以上传新版本的验证。 该插件会记住在以前的版本上设置的验证工作流，但您可以根据需要更改此设置。

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![菜单图标](assets/menu-350x440.png)

1. 转到需要上载文档的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 启用&#x200B;**[!UICONTROL 创建验证]**。
1. 选择要上载的画板。

   >[!NOTE]
   >
   >如果要上传.svg、.png或.jpg的新版本，则只能上传一个画板。

1. 选择所需的验证审批类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本审批流程是临时性的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）将<strong>审批者</strong>添加到框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动批准流程由管理员预先构建，并包括特定的审阅人和阶段。 有关详细信息，请参阅<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>。</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL 工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. 从&#x200B;**[!UICONTROL 资源类型]**&#x200B;下拉菜单中选择导出格式。

   ![在XD中创建验证](assets/create-a-proof-xd-350x202.png)

1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

   在XD中![校对审批](assets/proof-approvals-xd-350x396.png)

1. （可选）如果您选择PDF作为资源类型并且选择了多个画板，请选择您要将画板导出为&#x200B;**[!UICONTROL 单个PDF文件]s**&#x200B;还是&#x200B;**M[!UICONTROL 多个PDF文件]**。

1. （可选）为PDF命名。

   PDF选项

1. 单击&#x200B;**[!UICONTROL 上传]**。\
   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。
