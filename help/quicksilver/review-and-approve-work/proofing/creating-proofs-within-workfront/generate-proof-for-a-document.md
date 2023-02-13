---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为文档创建校样
description: 您可以在将文档上传到Workfront时为其生成校样。
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 为文档创建校样

您可以在将文档上传到Workfront时为其生成校样。

您还可以为已在Adobe Workfront中上传的文档或已在Workfront中生成校样的新版本生成校样。

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 上传文档并创建校样

1. 转到要创建新校样的项目、任务或问题。
1. 单击 **文档** 选项卡。
1. 单击文档 ![](assets/document-icon.png) 中。
1. 单击 **新增**，然后单击 **校样** 中。

   >[!TIP]
   >
   >您可以启用 **上传文档时自动生成校样** 在用户配置文件中设置以自动执行此过程。 有关更多信息，请参阅 [配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. 在 **新校样** 页面，您可以

   * [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 上传文档并创建校样的新版本

1. 转到要创建现有校样新版本的项目、任务或问题。
1. 单击 **文档** 选项卡。
1. 选择要添加新版本的文档。
1. 单击 **新增** > **版本** > **校样**.
1. 在 **新校样版本** 页面，您可以

   * [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 使用拖放为新版本生成简单的校样

您可以从文件系统（如桌面）中拖放文档，以创建新校样或现有校样的新版本。 校样包含以下设置，具体取决于您是创建新校样还是创建新版本：

* **新校样：** 创建一个仅与您共享的简单校样。 创建校样后，您可以修改共享设置，如 [编辑校样设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **现有校样的新版本：** 使用与先前版本相同的校样设置创建新版本。

要使用拖放功能生成新校样或新校样版本，请执行以下操作：

1. 确保将校样配置为自动生成，如中所述。
1. 继续  [从文件系统将文档添加到Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)，其中说明了添加文档的拖放方法。 

## 为现有文档创建校样

1. 转到要校样的项目、任务或问题，然后单击 **文档** 中。
1. 将鼠标悬停在文档上，然后单击 **创建校样** 链接。

   >[!NOTE]
   >
   >如果 **上传文档时自动生成校样** 系统会在您的用户配置文件中启用，从而自动创建一个简单的校样。

1. 选择以下选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">简单校样</td> 
      <td>此选项会创建一个未附加工作流的校样，并应用默认校样设置。 您可以更新默认的校样设置，或在创建校样后添加工作流。 有关校样设置的更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校样设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高级校样</td> 
      <td> <p>此选项允许您配置基本或高级工作流，并修改所创建校样的校样设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校样</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动工作流创建高级校样</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
