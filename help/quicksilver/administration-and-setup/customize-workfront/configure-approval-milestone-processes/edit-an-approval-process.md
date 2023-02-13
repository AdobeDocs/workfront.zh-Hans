---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: 编辑批准流程
description: 如果您是Adobe Workfront管理员，或者您拥有审批流程的管理权限，则可以查看和编辑系统中的所有审批流程。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 5%

---

# 编辑批准流程

如果您是Adobe Workfront管理员，或者您拥有审批流程的管理权限，则可以查看和编辑系统中的所有审批流程。

如果您是群组管理员，则可以查看和编辑与您管理的群组或群组关联的审批流程。

有关创建审批流程的信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* 在编辑已在使用的全局批准流程时，所做的更改会影响整个系统中已与其关联的所有对象。
>* 如果在已在对象上启动的审批流程上向当前阶段添加新的审批者，则该对象的流程将重置，审批者必须重新开始。
>
>  但是，如果您对已在对象上启动的批准流程进行了以下更改，则该流程会继续运行且不会中断：
>
>* 在当前阶段之外添加阶段
>* 在当前阶段之前添加其他审批者


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
   <td> <p>如果您不是系统管理员，则对审批流程的管理访问权限</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑现有审批流程

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).
1. （视情况而定）如果您正在编辑系统级别的批准流程，请单击 **流程** > **批准** 中。

   或

   如果您正在编辑组级别的审批流程，请执行以下操作：

   1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).
   1. 单击要列出或管理组审批流程的组名称。
   1. 在左侧面板中，单击 **批准**. 您可能需要单击 **显示更多** 第一个。

1. 单击 **项目批准**, **任务批准**&#x200B;或 **发出批准** 选项卡，具体取决于您要编辑的批准流程类型。

1. 选择要编辑的审批流程，然后单击 **编辑** 列表顶部。 此时将显示“编辑审批”流程框。

   ![](assets/edit-approval-process-global-area-new.png)

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
      <td> <p>如果您希望其他用户能够将批准流程附加到他们创建的项目、任务和问题，请启用此选项。 </p> <p>默认情况下，此选项处于启用状态。</p> <p>提示：如果贵组织不再需要使用审批流程，但您希望保留其使用情况的历史信息，则将审批流程标记为不活动会非常有用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此批准流程的使用者可以为 </td> 
      <td> <p>如果您希望审批流程仅适用于属于特定组的项目、任务、问题和模板，请开始键入组的名称，然后在显示时选择该名称：</p> 
       <ul> 
        <li>如果您是系统管理员，或者您拥有审批流程的管理权限，则在键入系统名称时，您可以在系统中看到任何组。 <b>所有组</b> 默认情况下，处于选中状态。 </li> 
        <li>如果您是群组管理员，无权管理审批流程，则可以在键入群组名称时将审批流程分配给您管理的任何群组。 的 <b>所有组</b> 选项不可用。</li> 
       </ul> <p>此选项不适用于一次性审批流程。</p> <p><b>警告</b>:当您更改特定于组的审批流程时，已与工作项关联的现有审批流程可能会发生更改。 有关这些更改的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>.</p> <p>有关从群组页面列出和管理群组审批流程的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">组级别的审批流程</a>. </p> <p>有关对审批流程的管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
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
      <li> 如果 <b>所有组</b> ，则只有系统范围的锁定状态可用。 <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>如果选择了特定群组，则只有该群组可用的状态才可用</p> </li> 
      </ul> <p>有关审批流程如何使用状态的信息，请参阅部分 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">审批流程如何依赖状态</a> 在文章中 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段名称</td> 
      <td>（可选）键入描述路径第一阶段的名称。 如果未指定阶段名称，则默认名称为 <b>阶段1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批者</td> 
      <td> <p>开始键入要指定为此阶段审批者的用户、团队或工作角色的名称，然后在下拉列表中显示该名称时单击该名称。 您只能添加活动用户、工作角色和团队。 </p>

   <p><b>笔尖</b>:</p>

   <p>在添加用户作为审批者时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。</p>

   <p><b>注释</b>:

   将用户、团队或角色添加为审批者不会自动为他们授予与该审批关联的对象的权限。 当触发批准步骤时，他们将收到对象的权限。 否则，必须先与对象共享对象，然后才能做出批准决定。 </p>
   <p>您还可以通过指定个人的角色将个人指定为审批者。 例如，您可以将项目所有者、项目赞助者、Portfolio所有者、项目所有者或经理分配为审批者。 当您开始键入内容时，这些选项会自动显示。</p> 
      <p><b>重要信息</b>:  
      <ul> 
      <li> 当您为项目发起人分配了批准，并且没有人被指定为项目的发起人时，批准将重新分配给项目所有者。 如果没有人指定为项目所有者，则会将批准分配给Workfront管理员。 </li> 
      <li> 在为角色和选项分配批准时 <b>项目团队不需要审批者</b> 已禁用，但项目团队中的任何角色都与审批时的角色不匹配，则审批会重新分配给项目所有者。 有关批准设置的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准设置</a>.
      </li> 
      <li>如果您为项目所有者分配了批准，并且没有人被指定为项目所有者，则该批准将重新分配给主Workfront管理员，如“设置”区域的“客户信息”部分中所述。 有关信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">配置系统的基本信息</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>在将作业角色分配为批准者时，与该作业角色关联的所有用户（同时也在项目团队中）都可以对批准做出决策。 </p> 
      <p>当您将团队指定为审批者时，该团队中的任何用户都可以对批准做出决策。 </p> 
      <p>有关项目团队的更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a>. 有关批准工作的更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">批准工作 </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">只需一个决策</td> 
      <td>（仅当您将多个批准者添加到舞台时显示）如果舞台上的任何一个批准者可以批准或拒绝此阶段中的工作项，请选择此选项。 此操作允许工作项离开舞台。  
      <p>如果未选择此选项，则所有已识别的批准者都必须批准或拒绝该阶段（按任意顺序），然后该项目才离开该阶段。 如果任何一个批准者拒绝该阶段，则该进程会中断并重新开始，以便能够进行所需的更改。 然后批准者可以再次批准或拒绝该阶段。</p> 
      <p>当团队被指定为审批者时，团队的任何成员都可以授予或拒绝阶段。</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">添加阶段</p> </td> 
      <td>（可选）使用上面三行中介绍的选项，向路径中添加另一个阶段。 您可以根据需要向路径中添加任意数量的阶段。</td> 
     </tr>
     <tr> 
      <td role="rowheader"> 选择拒绝批准时发生的情况</td> 
      <td> <p>选择在路径的任何阶段拒绝工作项时要执行的操作：</p> 
      <ul> <li><strong>创建问题</strong>:（仅适用于项目和任务审批流程）在正在运行审批流程的项目或任务中创建问题。 为任务分配的默认资源，或将项目所有者分配给问题。 默认情况下，创建的问题的名称为 <strong>已拒绝批准（项目或任务名称）</strong>. 这是在任务或项目下输入的拒绝问题，具体取决于发生拒绝的审批流程。</li> 
      <li> <p><strong>将状态设置为</strong>:选择以下选项之一：</p> 
      <ul> <li><strong>上一状态</strong>:被拒绝的项目、任务或问题将在激活审批流程的状态之前还原为状态。</li> 
      <li> <p><strong>列表中的任何其他状态</strong>:被拒绝的对象将移至您选择的状态，如“暂挂”。 您可以选择添加到Workfront系统的默认状态之一或自定义状态。</p> <p>如果您选择与审批流程关联的状态作为审批路径的拒绝状态，则被拒绝的对象将移动到选定状态，并将标记为“待批准”。 </p>
      <p>例如，如果您选择已搁置作为拒绝状态，并且该已搁置状态与审批流程相关联，被拒绝的对象置于“已搁置 – 待审批”状态，需要审批。</p>    <p>对于系统范围的批准流程，仅系统范围的状态可用。</p> <p>对于特定于群组的审批流程，所有群组状态均可用。 这包括群组管理员专门为群组创建的任何自定义状态，以及任何系统范围的状态。 </p> <p>有关审批流程如何使用状态的信息，请参阅部分 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">审批流程如何依赖状态</a> 在文章中 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. （可选）单击 **添加路径** 要添加审批流程的其他路径，请参阅上一步中的选项列表。

   新路径必须与其他状态关联。 更新项目以显示此状态时，将触发路径。 不能有两个具有相同状态的路径。

1. 单击&#x200B;**保存**。
1. （可选）执行以下任一操作：

   * 将审批流程与整个系统中的特定项目、任务或问题关联，如 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 在Workfront之外，通知用户批准流程可供他们与其项目、任务或问题关联，如 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 创建另一个批准流程，该流程在此批准流程被拒绝且项目处于其他状态时触发。 这样，您就可以将审批流程链接在一起。
