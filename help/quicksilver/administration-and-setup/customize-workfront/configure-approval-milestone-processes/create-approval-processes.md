---
title: 创建工作项的审批流程
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 您可以创建用户可以附加到工作项（项目、任务、问题、模板或模板任务）、文档或验证的审批流程。 批准流程可确保对象上的指定受分配人在对象在系统中继续前进之前审阅某些更改。
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '2163'
ht-degree: 1%

---

# 创建工作项的审批流程

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

您可以创建用户可以附加到工作项（项目、任务、问题、模板或模板任务）、文档或验证的审批流程。 批准流程可确保对象上的指定受分配人在对象在系统中继续前进之前审阅某些更改。

本文介绍如何为工作项（项目、任务、问题、模板或模板任务）创建系统级或组级全局审批流程。

有关与文档或验证关联的批准的信息，请参阅以下文章：

* [请求文档审批](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>用户还可以为其拥有管理权限的项目、任务、问题、模板或模板任务创建一次性审批流程。
>
>本文使用“全局批准流程”一词来区分一次性批准流程。 可以重复使用全局批准流程。
>
>在组层，全局审批流程仅限于属于该组的工作项和状态。
>
>有关一次性审批流程的信息，请参阅 [审批流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) 和 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新计划：标准 </p>
 <p>或</p> 
<p>当前计划：计划 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>如果您是Workfront管理员或者对审批流程具有管理访问权限，则可以为特定组创建系统级审批流程或组级审批流程。</p> 
   <p>如果您是组管理员，则可以为所管理的组创建组级批准流程。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 为工作项创建系统级或组级全局审批流程

{{step-1-to-setup}}

1. （视情况而定）如果要创建系统级批准流程，请单击 **进程** > **审批** 在左侧面板中。

   或

   如果要创建组级批准流程，请单击 **组** ![](assets/groups-icon.png)，单击组的名称，然后单击 **审批**.

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. 选择 **项目审批**， **任务审批**，或 **问题审批** 选项卡。

1. 单击 **新建批准流程**.
1. 在显示的框中指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">批准流程名称</td> 
      <td><p>键入审批流程的描述性名称。 在将审批流程应用于对象时，用户会看到此名称，如中所述 <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">将新的或现有的审批流程与工作关联</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td><p>键入审批流程的描述。 这显示在 <b>审批</b> 中的部分 <b>设置</b> 批准流程名称旁边的区域。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">活动</td> 
      <td> <p>如果您希望其他用户能够将审批流程附加到他们创建的项目、任务和问题，请保持启用此选项。 </p> <p>此选项默认处于启用状态。</p> <p> 提示：当您的组织不再需要使用审批流程，但希望保留有关其使用的历史信息时，将审批流程标记为不活动会很有用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此批准流程的使用者可以为 </td> 
      <td> <p>如果您希望审批流程仅适用于特定组的项目、任务、问题和模板，请开始键入组的名称，然后在组出现时选择该名称：</p> 
       <ul> 
       <li>如果您是系统管理员或对审批流程具有管理访问权限，则键入组名时，可以在系统中看到任何组。 <b>所有组</b> 默认情况下处于选中状态。 </li> 
       <li>如果您是组管理员，但没有审批流程的管理权限，则可以在键入审批流程名称时将审批流程分配给您管理的任何组。 此 <b>所有组</b> 选项不可用。</li> 
       </ul> 
       <p>此选项不适用于一次性审批流程。</p> 
       <p><b>警告</b>：当您对特定于组的审批流程进行更改时，已与工作项关联的现有审批流程可能会发生更改。 有关这些更改的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>.</p> 
       <p>有关从组的页面列出和管理组的审批流程的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">组级别审批流程</a>. </p> 
       <p>有关对审批流程的管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 使用以下选项配置批准流程的路径。

   您可在路径中指定批准流程中需要执行的操作。 可在路径中创建阶段，以指示需要谁按什么顺序进行批准工作。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">启动审批流程（当状态设置为</p> </td> 
      <td> <p>选择将触发工作项的审批流程的状态。 当有人将工作项更新为此状态时，其审批流程就会开始。 </p> <p>无法为多个审批流程路径选择相同状态。</p> <p>可用的状态取决于在选项下选择的内容 <b>此审批的使用者包括</b> （见上表）：</p> 
       <ul> 
       <li> 如果 <b>所有组</b> 选中时，仅系统范围状态可用
       <li> <p>如果选择了特定组，则仅对该组可用的状态可用</p> </li> 
       </ul> <p>有关审批流程如何处理状态的信息，请参阅部分 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">审批流程如何依赖状态</a> 在文章中 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段名称</td> 
      <td>（可选）键入描述路径第一阶段的名称。 如果未指定阶段名称，则默认名称为 <b>阶段1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批者</td> 
      <td> <p>开始键入要指定为此阶段的批准者的用户、团队或工作角色的名称，然后在该名称出现在下拉列表中时单击该名称。 您只能添加活动用户， <span>职位角色</span>和团队。 </p>

   <p><b>提示</b>：</p>

   <p>将用户添加为审批者时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。</p>
      <p>您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">授予用户访问权限</a>. </p>

   <p><b>注意</b>：

   将用户、团队或角色添加为批准者，不会自动授予他们与该批准相关联的对象的权限。 在触发审批步骤时，用户会获得对对象的权限。 否则，必须先与他们共享对象，然后才能作出批准决定。 </p> <p>也可以通过指定个人的角色将个人指定为批准者。 例如，您可以将项目所有者、项目发起人、Portfolio所有者、项目群所有者或经理分配为批准者。 当您开始键入时，这些选项会自动显示。</p>

   <p><b>重要</b>：  
       <ul> 
       <li> <p>当您将审批分配给项目发起人并且没有人被指定为项目发起人时，审批将重新分配给项目所有者。 如果没有指定任何人为项目的所有者，则会将审批分配给Workfront管理员。 </p> </li> 
      </ul> 
       <ul> 
       <li> <p>当您向角色分配审批并且 <b>对于包含角色的审批流程，要求审批者加入项目团队</b> 已禁用，但项目团队中没有与审批角色匹配的角色，审批被重新分配给项目所有者。 有关审批设置的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局审批设置</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>当您将审批分配给项目责任人，并且没有指定任何人为项目责任人时，审批将重新分配给主要Workfront管理员，如设置区域的客户信息部分所述。 有关信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">配置系统的基本信息</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>您可以重复此过程以将多个批准者添加到阶段。 单个阶段可以包括用户、团队和工作角色作为批准者的组合。 您可以添加到阶段的批准者数量没有限制。</p> <p><b>重要</b>：  <p>将工作角色指定为批准者时，与该工作角色关联、也位于项目团队中的所有用户都可以作出批准决定。 </p> <p>将团队分配为批准者时，该团队中的任何用户都可以就批准做出决定。 </p> <p>有关项目团队的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>. 有关批准工作的更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">审批工作 </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需一个决策 <br> <br>（仅当将多个批准者添加到阶段时才显示） </td> 
      <td> <p>如果阶段中的任何一位审批者可以在此阶段批准或拒绝工作项，请选择此选项。 此操作允许工作项离开阶段。 </p> <p>如果未选择此选项，则在项目离开阶段之前，所有已标识的批准者必须批准或拒绝阶段（按任何顺序）。 如果任何一位批准者拒绝该阶段，该进程将中断并重新开始，以便进行所需的更改。 然后，审批者可以再次批准或拒绝该阶段。</p> <p>当团队被指定为批准者时，团队的任何成员都可以授予或拒绝阶段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">添加阶段</p> </td> 
      <td><p>（可选）使用上面三行中说明的选项，向路径中添加另一个阶段。 您可以根据需要向路径添加任意数量的阶段。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">选择批准被拒绝时发生的情况</p> </td> 
      <td> <p>选择当工作项在路径的任何阶段被拒绝时要执行的操作：</p> 
       <ul> 
       <li><b>创建问题</b>：（仅适用于项目和任务审批流程）在运行审批流程的项目或任务中创建问题。 任务的默认已分配资源，或项目的所有者已分配给问题。 默认情况下，创建的问题名称为 <b>批准被拒绝(&lt;project or="" task="" name=""&gt;)</b>. 这是一个拒绝问题，在任务或项目下输入，具体取决于发生拒绝的审批流程。</li> 
       <li> <p><b>将状态设置为</b>：选择以下选项之一：</p> 
       <ul> 
       <li><b>以前的状态</b>：被拒绝的项目、任务或问题恢复到激活审批流程状态之前的状态。</li> 
       <li><p><b>列表中的任何其他状态</b>：被拒绝的对象将移动到您选择的状态，例如已搁置。 您可以选择默认状态之一，也可以选择添加到Workfront系统中的自定义状态。</p>
       <p>如果您选择与审批流程关联的状态作为拒绝状态，则被拒绝的对象将移动到选定状态，并将标记为“待审批”。</p> 
       <p> 例如，如果您选择已搁置作为拒绝状态，并且该已搁置状态与审批流程相关联，被拒绝的对象置于“已搁置 — 待审批”状态，需要审批。</p>

   </tr> 
    </tbody> 
   </table>

1. （可选）单击 **添加路径** 向审批流程添加其他路径，请参阅上一步骤中的选项列表。

   新路径必须与其他状态关联。 更新项以显示此状态时会触发路径。 对于同一状态，不能有两个路径。

1. 单击&#x200B;**保存**。
1. 现在审批流程已创建，请继续执行以下任一操作：

   * 将审批流程与系统中的特定项目、任务或问题相关联，如中所述 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 在Workfront之外，通知用户审批流程可供他们关联到其项目、任务或问题，如中所述 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 创建另一个审批流程，如果此审批流程被拒绝并且项目具有其他状态，则会触发该审批流程。 这为您提供了一种将审批流程链接在一起的方法。

有关编辑批准流程的信息，请参阅 [编辑审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## 将审批流程与工作项关联

当您要为工作项（项目、任务或问题）创建审批流程时，

1. 首先创建批准流程
1. 创建工作项
1. 将审批流程与工作项关联

有关将审批流程与工作项关联的说明，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>任何对项目、任务或问题具有管理权限的Workfront用户都可以创建一次性审批流程，以便仅用于创建这些流程的对象。 有关更多信息，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 允许用户修改单个工作项的全局审批流程

默认情况下，拥有项目、任务和问题管理权限的用户可以为其创建一次性审批流程。 有关将一次性审批流程添加到项目、任务和问题的信息，请参阅部分 [将一次性审批流程与项目、任务、问题、模板或模板任务关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) 在文章中 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

用户还可以更改与工作项关联的全局审批流程的设置。 这些更改仅影响与系统级审批流程关联的项目、任务或问题。 有关更多信息，请参阅部分 [修改用于特定对象的全局批准流程](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) 在文章中 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md))。
