---
navigation-topic: get-started-with-workfront
title: 在优先级中上传文档并创建验证
description: 文档
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 63aa5e45-e51d-4049-a5d9-18dfaaa79647
source-git-commit: b886284eb44c2154987019655ff07cdeb0e1ae22
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# 在优先级中上传文档并创建验证

您可以在优先级中上传文档并创建验证。

优先级显示分配给您的工作项。 您看不到分配给您团队的工作项。

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
   <p>当前： Pro或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p><strong>上传文档</strong></p>
   <p>新：参与者</p>
   <p>当前：请求</p>
      <p><strong>创建验证</strong></p>
        <p>新增：标准</p>
     <p>当前：工作或计划</p>
   </td> 
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

## 将文档上传到工作项

您可以从工作列表或工作项详细信息页面将文档上载到工作项。

### 工作列表摘要面板


{{step1-to-priorities}}

1. 在工作列表中，将鼠标悬停在工作名称上，然后单击&#x200B;**摘要**&#x200B;图标![打开摘要图标](assets/summary-icon.png)。
1. 确保在摘要面板中的&#x200B;**任务**&#x200B;或&#x200B;**问题**&#x200B;选项卡上。
1. 单击&#x200B;**上载文件**&#x200B;图标![上载文件图标](assets/upload-file-icon.png)。
1. 拖放文件或按Cmd/Ctrl + V以从剪贴板粘贴
或
单击**添加文件**浏览文件或从Document Cloud提供程序导入文件。
   ![添加文件](assets/add-files.png)
1. （可选）添加评论。
1. （可选）添加更多文件。

   >[!NOTE]
   >
   >其他文件作为单独的文档上传。
1. 单击&#x200B;**上传**。

### 工作项详细信息

{{step1-to-priorities}}

1. 在工作列表中，单击工作项名称。
1. 单击屏幕顶部的&#x200B;**文档**&#x200B;选项卡。
1. 单击右上角的&#x200B;**上传文档**，然后选择&#x200B;**文档**。
1. 拖放文件或按Cmd/Ctrl + V以从剪贴板粘贴
或
单击**添加文件**浏览文件或从Document Cloud提供程序导入文件。
   ![添加文件](assets/add-files.png)
1. （可选）添加评论。
1. （可选）添加更多文件。

   >[!NOTE]
   >
   >其他文件作为单独的文档上传。
1. 单击&#x200B;**上传**。


## 创建简单或高级校对

您可以从工作列表或工作项详细信息页面的文档创建验证。

### 工作列表摘要面板


{{step1-to-priorities}}

1. 在工作列表中，将鼠标悬停在工作名称上，然后单击&#x200B;**摘要**&#x200B;图标![打开摘要图标](assets/summary-icon.png)。
1. 确保在摘要面板中的&#x200B;**任务**&#x200B;或&#x200B;**问题**&#x200B;选项卡上。
1. 单击右侧边栏中的&#x200B;**文档**&#x200B;图标![文档图标](assets/show-document-icon.png)。
1. 单击&#x200B;**上载文件**&#x200B;图标![上载文件图标](assets/upload-file-icon.png)，然后选择文件。

   >[!NOTE]
   >
   >在创建验证之前，必须上传文档。


1. 上传文件后，在&#x200B;**文档**&#x200B;部分中选择文件。
1. 单击文件详细信息框右上角的&#x200B;**创建验证**。
1. 选择下列选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>简单校对</b></td> 
      <td>此选项创建一个未附加工作流的验证，并应用默认验证设置。 您可以更新默认验证设置，或在创建验证后添加工作流。 有关校对设置的详细信息，请参阅<a href="/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">编辑校对设置</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>高级校对</b></td> 
      <td> <p>利用此选项，可配置基本或高级工作流并修改所创建验证的验证设置。 有关更多信息，请参阅 </p> 
       <ul> 
        <li><p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流创建高级校对</a> </p> </li> 
        <li> <p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自动化工作流创建高级验证</a></p></li> 
       </ul>
        </td> 
     </tr> 
    </tbody> 
   </table>

### 工作项详细信息

{{step1-to-priorities}}

1. 在工作列表中，单击工作项名称。
1. 单击屏幕顶部的&#x200B;**文档**&#x200B;选项卡。
1. 单击右上角的&#x200B;**上传文档**，然后选择&#x200B;**验证**。
1. 按照中的说明创建验证
   [使用基本工作流创建高级校对](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   [使用自动化工作流创建高级校对](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

<!--

## Open a proof



## Edit a document

Edit name

Add description

manage

Add new version, open proof, edit, download, move, share, remove
-->

## 过滤和排序

您可以使用过滤器和排序选项组织文档。

### 筛选条件

您可以通过以下方式筛选文档

* 添加者
* 文件类型

### 排序

文档排序依据

* 添加日期
* 文件类型
