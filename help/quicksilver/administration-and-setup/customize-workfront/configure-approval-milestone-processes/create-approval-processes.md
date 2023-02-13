---
title: 为工作项创建审批流程
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 您可以创建一个审批流程，用户可以将该流程附加到工作项（项目、任务、问题、模板或模板任务）、文档或校样。 审批流程可确保对象上的指定任务负责人在对象进入系统之前审查某些更改。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '2201'
ht-degree: 1%

---

# 为工作项创建审批流程

您可以创建一个审批流程，用户可以将该流程附加到工作项（项目、任务、问题、模板或模板任务）、文档或校样。 审批流程可确保对象上的指定任务负责人在对象进入系统之前审查某些更改。

本文介绍了如何为工作项（项目、任务、问题、模板或模板任务）创建系统级或组级全局审批流程。

有关与文档或校样关联的批准的信息，请参阅以下文章：

* [请求文档批准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>用户还可以为具有“管理”权限的项目、任务、问题、模板或模板任务创建一次性审批流程。
>
>本文使用术语“全局批准流程”来区分单次使用的批准流程。 全局批准流程可重复使用。
>
>在组级别，全局审批流程仅限于属于组的工作项目和状态。
>
>有关单次使用审批流程的信息，请参阅 [审批流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) 和 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>如果您是Workfront管理员，或者您拥有审批流程的管理权限，则可以为特定组创建系统级别审批流程或组级别审批流程。</p> 
   <p>如果您是群组管理员，则可以为您管理的群组创建群组级别的审批流程。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为工作项创建系统级或组级全局审批流程

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. （视情况而定）如果要创建系统级别的批准流程，请单击 **流程** > **批准** 中。

   或

   如果要创建组级别的审批流程，请单击 **群组** ![](assets/groups-icon.png)，单击群组的名称，然后单击 **批准**.

1. 单击 **项目批准**, **任务批准**&#x200B;或 **发出批准** 选项卡，具体取决于您要创建的批准流程类型。

1. 单击 **新审批流程**.
1. 在显示的框中指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">批准流程名称</td> 
      <td>为审批流程键入一个描述性名称。 如 <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">将新审批流程或现有审批流程与工作关联</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入审批流程的描述。 此参数显示在 <b>批准</b> 部分 <b>设置</b> 批准流程名称旁边的区域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">活动</td> 
      <td> <p>如果您希望其他用户能够将批准流程附加到他们创建的项目、任务和问题，请启用此选项。 </p> <p>默认情况下，此选项处于启用状态。</p> <p> 如果贵组织不再需要使用审批流程，但您希望保留其使用情况的历史信息，则将审批流程标记为不活动会非常有用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此批准流程的使用者可以为 </td> 
      <td> <p>如果您希望审批流程仅适用于属于特定组的项目、任务、问题和模板，请开始键入组的名称，然后在显示时选择该名称：</p> 
       <ul> 
       <li>如果您是系统管理员，或者您拥有审批流程的管理权限，则在键入系统名称时，您可以在系统中看到任何组。 <b>所有组</b> 默认情况下，处于选中状态。 </li> 
       <li>如果您是群组管理员，无权管理审批流程，则可以在键入群组名称时将审批流程分配给您管理的任何群组。 的 <b>所有组</b> 选项不可用。</li> 
       </ul> 
       <p>此选项不适用于一次性审批流程。</p> 
       <p><b>警告</b>:当您更改特定于组的审批流程时，已与工作项关联的现有审批流程可能会发生更改。 有关这些更改的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>.</p> 
       <p>有关从群组页面列出和管理群组审批流程的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">组级别的审批流程</a>. </p> 
       <p>有关对审批流程的管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 使用以下选项配置批准流程的路径。

   在路径中，您可以指定批准流程中需要执行的操作。 您可以在路径中创建阶段，以指明谁需要执行批准工作以及按什么顺序执行。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">启动审批流程（当状态设置为</p> </td> 
      <td> <p>选择将触发工作项审批流程的状态。 当某人将工作项更新为此状态时，即会开始其批准过程。 </p> <p>无法为多个批准流程路径选择相同的状态。</p> <p>可用状态取决于选项下选择的状态 <b>此批准可供</b> （如上表所述）：</p> 
       <ul> 
       <li> 如果 <b>所有组</b> ，则仅系统范围的状态可用
       <li> <p>如果选择了特定群组，则只有该群组可用的状态才可用</p> </li> 
       </ul> <p>有关审批流程如何使用状态的信息，请参阅部分 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">审批流程如何依赖状态</a> 在文章中 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段名称</td> 
      <td>（可选）键入描述路径第一阶段的名称。 如果未指定阶段名称，则默认名称为 <b>阶段1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批者</td> 
      <td> <p>开始键入要指定为此阶段审批者的用户、团队或工作角色的名称，然后在下拉列表中显示该名称时单击该名称。 您只能添加活动用户， <span>工作角色</span>和团队。 </p>

   <p><b>笔尖</b>:</p>

   <p>在添加用户作为审批者时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。</p>

   <p><b>注释</b>:

   将用户、团队或角色添加为审批者不会自动为他们授予与该审批关联的对象的权限。 当触发批准步骤时，他们将收到对象的权限。 否则，必须先与对象共享对象，然后才能做出批准决定。 </p> <p>您还可以通过指定个人的角色将个人指定为审批者。 例如，您可以将项目所有者、项目赞助者、Portfolio所有者、项目所有者或经理分配为审批者。 当您开始键入内容时，这些选项会自动显示。</p>

   <p><b>重要信息</b>:  
       <ul> 
       <li> <p>当您为项目发起人分配了批准，并且没有人被指定为项目的发起人时，批准将重新分配给项目所有者。 如果没有人指定为项目所有者，则会将批准分配给Workfront管理员。 </p> </li> 
      </ul> 
       <ul> 
       <li> <p>在您为角色分配批准时，以及 <b>审批者不需要加入项目团队（对于包含角色的审批流程）</b> 已禁用，但项目团队中没有与审批中的角色相匹配的角色，则审批会重新分配给项目所有者。 有关批准设置的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准设置</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>如果您为项目所有者分配了批准，并且没有人被指定为项目所有者，则该批准将重新分配给主Workfront管理员，如“设置”区域的“客户信息”部分中所述。 有关信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">配置系统的基本信息</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>您可以重复此过程，将多个批准者添加到舞台。 单个阶段可以包含用户、团队和作业角色作为批准者的组合。 可以添加到舞台的批准者数量没有限制。</p> <p><b>重要信息</b>:  <p>在将作业角色分配为批准者时，与该作业角色关联的所有用户（同时也在项目团队中）都可以对批准做出决策。 </p> <p>当您将团队指定为审批者时，该团队中的任何用户都可以对批准做出决策。 </p> <p>有关项目团队的更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>. 有关批准工作的更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">批准工作 </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需一个决策</td> 
      <td> <p>（仅当您将多个批准者添加到舞台时显示）如果舞台上的任何一个批准者可以批准或拒绝此阶段中的工作项，请选择此选项。 此操作允许工作项离开舞台。 </p> <p>如果未选择此选项，则所有已识别的批准者都必须批准或拒绝该阶段（按任意顺序），然后该项目才离开该阶段。 如果任何一个批准者拒绝该阶段，则该进程会中断并重新开始，以便能够进行所需的更改。 然后批准者可以再次批准或拒绝该阶段。</p> <p>当团队被指定为审批者时，团队的任何成员都可以授予或拒绝阶段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">添加阶段</p> </td> 
      <td>（可选）使用上面三行中介绍的选项，向路径中添加另一个阶段。 您可以根据需要向路径中添加任意数量的阶段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">选择拒绝批准时发生的情况</p> </td> 
      <td> <p>选择在路径的任何阶段拒绝工作项时要执行的操作：</p> 
       <ul> 
       <li><b>创建问题</b>:（仅适用于项目和任务审批流程）在正在运行审批流程的项目或任务中创建问题。 为任务分配的默认资源，或将项目所有者分配给问题。 默认情况下，创建的问题的名称为 <b>已拒绝批准(&lt;project or="" task="" name=""&gt;)</b>. 这是在任务或项目下输入的拒绝问题，具体取决于发生拒绝的审批流程。</li> 
       <li> <p><b>将状态设置为</b>:选择以下选项之一：</p> 
       <ul> 
       <li><b>上一状态</b>:被拒绝的项目、任务或问题将在激活审批流程的状态之前还原为状态。</li> 
       <li><p><b>列表中的任何其他状态</b>:被拒绝的对象将移至您选择的状态，如“暂挂”。 您可以选择添加到Workfront系统的默认状态之一或自定义状态。</p>
       <p>如果您选择与审批流程关联的状态作为拒绝状态，则被拒绝对象将移至选定状态，并且它将被标记为“待批准”。</p> 
       <p> 例如，如果为拒绝状态选择“暂挂”，并且“暂挂”状态与审批流程相关联，则被拒绝对象将处于“暂挂 — 待批准”状态，需要审批。</p>

   </tr> 
    </tbody> 
   </table>

1. （可选）单击 **添加路径** 要添加审批流程的其他路径，请参阅上一步中的选项列表。

   新路径必须与其他状态关联。 更新项目以显示此状态时，将触发路径。 不能有两个具有相同状态的路径。

1. 单击&#x200B;**保存**。
1. 现在，创建批准流程后，继续执行以下任一操作：

   * 将审批流程与整个系统中的特定项目、任务或问题关联，如 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 在Workfront之外，通知用户批准流程可供他们与其项目、任务或问题关联，如 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 创建另一个批准流程，该流程在此批准流程被拒绝且项目处于其他状态时触发。 这样，您就可以将审批流程链接在一起。

有关编辑批准流程的信息，请参阅 [编辑批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## 将审批流程与工作项关联

如果要为工作项（项目、任务或发放）创建审批流程，请先创建审批流程，然后创建工作项，然后您和您的用户可以将审批流程与工作项关联。

有关将审批流程与工作项关联的说明，请参阅 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>对项目、任务或问题具有管理权限的任何Workfront用户都可以创建一次性审批流程，以便仅在创建这些流程的对象上使用。 有关更多信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 允许用户修改单个工作项的全局批准流程

默认情况下，对项目、任务和问题具有管理权限的用户可以在其上创建一次性审批流程。 有关向项目、任务和问题添加一次性审批流程的信息，请参阅部分 [将一次性使用的审批流程与项目、任务、问题、模板或模板任务相关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) 在文章中 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

用户还可以更改与工作项关联的全局批准流程的设置。 这些更改仅影响与系统级别审批流程关联的项目、任务或问题。 有关更多信息，请参阅 [修改全局批准流程以在特定对象上使用](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) 在文章中 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md))。
