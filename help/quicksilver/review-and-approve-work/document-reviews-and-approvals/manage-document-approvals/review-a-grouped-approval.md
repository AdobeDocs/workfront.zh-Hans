---
product-area: documents
navigation-topic: approvals
title: 审核分组的审批
description: 您可以从主页或Frame.io查看器中的“我的审批”小组件查看分组审批中的所有文档并进行决策。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: ccb3d004feca5373473a872b101a7acff11de77f
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 3%
---

# 审核分组的审批

<span class="preview">此页面上的信息在“预览沙盒”环境中不可用，因为Frame.io集成在该环境中不可用。 此功能将于2026年10月22日在生产环境中可用。</span>

当您被分配到分组审批时，该分组中的所有文档都会显示在一起，以便您能够针对每个文档做出决策。 您可以一次批准或请求对每个文档进行更改，或单独对每个文档做出决定。

如果一个或多个文档在多阶段的分组审批中被标记为&#x200B;**需要工作**，则在组中的所有文档都有批准决策之前，该组无法进入下一阶段。 有关详细信息，请参阅[在多阶段分组审批中解决单个文档的“需要工作”决策](#resolve-a-needs-work-decision-on-a-single-document-in-a-multi-stage-grouped-approval)。



>[!IMPORTANT]
>
>如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 分组的审批仅在新的“文档”区域可用。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 包</td>
   <td> <p>任何使用Adobe云存储管理审批的工作流包</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront许可证</td>
   <td>
   <p>参与者或更高版本</p>
   <p>审核或更高</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">访问级别配置</td>
   <td> <p>查看或更高权限访问与审批关联的对象</p></td>
  </tr>
  <tr>
   <td role="rowheader">对象权限</td>
   <td> <p>查看与审批关联的对象的权限或更高的权限</p></td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在主页中查看我的审批小组件的分组审批

主页中的“我的审批”小组件对文档进行单个审批分组，以便您能够一起处理所有文档。

>[!NOTE]
>
>您可能需要将我的审批构件添加到您的主页。 有关详细信息，请参阅[添加、编辑或删除主页中的小组件](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)。

1. 单击Adobe Workfront左上角的&#x200B;**主页**&#x200B;图标，然后找到&#x200B;**我的审批**&#x200B;构件。

1. 打开分组审批。 组中的所有文档一起列出，组内的项目数列在顶部。

1. 使用以下方式之一做出决策：

   * **将所有文档标记为已批准**：同时记录对组中每个文档的已批准决策。
   * **标记所有需要工作**：同时记录对组中每个文档的需要工作决定。
   * **做出决定**：对单个文档做出单个决定。 对要分别决定的每个文档重复此操作。


   ![我的审批小组件分组审批](assets/my-approvals-group.png)

## 在Frame.io查看器中查看分组的批准

在Frame.io查看器中，该组中的所有文档一起显示，以便您快速决定每个文档，或打开文档进行详细查看。

1. 转到审阅电子邮件通知并单击&#x200B;**转到审阅**，或从主页中的&#x200B;**我的审批**&#x200B;构件打开分组的审批。

1. 执行下列操作之一：

   * 直接从组页面快速决策每个文档，而无需打开它。
   * 单击文档以将其打开，添加注释或标注，然后使用箭头移动到组中的下一个文档。 文档计数器（例如，2 **的** 1）显示您在组中的位置。

   有关在Frame.io查看器中添加注释和标记的详细信息，请参阅[使用Frame.io查看器进行审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)。

1. 为每个文档选择一个决策：

   * **已批准**：文档不需要更改，已可供使用。
   * **需要工作**：文档需要更改，且未准备就绪。

   有关决策的详细信息，请参阅[文档决策状态概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)。

   ![frame.io查看器分组审批](assets/frame-group-approval.png)

## 其他资源

本文介绍有关审阅一组文档的信息。 有关对单个文档做出决策、添加标记等的信息，请参阅

* [在Workfront中批准文档](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/approve-a-document.md)
* [在Workfront中查看文档](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md)
* [使用Frame.io查看器审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)