---
product-area: documents
navigation-topic: approvals
title: 上传新文档版本并请求审批
description: 您可以在Adobe Workfront中上传新文档版本并请求其他用户审批。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 2%

---

# 上传新文档版本并请求审批

如果文档在以前的审阅中被标记为“需要工作”，则您可以将新版本上传到原始文档并开始另一轮审批。 上传文档的新版本后，先前版本将被锁定。

如果新版本的文件名与先前版本的文件名不同，则Workfront显示具有新文件名的文档。

当向具有未完成审批的文档中添加新版本时，对先前版本的审批显示为“已撤回”。 先前的批准流程将关闭，即使一些参与者尚未做出决定。

如果删除了最新的文档版本，则以前的版本仍保持锁定状态。 如果需要编辑以前的版本，则必须手动解锁该版本。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>使用旧版Workfront存储管理审批的任何Workfront软件包</p>
<p>任何使用Adobe云存储管理审批的工作流包</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证</td> 
   <td> <p>请求或更高版本</p>
   <p>参与者或更高版本</p>
   <p>如果您使用的是Frame.io集成，则必须具有Standard许可证才能创建批准工作流。</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对与文档关联的对象的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

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



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## 使用拖放操作在旧文档区域中添加新版本

如果您的组织位于Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的更多信息，请参阅[Adobe云存储与旧版Workfront存储之间的区别](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

>[!NOTE]
>
>Internet Explorer无法执行拖放操作。

如果您需要对文档进行另一轮审核和批准，则可以在Workfront中创建新文档版本。 可添加先前的参与者、新参与者或两者的组合。 您可以在“文档详细信息”页面上查看有关先前版本和参与者的信息。

默认情况下，请求审批对话框在基本模式下打开，以进行单阶段审批。 切换到高级模式以配置多阶段审批或并行路径。

要添加新版本并请求审批，请执行以下操作：

1. 导航到Workfront中的文档。

1. 将新文件拖放到上一个文档上。 Workfront会自动创建新版本。

1. 文档上传完成后，选择文档以打开文档摘要面板。 版本号显示在面板顶部。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 配置审批工作流。 有关字段描述、高级模式切换和平行路径流，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 若要从以前的文档版本复制相同的审阅人和批准者，请单击&#x200B;**复制**。
1. 单击&#x200B;**请求审批**。

   审批工作流将启动，审批者会收到通知，告知需要对新文档版本进行审批。 以前的文档版本被锁定，并且以前版本上的任何未完成的批准都将被撤回。

## 使用拖放操作在新的“文档”区域中添加新版本

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

>[!NOTE]
>
>Internet Explorer无法执行拖放操作。

如果您需要对文档进行另一轮审核和批准，则可以在Workfront中创建新文档版本。 您可以将审批工作流添加到文档的新版本。

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

默认情况下，请求审批对话框在基本模式下打开，以进行单阶段审批。 切换到高级模式以配置多阶段审批或并行路径。

要添加新版本并请求审批，请执行以下操作：

1. 导航到Workfront中的文档。

1. 将新文件拖放到上一个文档上。 Workfront会自动创建新版本。

1. 文档上传完成后，选择文档以打开“摘要”面板。 默认情况下，将选择文档的最新版本。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 配置审批工作流。 有关字段描述、高级模式切换和平行路径流，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 若要从以前的文档版本复制相同的审阅人和批准者，请单击&#x200B;**复制**。
1. 单击&#x200B;**请求审批**。

   审批工作流将启动，审批者会收到通知，告知需要对新文档版本进行审批。 以前的文档版本被锁定，并且以前版本上的任何未完成的批准都将被撤回。
