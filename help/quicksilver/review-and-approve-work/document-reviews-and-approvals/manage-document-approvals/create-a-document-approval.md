---
product-area: documents
navigation-topic: approvals
title: 创建文档审批工作流
description: 您可以在Adobe Workfront中请求其他用户批准文档。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 315ec33fdcb79c6ba739a40de92be92e829a96d5
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 2%

---

# 创建文档审批工作流

{{highlighted-preview}}

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

## 从生产的旧文档区域中的“摘要”面板创建审批工作流

如果您的组织位于Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的更多信息，请参阅[Adobe云存储与旧版Workfront存储之间的区别](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

要创建审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 在版本下拉列表中选择要创建批准的文档版本。 默认情况下会选择最新版本。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。


1. 填写以下详细信息：

   <table>
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
   <td><strong>截止日期（可选）</strong></td>
   <td>设置审批的截止日期。 用户和团队将在指定到期日期之前的72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   </table>

1. （可选）根据需要重复上一步添加其他阶段。

   >[!NOTE]
   >
   >如果添加多个阶段，则审批工作流会按阶段列出的顺序继续执行。 完成所有必需的决策后，将开始下一阶段，并锁定上一阶段。

   ![文档详细信息](assets/new-stage.png)


<div class="preview">

## 在预览的旧文档区域的“摘要”面板中创建审批工作流

如果您的组织位于Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的更多信息，请参阅[Adobe云存储与旧版Workfront存储之间的区别](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

要创建审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击所需的文档，该文档的“文档摘要”面板将打开。

1. 在版本下拉菜单中选择要为其创建审批的文档版本。 默认情况下会选择最新版本。

1. 向下滚动到&#x200B;**审批**&#x200B;部分，然后单击&#x200B;**创建工作流**。

1. 填写以下详细信息：

   <table>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>添加阶段名称。 您可以将名称更改为更具描述性的名称，如<em>初始审阅</em>或<em>最终批准</em>。</td>
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
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。
   <p>添加第二个阶段时，默认情况下会选中<strong>在所有阶段上显示此消息</strong>。 将其保留为选中状态，以便在每个阶段中使用相同的消息。 若要对每个阶段使用不同的消息，请清除<strong>在所有阶段上显示此消息</strong>，然后根据需要在每个阶段的<strong>添加自定义消息</strong>文本框中键入特定于阶段的消息。</p></td>
   </tr>
   </table>

1. （可选）根据需要重复上一步添加其他阶段。

   >[!NOTE]
   >
   >* 如果添加多个阶段，则审批工作流会按阶段列出的顺序继续执行。 完成所有必需的决策后，将开始下一阶段，并锁定上一阶段。
   >* 如果在创建审批工作流后编辑自定义消息，则会向所有现有参与者发送更新的电子邮件通知。 如果稍后添加参与者，则自定义消息将包含在其电子邮件通知中。

   ![将自定义消息添加到阶段](assets/add-custom-message.jpeg)

</div>


## 从生产中新建文档区域的摘要面板创建审批工作流

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

要创建审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击文档，然后单击页面右侧的&#x200B;**审批**&#x200B;图标。

   ![在文档摘要中添加批准者](assets/approvals-icon-new.png)

1. 单击&#x200B;**创建工作流**，然后填写以下详细信息：

   <table>
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
   <td><strong>截止日期（可选）</strong></td>
   <td>设置审批的截止日期。 用户和团队将在指定到期日期之前的72小时（即24小时）通过电子邮件接收通知。</td>
   </tr>
   </table>

1. （可选）根据需要重复上一步添加其他阶段。

   >[!NOTE]
   >
   >如果添加多个阶段，则审批工作流会按阶段列出的顺序继续执行。 完成所有必需的决策后，将开始下一阶段，并锁定上一阶段。

   ![文档详细信息](assets/new-stage.png)


<div class="preview">

## 在预览中新建文档区域的“摘要”面板中创建审批工作流

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

要创建审批工作流，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。

1. 单击文档，然后单击页面右侧的&#x200B;**审批**&#x200B;图标。

   ![在文档摘要中添加批准者](assets/approvals-icon-new.png)

1. 单击&#x200B;**创建工作流**，然后填写以下详细信息：

   <table>
   <tr>
   <td><strong>阶段名称</strong></td>
   <td>添加阶段名称。 您可以将名称更改为更具描述性的名称，如<em>初始审阅</em>或<em>最终批准</em>。</td>
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
   <td>在<strong>添加自定义消息</strong>文本框中键入消息。该消息会显示在批准电子邮件通知和Workfront的“批准”选项卡中。
   <p>添加第二个阶段时，默认情况下会选中<strong>在所有阶段上显示此消息</strong>。 将其保留为选中状态，以便在每个阶段中使用相同的消息。 若要对每个阶段使用不同的消息，请清除<strong>在所有阶段上显示此消息</strong>，然后在每个阶段的<strong>添加自定义消息</strong>文本框中键入特定于阶段的消息。</p></td>
   </tr>
   </table>

1. （可选）根据需要重复上一步添加其他阶段。

   >[!NOTE]
   >
   >* 如果添加多个阶段，则审批工作流会按阶段列出的顺序继续执行。 完成所有必需的决策后，将开始下一阶段，并锁定上一阶段。
   >* 如果在创建审批工作流后编辑自定义消息，则会向所有现有参与者发送更新的电子邮件通知。 如果稍后添加参与者，则自定义消息将包含在其电子邮件通知中。

   ![将自定义消息添加到阶段](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
