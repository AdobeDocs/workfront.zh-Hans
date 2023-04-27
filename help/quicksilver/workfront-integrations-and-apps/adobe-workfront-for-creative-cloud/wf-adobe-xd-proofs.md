---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: 将XD画板作为校样上传到Workfront
description: 您可以将画板作为校样直接上传到Adobe Workfront，以便进行彻底的审核和批准。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d0afdfc7be9177f6ff45dcc247253faa9dc57967
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 1%

---

# 上传 [!DNL XD] 将画板作为校样 [!DNL Workfront]

您可以将画板作为校样直接上传到 [!DNL Adobe Workfront] 进行彻底的审查和批准。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>当前计划：[!UICONTROL Pro]或更高版本</p> <p>或</p> <p>旧版计划：[!UICONTROL Premium]</p> <p>有关使用不同计划校样访问权限的更多信息，请参阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>当前计划：[!UICONTROL Work]或[!UICONTROL Proof]</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须具有 [!DNL Adobe Creative Cloud] 除 [!DNL Workfront] 许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对[!UICONTROL Documents]的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的 [!DNL Workfront] 或 [!DNL Workfront Proof] 管理员。

## 先决条件

* 您必须安装 [!DNL Adobe Workfront for XD] 插件，然后才能在 [!DNL Adobe XD].

   有关说明，请参阅 [安装 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 上传静态校样

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/menu-350x440.png)

1. 转到要上传静态校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 中。

1. 单击 **[!UICONTROL 新建文件]** 在插件底部附近。
1. 选择要上传的画板。

   >[!TIP]
   >
   >要选择多个画板，请单击鼠标并将其拖动到所需的画板上。

1. 启用 **[!UICONTROL 创建校样]**.

1. 命名校样。

1. 选择所需的校样批准类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的审批流程是临时的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）添加 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动审批流程由管理员预先构建，并包括特定的审阅者和阶段。 有关更多信息，请参阅 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （可选）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. 从 **[!UICONTROL 资产类型]** 下拉菜单。


1. （可选）如果您选择“PDF”作为资产类型，并选择了多个画板，请选择是否要将画板导出为 **[!UICONTROL 单个PDF文件]s** 或 **M[!UICONTROL 多个PDF文件]**.

1. （可选）将PDF命名为。

   ![](assets/pdf-options.png)

1. 单击 **[!UICONTROL 上传]**.\
   文档将显示在 [!UICONTROL 文档] 区域。

## 上传交互式校样 {#upload-an-interactive-proof}

您可以使用 [!DNL Workfront for Adobe] 插件。 这是一个两步流程。 首先，您需要创建一个交互式链接，然后，您需要将校样上传到工作项。

### 为画板创建交互式链接  {#create-an-interactive-link-for-your-art-board}

1. 打开画板，然后单击 **[!UICONTROL 共享]** 在屏幕的左上角区域。
1. 指定链接设置：

   1. 命名链接。
   1. 选择视图设置。
   1. 在 **[!UICONTROL 链接访问]** 部分，确保 **[!UICONTROL 具有此链接的任何人]** 中。

      必须启用此类型的访问才能生成交互式校样。

   1. 单击 **[!UICONTROL 创建链接]**.

1. 单击返回 **[!UICONTROL 设计]** 在屏幕的左上角区域。 继续 [上传交互式校样](#upload-an-interactive-proof) 部分。

   >[!NOTE]
   >
   >您可能需要在屏幕左下角重新打开插件面板。

### 上传交互式校样

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/menu-350x440.png)

1. 转到要上传交互式校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 中。

1. 单击 **[!UICONTROL 新建文件]** 在插件底部附近。
1. 启用 **[!UICONTROL 创建校样]**.

1. 选择所需的校样批准类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的审批流程是临时的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）添加 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动审批流程由管理员预先构建，并包括特定的审阅者和阶段。 有关更多信息，请参阅 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （可选）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. 在 **[!UICONTROL 资产类型]** 下拉菜单中，选择您刚刚在 **共享链接** 选项卡。 有关更多信息，请参阅 [为画板创建交互式链接](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. 单击 **[!UICONTROL 上传]**.

   文档将显示在 [!UICONTROL 文档] 区域。

   >[!IMPORTANT]
   >
   >用户必须具有 [!UICONTROL 桌面校对查看器] 以审阅和批准交互式校样。 有关详细信息，请参阅[安装[!UICONTROL 桌面校样查看器]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)。

## 上传新校样版本

您可以上传校样的新版本。 该插件会记住在以前版本中设置的校对工作流，但您可以根据需要更改此工作流。

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/menu-350x440.png)

1. 转到将文档上传到所需的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png)中。

1. 单击 **[!UICONTROL 新版本]** 在插件底部附近。
1. 启用 **[!UICONTROL 创建校样]**.
1. 选择要上传的画板。

   >[!NOTE]
   >
   >如果要上传.svg、.png或.jpg的新版本，则只能上传一个画板。

1. 选择所需的校样批准类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的审批流程是临时的，可以根据需要包括不同的审阅人： </p> 
       <ul> 
        <li> <p>（可选）添加 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>自动审批流程由管理员预先构建，并包括特定的审阅者和阶段。 有关更多信息，请参阅 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</p> 
       <ul> 
        <li> <p>从下拉菜单中选择一个[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. 从 **[!UICONTROL 资产类型]** 下拉菜单。

   ![](assets/create-a-proof-xd-350x202.png)

1. （可选）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. （可选）如果您选择“PDF”作为资产类型，并选择了多个画板，请选择是否要将画板导出为 **[!UICONTROL 单个PDF文件]s** 或 **M[!UICONTROL 多个PDF文件]**.

1. （可选）将PDF命名为。

   ![](assets/pdf-options.png)

1. 单击 **[!UICONTROL 上传]**.\
   文档将显示在 [!UICONTROL 文档] 区域。
