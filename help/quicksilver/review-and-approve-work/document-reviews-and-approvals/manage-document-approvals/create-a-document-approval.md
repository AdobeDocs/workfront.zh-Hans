---
product-area: documents
navigation-topic: approvals
title: 创建文档审批工作流
description: 您可以在Adobe Workfront中请求其他用户批准文档。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 2231
ht-degree: 1%

---

# 创建文档审批工作流

您可以在Adobe Workfront中请求其他用户或团队批准文档，或请求他们审核文档而无需批准。

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
   <td> <p>使用旧版Workfront存储管理审批的任何Workfront软件包</p>
<p>任何使用Adobe云存储管理审批的工作流包</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td>  
   <td>
   <p>参与者或更高版本</p>
   <p>审核或更高</p>
   <p>如果您使用的是Frame.io集成，则必须具有Standard许可证才能创建批准工作流。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的项目、任务、问题、模板、项目组合、程序、报告、功能板和日历、文档</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理与请求访问或审批关联的对象的访问权限 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--

## Create an approval workflow in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

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

   ![Document details](assets/new-stage.png)

-->

## 在旧文档区域创建审批工作流

如果您的组织位于Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的更多信息，请参阅[Adobe云存储与旧版Workfront存储之间的区别](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

### 创建基本审批工作流

要创建单阶段审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 在版本下拉菜单中选择要为其创建审批的文档版本。 默认情况下会选择最新版本。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 填写以下详细信息：

   <table>
   <tr>
   <td><strong>使用审批模板（可选）</strong></td>
   <td>从下拉菜单中选择模板。 如果模板具有一个路径和一个阶段，则它适用于基本模式。 如果模板具有多个阶段或多个路径，则该对话框会自动切换到“高级”模式，并且在“基本”模式下输入的任何输入都将被模板的内容替换。</td>
   </tr>
   <tr>
   <td><strong>添加姓名或电子邮件</strong></td>
   <td>开始键入要作为审批者或审阅者添加的用户或团队名称。 如果您只有审阅人，则系统会通知他们并可以选择完成审阅，但无需或做出任何决定。</td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>设置审批的截止日期。 用户和团队将在指定到期日期之前的72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。
   <p>注意：如果在创建审批工作流后编辑自定义消息，则会向所有现有参与者发送更新的电子邮件通知。 如果稍后添加参与者，则自定义消息将包含在其电子邮件通知中。</p>
   </td>
   </tr>
   </table>

1. 单击&#x200B;**请求审批**。

   ![在基本模式下请求审批](assets/request-approval-basic.jpeg)

### 创建高级审批工作流

高级模式支持多个阶段以及并行路径。 每个路径都独立运行，并包含一个或多个顺序阶段。 当阶段中所有必需的决策都完成时，该路径中的下一阶段将开始，前一阶段将被锁定，新阶段的审阅人和批准者将收到电子邮件通知。

“需要工作”决策会停止其所在的路径，但不会影响其他路径上的审批工作流。 您最多可以配置30条路径，共100个阶段。

要创建高级审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 在版本下拉菜单中选择要为其创建审批的文档版本。 默认情况下会选择最新版本。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。

1. 在&#x200B;**请求审批**&#x200B;对话框的右上角，单击&#x200B;**转到高级**。 您在基本模式下输入的任何输入都将被保留，并应用于&#x200B;**路径1**，**阶段1**。

   >[!TIP]
   >
   >创建审批时，单击右上方的&#x200B;**转到“基本”**，可返回到“基本”模式。 单击&#x200B;**请求审批**&#x200B;后，**转到基本**&#x200B;选项不再可用。

1. 填写路径1的第1阶段的详细信息：

   <table>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>默认情况下，阶段名为<em>阶段1</em>、<em>阶段2</em>，依此类推。 将阶段重命名为更具描述性的状态，如<em>初始审阅</em>或<em>最终批准</em>。</td>
   </tr>
   <tr>
   <td><strong>添加姓名或电子邮件</strong></td>
   <td>开始键入要作为审批者或审阅者添加的用户或团队名称。 如果您只有审阅人，则系统会通知他们并可以选择完成审阅，但无需或做出任何决定。<p>注意：对于同一资源，一次只能将一个打开阶段分配给查看者或审批者。 如果同时打开多个并行阶段，则无法将同一人员添加到多个阶段。</p></td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>每个路径的第一阶段都支持绝对到期日期。 路径中的每个后续阶段都支持相对到期日期，即从该阶段打开后的天数。 用户和团队将在截止日期前72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。<p>添加第二个阶段时，默认情况下会选中<strong>在所有阶段上显示此消息</strong>。 将其保留为选中状态，以便在每个阶段中使用相同的消息。 若要对每个阶段使用不同的消息，请清除<strong>在所有阶段上显示此消息</strong>，然后在每个阶段的<strong>添加自定义消息</strong>文本框中键入特定于阶段的消息。</p></td>
   </tr>
   </table>

1. （可选）单击&#x200B;**添加阶段**&#x200B;以向路径中添加另一个阶段。 路径中的阶段将按其列出的顺序依次运行。 您可以对路径中的阶段重新排序，但无法将阶段从一个路径移动到另一个路径。 每个路径可以有不同的阶段数。

1. （可选）在&#x200B;**并行路径**&#x200B;下，单击&#x200B;**添加路径**&#x200B;以添加其他路径。 新路径从一个空阶段开始，成为选定的路径。 要重命名路径，请将鼠标悬停在路径标签上，单击铅笔图标，然后键入新名称。

1. （可选）要删除路径，请将鼠标悬停在路径标签上并单击垃圾桶图标。 无法删除&#x200B;**路径1**，也无法对路径重新排序。 仅当路径中没有已锁定或已完成的阶段时，才能删除其他路径。

   ![具有并行路径的高级模式](assets/request-approval-parallel-paths.jpeg)

1. （可选）要清除所有路径和阶段并重新开始，请单击右上方的&#x200B;**重置**。

1. 单击&#x200B;**请求审批**。


<!--

## Create an approval workflow in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

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

   ![Document details](assets/new-stage.png)
   
-->

## 在新建文档区域创建审批工作流

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

默认情况下，**请求审批**&#x200B;对话框以&#x200B;**基本**&#x200B;模式打开。 基本模式是一个包含一组批准者或审阅者的阶段。 切换到&#x200B;**高级**&#x200B;模式以配置多阶段审批或并行路径。

### 创建基本审批工作流

要创建单阶段审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击文档，然后单击页面右侧的&#x200B;**审批**&#x200B;图标。

   ![在文档摘要中添加批准者](assets/approvals-icon-new.png)

1. 单击&#x200B;**创建工作流**。 **请求审批**&#x200B;对话框在基本模式下打开。

1. 填写以下详细信息：

   <table>
   <tr>
   <td><strong>使用审批模板（可选）</strong></td>
   <td>默认情况下，“模板”字段处于折叠状态。 单击该字段以将其展开，然后从下拉菜单中选择一个模板。 如果模板具有一个路径和一个阶段，则它适用于基本模式。 如果模板具有多个阶段或多个路径，则该对话框会自动切换到“高级”模式，并且在“基本”模式下输入的任何输入都将被模板的内容替换。</td>
   </tr>
   <tr>
   <td><strong>添加姓名或电子邮件</strong></td>
   <td>开始键入要作为审批者或审阅者添加的用户或团队名称。 如果您只有审阅人，则系统会通知他们并可以选择完成审阅，但无需或做出任何决定。</td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>设置审批的截止日期。 用户和团队将在指定到期日期之前的72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。</td>
   </tr>
   </table>

1. 单击&#x200B;**请求审批**。

   ![在基本模式下请求审批](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* 每次都在“基本”模式下打开&#x200B;**请求审批**&#x200B;对话框，这与您之前的会话无关。
>* 如果在创建审批工作流后编辑自定义消息，则会向所有现有参与者发送更新的电子邮件通知。 如果稍后添加参与者，则自定义消息将包含在其电子邮件通知中。
>* 保存审批后，无法将其切换回“基本”模式。 您可以将正在进行的审批从基本切换到高级，只要未锁定或未完成审批即可。

### 创建高级审批工作流

高级模式支持并行路径。 每个路径都独立运行，并包含一个或多个顺序阶段。 当阶段中所有必需的决策都完成时，该路径中的下一阶段将开始，前一阶段将被锁定，新阶段的审阅人和批准者将收到电子邮件通知。

“需要工作”决策会停止其所在的路径，但不会影响其他路径上的审批工作流。 您最多可以配置30条路径，共100个阶段。

要创建高级审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击文档，然后单击页面右侧的&#x200B;**审批**&#x200B;图标。

   ![在文档摘要中添加批准者](assets/approvals-icon-new.png)

1. 单击&#x200B;**创建工作流**。

1. 在&#x200B;**请求审批**&#x200B;对话框的右上角，单击&#x200B;**转到高级**。 您在基本模式下输入的任何输入都将被保留，并应用于&#x200B;**路径1**，**阶段1**。

   >[!TIP]
   >
   >创建审批时，单击右上方的&#x200B;**转到“基本”**，可返回到“基本”模式。 单击&#x200B;**请求审批**&#x200B;后，**转到基本**&#x200B;选项不再可用。

1. 填写路径1的第1阶段的详细信息：

   <table>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>默认情况下，阶段名为<em>阶段1</em>、<em>阶段2</em>，依此类推。 将阶段重命名为更具描述性的状态，如<em>初始审阅</em>或<em>最终批准</em>。</td>
   </tr>
   <tr>
   <td><strong>添加姓名或电子邮件</strong></td>
   <td>开始键入要作为审批者或审阅者添加的用户或团队名称。 如果您只有审阅人，则系统会通知他们并可以选择完成审阅，但无需或做出任何决定。<p>注意：对于同一资源，一次只能将一个打开阶段分配给查看者或审批者。 如果同时打开多个并行阶段，则无法将同一人员添加到多个阶段。</p></td>
   </tr>
   <tr>
   <td><strong>只需一个决策（可选）</strong></td>
   <td>第一个做出决策的人将完成阶段。</td>
   </tr>
   <tr>
   <td><strong>到期日期（可选）</strong></td>
   <td>每个路径的第一阶段都支持绝对到期日期。 路径中的每个后续阶段都支持相对到期日期，即从该阶段打开后的天数。 用户和团队将在截止日期前72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   <tr>
   <td><strong>添加自定义消息（可选）</strong></td>
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。 该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。<p>添加第二个阶段时，默认情况下会选中<strong>在所有阶段上显示此消息</strong>。 将其保留为选中状态，以便在每个阶段中使用相同的消息。 若要对每个阶段使用不同的消息，请清除<strong>在所有阶段上显示此消息</strong>，然后在每个阶段的<strong>添加自定义消息</strong>文本框中键入特定于阶段的消息。</p></td>
   </tr>
   </table>

1. （可选）单击&#x200B;**添加阶段**&#x200B;以向路径中添加另一个阶段。 路径中的阶段将按其列出的顺序依次运行。 您可以对路径中的阶段重新排序，但无法将阶段从一个路径移动到另一个路径。 每个路径可以有不同的阶段数。


1. （可选）在&#x200B;**并行路径**&#x200B;下，单击&#x200B;**添加路径**&#x200B;以添加其他路径。 新路径从一个空阶段开始，成为选定的路径。 要重命名路径，请将鼠标悬停在路径标签上，单击铅笔图标，然后键入新名称。

1. （可选）要删除路径，请将鼠标悬停在路径标签上并单击垃圾桶图标。 无法删除&#x200B;**路径1**，也无法对路径重新排序。 仅当路径中没有已锁定或已完成的阶段时，才能删除其他路径。

   ![具有并行路径的高级模式](assets/request-approval-advanced.jpeg)

1. （可选）要清除所有路径和阶段并重新开始，请单击右上方的&#x200B;**重置**。

1. 单击&#x200B;**请求审批**。

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->