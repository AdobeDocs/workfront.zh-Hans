---
product-area: documents
navigation-topic: approvals
title: Create an approval workflow template for documents
description: You can create Approval Templates to streamline your approval process.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 8%

---

# Create an approval workflow template for documents

In the Workfront Setup area, users with a Standard license can create reusable Approval Templates. Once created, Approval Templates can be applied to assets in the Documents area of a project, task, or issue.

>[!IMPORTANT]
>
>本文内容介绍更新的文档审批功能，该功能仅适用于特定帐户。 有关标准审批流程的信息，请参阅[工作审批](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>使用旧版Workfront存储管理审批的任何Workfront软件包</p>
<p>使用Adobe企业存储管理审批的任意工作流包</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>规划</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++
ß

## Create an Approval Template

{{step-1-to-setup}}

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Click **New Template** on the right side of the page.

1. 填写以下详细信息：

   <table>
     <tr>
   <td><strong>模板名称</strong></td>
   <td>Add a template name. </td>
   </tr>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>添加阶段名称。 您可以将名称更改为更具描述性的名称，如<em>初始审阅</em>或<em>最终批准</em>。</td>
   </tr>
   <tr>
   <td><strong>添加姓名或电子邮件</strong></td>
   <td>开始键入要作为审批者或审阅者添加的用户或团队名称。 如果您只有审阅人，则系统会通知他们并可以选择完成审阅，但无需或做出任何决定。</td>
   </tr>
   <tr>
   <td><strong>需要一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期前的工作日</strong></td>
   <td>Choose how many workdays until the approval is due after a stage is activated.</td>
   </tr>
   </table>

1. （可选）根据需要重复上一步添加其他阶段。

   >[!NOTE]
   >
   >如果添加多个阶段，则审批工作流会按阶段列出的顺序继续执行。 完成所有必需的决策后，将开始下一阶段，并锁定上一阶段。

   ![文档详细信息](assets/new-stage.png)

1. 单击&#x200B;**保存**。

Once the template is created, it can be applied to documents in the Documents area of a project, task, or issue to begin the formal review and approval process in Workfront.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
