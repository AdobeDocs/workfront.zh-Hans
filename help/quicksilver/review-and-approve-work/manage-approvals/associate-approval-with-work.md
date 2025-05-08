---
product-area: projects
navigation-topic: approvals
title: 将新的或现有的审批流程与工作关联
description: 本文介绍了如何将审批流程与工作项关联。 有关将审批与验证或文档关联的信息，请参阅以下文章。
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 06e42fa713bc9b0c1e308feb2b84ca62dafa416c
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 将新的或现有的审批流程与工作关联

本文介绍了如何将审批流程与工作项关联。 有关将审批与验证或文档关联的信息，请参阅以下文章：

* [使用自动化工作流创建高级校对](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [请求文件审批](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

您可以在Adobe Workfront中将全局或一次性审批流程与工作项关联。 存在以下情况：

* 将现有的全局审批流程与项目、任务、问题、模板或模板任务关联。 某些全局审批流程适用于系统中的所有组。 组级别的全局审批流程仅适用于某些组。
* 创建一次性审批流程，并将其与现有项目、任务、问题、模板或模板任务关联。

>[!NOTE]
>
>本文使用“全局批准流程”一词来区分“一次性批准流程”。 可以重复使用全局批准流程。
>
>术语“组级别全局审批流程”是指可以重复用于项目的审批流程，其状态仅与特定组关联。

有关批准流程的更多常规信息，请参阅[批准流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)。

有关创建全局审批流程的信息，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对项目、任务、问题或模板的访问权限或更高</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目、任务、问题或模板的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 有关将审批流程与工作项关联的注意事项

除了下述注意事项外，我们建议您重新访问有关Workfront中审批流程的一般注意事项。 有关详细信息，请参阅[审批流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* 您必须先创建项目、任务、问题、模板或模板任务，然后才能将审批流程与其关联。
* 当您将审批流程附加至状态为已通过、当前状态为的项时，不会触发审批流程，也不会向审批人发送任何通知。

  **示例：**&#x200B;如果任务处于“完成”状态，并且您附加了与“完成”状态关联的审批流程，则不会触发审批。

* 在将审批流程附加到项的第一个状态时（通过使用任务和项目的模板、使用问题的队列设置设置设置或为新任务定义项目的任务设置），如果撤消已提交的审批，则会绕过审批流程。 在这种情况下，审批者不会收到任何通知。

  有关撤消审批的详细信息，请参阅[查看审批](../../review-and-approve-work/manage-approvals/view-approvals.md)。

  >[!TIP]
  >
  >任务或问题的第一个状态为“新建”。 项目的第一个状态是您的Workfront管理员在系统中的项目首选项中选择的状态。 有关信息，请参阅[配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 批准流程与对象的关联不会记录在该对象的“更新”区域中。
* 您不能将审批流程与父任务关联。
* 将用户、团队或角色添加为批准者，不会自动授予他们与该批准相关联的对象的权限。 在触发审批步骤时，用户会获得对对象的权限。 否则，必须先与他们共享对象，然后才能作出批准决定。

以下各节介绍了将审批流程与项目、任务或问题关联的不同方法。

## 将全局审批流程与工作项关联 {#associate-a-global-approval-process-with-a-work-item}

您可以将全局审批流程与工作项（项目、任务、问题、模板、模板任务）关联。

您可以访问任何全局审批流程，只要该流程与您所属的组或系统中的所有组共享。

<!--The global approval process must be available to the group associated with the work item or to all groups in the system.-->

>[!NOTE]
>
>您可以将项目审批流程附加到模板，将任务审批流程附加到模板任务。 执行此操作后，当有人使用模板创建项目时，审批流程将分别变为项目或任务审批流程。 附加到模板或模板任务的一次性审批流程仍然是项目和任务的一次性审批流程。

有关Workfront管理员如何为系统中的所有组配置全局审批流程以及组管理员如何为组创建审批的信息，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

>[!NOTE]
>
>您还可以修改全局批准流程以满足特定需求。 有关详细信息，请参阅本文中的[修改用于特定对象](#modify-a-global-approval-process-for-use-on-a-specific-object)的全局审批流程。

要将现有的全局审批流程与项目、任务、问题、模板或模板任务相关联，请执行以下操作：

1. 转到要关联审批流程的工作项。
1. 单击左侧面板中的&#x200B;**审批**。

   任务![&#128279;](assets/approvals-section-on-task-highlighted-nwe-350x246.png)上的审批分区

1. ![使用现有审批或创建单次使用审批](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   此时会显示选定的审批流程。

1. 展开&#x200B;**使用现有**&#x200B;下拉菜单，然后选择现有审批流程。

   ![审批菜单](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   此时会显示选定的审批流程。

   ![附加到任务的现有审批](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. 单击&#x200B;**保存**。
1. （可选）如果要修改附加到项目的现有批准，请单击“编辑批准流程”。 这会将全局批准流程更改为单次使用批准流程。 有关详细信息，请参阅本文中的[修改用于特定对象](#modify-a-global-approval-process-for-use-on-a-specific-object)的全局审批流程。

## 修改用于特定对象的全局批准流程 {#modify-a-global-approval-process-for-use-on-a-specific-object}

您的Workfront管理员或组管理员创建全局审批流程供您使用，如[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)中所述。

修改附加到项目的全局审批流程与修改一次性审批流程相同。

您可以修改全局审批流程，以符合与项目、任务或问题关联的任何特定需求。

>[!IMPORTANT]
>
>修改全局审批流程后，该流程将变成仅用于修改对象的单次使用审批流程。 全球审批流程保持不变。
>
>修改全局批准流程时，请考虑以下限制：
>
>* 仅针对与审批流程关联的项目、任务或问题修改审批流程。
>* 管理员对原始全局审批流程所做的任何未来更改都不会反映在您修改的全局审批流程中。
>

要修改已附加到项目的审批流程，请执行以下操作：

1. 向项目、任务或问题添加全局审批流程。

   有关说明，请参阅本文中的[将全局审批流程与工作项关联](#associate-a-global-approval-process-with-a-work-item)部分。

   >[!IMPORTANT]
   >
   >确保在添加批准时单击&#x200B;**保存**。

1. 添加全局审批流程后，单击审批页面右上角的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。 此操作可将全局或组级别的审批流程转换为单次使用的审批流程。
1. 对现有审批流程进行任何更改。 有关详细信息，请参阅本文中的[将一次性审批流程与项目、任务、问题、模板或模板任务相关联](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task)部分。
1. 单击“**保存**”，然后再次单击“**保存**”以确认要将全局审批流程转换为仅在此对象上可用的一次性审批流程。

## 将一次性审批流程与项目、任务、问题、模板或模板任务关联 {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

您可以创建仅用于特定项目、任务或问题的一次性审批流程。

您还可以将一次性审批流程与模板或模板任务相关联，以便该流程可用于从该模板创建的项目和任务。

>[!NOTE]
>
>您可以将一次性审批流程与项目、任务、问题、模板或模板任务的任何系统级别或组级别状态关联。 有关Workfront状态的信息，请参阅[创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

通过这种方式创建审批流程，您可以创建自定义审批流程以满足您的需求。 但是，审批流程不能与将来的其他工作项相关联。

或者，您可以修改特定物料的全局审批流程，该流程也会变成一次性审批流程。 有关信息，请参阅本文中的[修改用于特定对象](#modify-a-global-approval-process-for-use-on-a-specific-object)的全局批准流程部分。

要创建一次性审批流程，请执行以下操作：

1. 转到要关联审批流程的项目、任务、问题、模板或模板任务。
1. 单击左侧面板中的&#x200B;**审批**。

   任务![&#128279;](assets/approvals-section-on-task-highlighted-nwe-350x246.png)上的审批分区

1. 单击&#x200B;**创建一次性**。

   ![审批菜单](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. 完成文章[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)中的“为工作项创建系统级别或组级别全局审批流程”一节中的步骤6。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >附加一次性审批流程后，它在模板和模板任务的编辑框内的审批流程字段中显示为“`<Custom>`”。 有关编辑模板或模板任务的信息，请参阅以下文章：
   >
   >* [编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [编辑模板任务](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## 从工作项移除或删除审批流程

您可以删除全局或组级别的审批流程，也可以从以前与其关联的项目、任务或问题中删除一次性审批流程。

存在以下情况： 

* 删除全局或组级别的审批流程不会删除审批。 该批准仍可用于将来使用。
* 删除单用户审批流程会将其从Workfront中删除，并且无法恢复。

要从工作项中删除或删除审批流程，请执行以下操作：

1. 转到要移除先前添加的审批流程的项目、任务、问题、模板或模板任务。
1. 单击左侧面板中的&#x200B;**审批**。

   任务![&#128279;](assets/approvals-section-on-task-highlighted-nwe-350x246.png)上的审批分区

1. 根据与项目关联的批准类型，单击“批准”部分右上角的以下图标之一：

   * **全局或组级别审批的“删除”**&#x200B;图标![“删除”图标](assets/remove-icon---x-in-circle.png)。
   * **一次性审批的“删除”**&#x200B;图标![“删除”图标](assets/delete.png)。

1. 单击&#x200B;**删除**&#x200B;或&#x200B;**删除**&#x200B;确认。

   审批流程将从工作项中删除。

## 自动将审批流程与工作项关联

您可以使用以下工作流自动将审批流程与工作项关联：

* 对于项目和任务，您可以使用模板关联审批流程。 您可以将现有审批流程附加到“模板审批”选项卡或“模板任务审批”选项卡。 有关将现有审批与工作项关联的信息，请参阅本文中的[将全局审批流程与工作项关联](#associate-a-global-approval-process-with-a-work-item)。
* 对于现有项目中的新任务，您可以在“编辑项目”框的“任务设置”区域中关联全局审批流程或组级别全局审批流程。 有关信息，请参阅文章[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)中的“任务设置”部分。
* 对于问题，通过将现有审批流程与请求队列关联，您可以将审批与添加到项目的每个新问题关联。 有关配置请求队列的信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
