---
product-area: projects
navigation-topic: approvals
title: 将新审批流程或现有审批流程与工作关联
description: 本文介绍了如何将审批流程与工作项关联。 有关将批准与校样或文档关联的信息，请参阅以下文章。
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# 将新审批流程或现有审批流程与工作关联

本文介绍了如何将审批流程与工作项关联。 有关将批准与校样或文档关联的信息，请参阅以下文章：

* [使用自动工作流创建高级校样](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [请求文档批准](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

您可以将全局或一次性审批流程与Adobe Workfront中的工作项目关联。 存在以下情形：

* 将现有的全局批准流程与项目、任务、问题、模板或模板任务相关联。 系统中的所有组都可以使用一些全局批准流程。 组级别的全局批准流程仅适用于某些组。
* 创建一次性审批流程，并将其与现有项目、任务、问题、模板或模板任务相关联。

>[!NOTE]
>
>本文使用术语“全局批准流程”来区分“单次使用批准流程”。 全局批准流程可重复使用。
>
>术语“组级全局批准流程”是指可重复用于项目且状态仅与特定组关联的批准流程。

有关审批流程的更多常规信息，请参阅 [审批流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

有关创建全局批准流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对项目、任务、问题或模板的访问权限或更高权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目、任务、问题或模板的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关将审批流程与工作项关联的注意事项

除了下面所述的注意事项外，我们建议您重新访问有关Workfront中审批流程的一般注意事项。 有关更多信息，请参阅 [审批流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* 您必须先创建项目、任务、问题、模板或模板任务，然后审批流程才能与它们关联。
* 将审批流程附加到已传递且项目当前处于状态的项目时，不会触发审批流程，也不会向审批人发送通知。

   **示例：** 如果任务处于“完成”状态，并且您附加了与“完成”状态关联的批准流程，则不会触发批准。

* 将审批流程附加到项目的第一个状态（通过为任务和项目使用模板，为问题使用队列设置设置，或为新任务定义项目的任务设置）时，如果撤回提交的审批，则会绕过审批流程。 在这种情况下，批准者不会收到任何通知。

   有关回调批准的更多信息，请参阅 [查看批准](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >任务或问题的第一个状态为“新”。 项目的第一个状态是Workfront管理员在系统的项目首选项中选择的状态。 有关信息，请参阅 [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 批准流程与对象的关联不会记录在对象的“更新”区域中。
* 您不能将审批流程与父任务关联。
* 将用户、团队或角色添加为审批者不会自动为他们授予与该审批关联的对象的权限。 当触发批准步骤时，他们将收到对象的权限。 否则，必须先与对象共享对象，然后才能做出批准决定。

以下各节介绍了将审批流程关联到项目、任务或问题的不同方法。

## 将全局审批流程与工作项关联 {#associate-a-global-approval-process-with-a-work-item}

您可以将全局审批流程与工作项（项目、任务、问题、模板、模板任务）关联。

全局批准流程必须可用于与工作项关联的组或系统中的所有组。

>[!NOTE]
您可以将项目审批流程附加到模板，将任务审批流程附加到模板任务。 在执行此操作后，当有人使用模板创建项目时，审批流程将分别变为项目或任务审批流程。 附加到模板或模板任务的一次性审批流程对于项目和任务来说仍然是一次性审批流程。

有关Workfront管理员如何为系统中的所有组配置全局批准流程，以及组管理员如何为组创建批准的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
您还可以修改全局批准流程以满足您的特定需求。 有关更多信息，请参阅 [修改全局批准流程以在特定对象上使用](#modify-a-global-approval-process-for-use-on-a-specific-object) 在本文中。

要将现有的全局批准流程与项目、任务、问题、模板或模板任务相关联，请执行以下操作：

1. 转到要关联审批流程的工作项。
1. 单击 **批准** 中。

   您可能需要单击 **显示更多**，然后单击 **批准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   此时将显示选定的审批流程。

1. 展开 **使用现有** 下拉菜单，然后选择现有的批准流程。

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   此时将显示选定的审批流程。

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. 单击&#x200B;**保存**。
1. （可选）如果要修改附加到项目的现有批准，请单击编辑批准流程。 这会将全局批准流程更改为一次性批准流程。 有关更多信息，请参阅 [修改全局批准流程以在特定对象上使用](#modify-a-global-approval-process-for-use-on-a-specific-object) 在本文中。

## 修改全局批准流程以在特定对象上使用 {#modify-a-global-approval-process-for-use-on-a-specific-object}

您的Workfront管理员或组管理员将创建供您使用的全局批准流程，如 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

修改附加到项目的全局批准流程与修改一次性批准流程相同。

您可以修改全局批准流程以符合您与其关联的项目、任务或问题的任何特定需求。

>[!IMPORTANT]
在修改全局批准流程时，该流程将变成一次性批准流程，只能在修改该流程的对象上使用。 全局批准流程保持不变。
修改全局批准流程时请考虑以下限制：
* 仅对要与审批流程关联的项目、任务或发放修改审批流程。
* 管理员对原始全局批准流程所做的任何未来更改都不会反映在您修改的全局批准流程上。
>


要修改已附加到项目的审批流程，请执行以下操作：

1. 向项目、任务或问题添加全局批准流程。

   有关说明，请参阅 [将全局审批流程与工作项关联](#associate-a-global-approval-process-with-a-work-item) 在本文中。

   >[!IMPORTANT]
   确保单击 **保存** 添加批准时。

1. 添加全局批准流程后，单击 **编辑**&#x200B;图标 ![](assets/edit-icon.png) 中。 此操作可将全局或组级别的审批流程转变为一次性审批流程。
1. 对现有批准流程进行任何更改。 有关更多信息，请参阅 [将一次性使用的审批流程与项目、任务、问题、模板或模板任务相关联](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) 在本文中。
1. 单击 **保存**，然后单击 **保存** 再次确认您要将全局批准流程转换为仅可用于此对象的一次性批准流程。

## 将一次性使用的审批流程与项目、任务、问题、模板或模板任务相关联 {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

您可以创建仅用于特定项目、任务或问题的一次性审批流程。

您还可以将一次性使用的审批流程与模板或模板任务相关联，以便该流程可用于使用该模板创建的项目和任务。

>[!NOTE]
您可以将一次性审批流程与项目、任务、问题、模板或模板任务的任何系统级别或组级别状态关联。 有关Workfront状态的信息，请参阅 [创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

通过这种方式创建批准流程，您可以创建自定义批准流程以满足您的需求。 但是，审批流程将来不能与其他工作项关联。

或者，您可以修改特定项目的全局批准流程，该流程也会变成一次性批准流程。 有关信息，请参阅 [修改全局批准流程以在特定对象上使用](#modify-a-global-approval-process-for-use-on-a-specific-object) 在本文中。

要创建一次性审批流程，请执行以下操作：

1. 转到要关联审批流程的项目、任务、问题、模板或模板任务。
1. 单击 **批准** 中。

   您可能需要单击 **显示更多** > **批准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 单击 **创建单次使用**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. 完成文章“为工作项创建系统级别或组级别的全局审批流程”部分中从步骤6开始的步骤 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   附加一次性使用审批流程后，该流程将显示为“`<Custom>`模板和模板任务的编辑框内的审批流程字段。 有关编辑模板或模板任务的信息，请参阅以下文章：
   * [编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [编辑模板任务](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## 从工作项中删除或删除审批流程

您可以删除全局或组级别的审批流程，也可以从以前与之关联的项目、任务或问题中删除一次性审批流程。

存在以下情形： 

* 删除全局或组级审批流程不会删除审批。 批准仍可供将来使用。
* 删除单用户批准流程会从Workfront中删除该流程，并且无法恢复该流程。

要从工作项中删除或删除审批流程，请执行以下操作：

1. 转到项目、任务、问题、模板或模板任务，您要在其中删除之前添加的批准流程。
1. 单击 **批准** 中。

   您可能需要单击 **显示更多** > **批准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 根据与项目关联的批准类型，单击“批准”部分右上角的以下图标之一：

   * **删除**&#x200B;图标 ![](assets/remove-icon---x-in-circle.png) 进行全局或组级别的批准。
   * **删除**&#x200B;图标 ![](assets/delete.png) 用于单次使用审批。

1. 单击 **删除** 或 **删除** 确认。

   审批流程将从工作项中删除。

## 自动将审批流程与工作项关联

您可以使用以下工作流自动将审批流程与工作项关联：

* 对于项目和任务，您可以使用模板关联审批流程。 您可以将现有审批流程附加到“模板审批”选项卡或“模板任务审批”选项卡。 有关将现有审批与工作项目关联的信息，请参阅 [将全局审批流程与工作项关联](#associate-a-global-approval-process-with-a-work-item) 在本文中。
* 对于现有项目上的新任务，您可以在“编辑项目”框的“任务设置”区域中关联全局审批流程或组级别的全局审批流程。 有关信息，请参阅文章中的“任务设置”部分 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md).
* 对于问题，您可以通过将现有审批流程与请求队列关联，将审批与添加到项目的每个新问题关联起来。 有关配置请求队列的信息，请参阅 [创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
