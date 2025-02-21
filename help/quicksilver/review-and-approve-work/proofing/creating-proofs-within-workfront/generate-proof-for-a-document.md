---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为文档创建验证
description: 您可以在将文档上传到Workfront时为其生成验证。 您还可以为已在Adobe Workfront中上传的文档或已在Workfront中的新版本验证生成验证。
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# 为文档创建验证

<!-- Audited: 1/2024 -->

您可以在将文档上传到Workfront时为其生成验证。

您还可以为已在Adobe Workfront中上传的文档或已在Workfront中的新版本验证生成验证。

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> 
   <p>新建：任何 </p>
   <p>当前： Pro或更高版本</p> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新增：标准</p>
   <p>当前：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 上传文档并创建验证

1. 转到要创建新验证的项目、任务或问题。
1. 单击&#x200B;**文档**&#x200B;选项卡。
1. 单击左侧面板中的文档![文档图标](assets/document-icon.png)。
1. 单击“新增”****，然后在出现的菜单中单击“校对”****。

   >[!TIP]
   >
   >您可以启用上载用户配置文件中的文档时&#x200B;**自动生成验证**&#x200B;设置以自动执行此过程。 有关详细信息，请参阅[配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) 。

1. 在出现的&#x200B;**新校对**&#x200B;页面中，您可以

   * [使用基本工作流创建高级校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 上传文档并创建新版本的验证

1. 转到要创建新版本现有校对的项目、任务或问题。
1. 单击&#x200B;**文档**&#x200B;选项卡。
1. 选择要添加新版本的文档。
1. 单击&#x200B;**新增** > **版本** > **校对**。
1. 在出现的&#x200B;**新验证版本**&#x200B;页面中，您可以

   * [使用基本工作流创建高级校对](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 使用拖放操作为新版本生成简单校对

您可以从文件系统（如桌面）拖放文档以创建新验证或现有验证的新版本。 校对包含以下设置，具体取决于您是创建新校对还是新版本：

* **新校对：**&#x200B;创建仅与您共享的简单校对。 您可以在创建验证后修改共享设置，如[编辑验证设置](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)中所述。

* **现有校对的新版本：**&#x200B;使用与先前版本相同的校对设置创建一个新版本。

要使用拖放操作生成新验证或新验证版本，请执行以下操作：

1. 确保将校样配置为自动生成，如中所述。
1. 继续  [从您的文件系统](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)将文档添加到Adobe Workfront，这说明了添加文档的拖放方法。 

## 为现有文档创建验证

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;部分。
1. 将鼠标悬停在文档上，然后单击文档名称下方显示的&#x200B;**创建验证**&#x200B;链接。

   >[!NOTE]
   >
   >如果您在上传用户配置文件中启用了文档&#x200B;**时**&#x200B;自动生成验证，则系统会自动创建一个简单的验证。

1. 选择下列选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">简单校对</td> 
      <td>此选项创建一个未附加工作流的验证，并应用默认验证设置。 您可以更新默认验证设置，或在创建验证后添加工作流。 有关校对设置的详细信息，请参阅<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校对设置</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">高级校对</td> 
      <td> <p>利用此选项，可配置基本或高级工作流并修改所创建验证的验证设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校对</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动化工作流创建高级校对</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
