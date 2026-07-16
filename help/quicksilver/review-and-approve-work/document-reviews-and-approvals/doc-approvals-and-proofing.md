---
product-area: documents
navigation-topic: approvals
title: 将统一审批和验证结合使用
description: 您可以将统一审批与验证结合使用。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 0%

---

# 将统一审批和验证结合使用

Workfront中的统一审批引入了一组新功能，可帮助您审阅和审批文档。 您可以将“统一审批”工作流与现有验证查看者结合使用，向审核中的文档添加注释和标记。

将统一审批和验证结合使用时，工作流存在一些主要差异：

* 参与者显示在文档摘要中，而不是验证工作流中。

* 文档列表中的已发送、已打开、评论、决策(SOCD)详细信息是验证相关的，并不反映文档的决策状态。

## 上传文档并创建验证

1. 转到要添加新文档的项目、任务或问题。
1. 单击&#x200B;**文档**&#x200B;选项卡，然后单击&#x200B;**新增**下拉菜单。
或
将文档拖放到文档列表中。

   >[!NOTE]
   >
   >如果您在上传用户配置文件中启用了文档&#x200B;**时**&#x200B;自动生成验证，则系统会自动创建一个简单的验证。

1. 将鼠标悬停在文档上，然后单击文档名称下方显示的&#x200B;**创建验证**&#x200B;链接，并选择&#x200B;**简单验证**。 您需要创建一个简单的校对，因为您将不使用校对工作流进行审批。

被指定为参与者的用户可以使用校对查看器在文档中添加注释和标记。 继续下一部分，了解如何添加审阅参与者。

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 打开文档摘要并分配参与者

默认情况下，请求审批对话框在基本模式下打开，以进行单阶段审批。 切换到高级模式以配置多阶段审批或并行路径。

要分配参与者，请执行以下操作：

1. 选择您上传的文档，然后打开文档摘要。

   ![打开文档摘要](assets/open-doc-summary.png)

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 配置审批工作流。 有关字段描述、高级模式切换和平行路径流，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 单击&#x200B;**请求审批**。 将通过电子邮件通知参与者。

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 根据需要创建新版本

如果您需要另一轮审阅和批准，则可创建新验证版本并添加以前的参与者、新参与者或两者的组合。 您可以在文档摘要中查看有关先前版本和参与者的信息。

默认情况下，请求审批对话框在基本模式下打开，以进行单阶段审批。 切换到高级模式以配置多阶段审批或并行路径。

要添加新版本：

1. 将新文件拖放到Workfront中的上一个文档上。 Workfront会自动创建新版本。

1. 文档上传完成后，选择文档，然后单击&#x200B;**创建验证** > **简单验证**。

1. 再次选择文档，然后打开文档摘要。

   ![打开文档摘要](assets/open-doc-summary.png)

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 配置审批工作流。 有关字段描述、高级模式切换和平行路径流，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 单击&#x200B;**请求审批**。 将通过电子邮件通知参与者。

## 查看证明并做出决定

在所有分配的审批人选择“已批准”之前，文档不会移至“已批准”状态。

要审阅和批准文档，请执行以下操作：

1. 转到审阅电子邮件通知，然后单击&#x200B;**转到审阅**。

1. 进入Workfront后，单击&#x200B;**前往校对**。

1. 查看内容，并添加任何注释或标记。 有关如何使用验证查看器的更多信息，请参阅[在Adobe Workfront中查看验证：文章索引](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。

1. 选择以下决策之一：

   * **批准**：文档不需要更改，可以随时使用。
   * **审批并更改**：文档需要更改，并且一旦更改即可使用。 不需要额外审批。
   * **需要工作**：文档需要更改，并且尚未准备就绪。 完成指定的更改后，必须将文档作为新版本上传，并经过另一轮批准。 有关上载新版本的更多信息，请参阅本文中的[根据需要创建新版本](#create-a-new-version-as-needed)。

作出决定后，将通过电子邮件通知文档所有者。