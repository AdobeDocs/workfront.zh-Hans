---
title: 配置全局审批设置
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 作为Adobe Workfront管理员，您可以在Workfront中确定批准流程的全局设置。 这些设置影响系统中的所有工作项批准流程。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# 配置全局审批设置

作为Adobe Workfront管理员，您可以在Workfront中确定批准流程的全局设置。 这些设置影响系统中的所有工作项批准流程。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是系统管理员或拥有对审批流程具有管理访问权限的计划许可证</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 配置全局审批设置

1. 以Workfront管理员身份登录到Workfront 。
1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 单击&#x200B;**进程** > **审批** 。

1. 单击&#x200B;**审批**&#x200B;区域名称旁边的&#x200B;**设置**&#x200B;图标![](assets/gear-icon-settings.png)。

1. 在出现的&#x200B;**审批设置**&#x200B;框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">将&lt;number&gt;天添加到计划完成日期以适应审批流程</td> 
      <td> <p>指定用于向需要批准的任务的计划完成日期添加时间的分钟数、小时数、天数、周数或月数。 选择“经过的时间”分钟、小时、天或周，以添加时间，包括系统工作时间表日历中指定的任何周末、节假日和非工作小时。</p> 
      <p>例如，如果任务在星期五分配，其持续时间为经过的3天，则任务完成日期将设置为星期一（假设星期六和星期日为周末）。 如果任务的持续时间为3天（未经过），则任务完成日期将设置为星期三。</p>
      <p><b>注意</b>：启用添加额外时间以适应任务的审批将影响任务的时间表和项目的时间表。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">对于包含角色的审批流程，要求审批者加入项目团队</td> 
      <td> <p>当审批流程包含角色时，如果不需要审批者加入项目团队，请选择此选项。 将审批决策分配给工作角色时，只有拥有项目中的相关角色的用户才能看到审批。 如果启用此设置，则任何具有该工作角色的用户都将收到审批请求，无论他们是否属于项目团队。 有关编辑用户的项目角色的信息，请参阅<a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理项目团队</a>。 </p> 
      <p><b>提示</b>：当您将审批分配给角色并且选项<b>审批者不需要位于项目团队中（对于包含角色的审批流程）</b>被禁用，但项目团队中没有与审批中的角色匹配的角色时，审批被重新分配给项目所有者。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">禁用审批委托</td> 
      <td> <p>选择此选项可禁用系统中的用户将审批委派给其他用户的功能。 选择此选项时，将从Workfront中删除委托审批的选项，并停止任何现有的审批委托。</p> <p>有关在Workfront中委托审批的更多信息，请参阅<a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">委托审批请求</a> 。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在项目、任务或问题处于未决批准状态时编辑自定义表单</td> 
      <td> <p>选择此选项可允许用户在处于未决批准状态时编辑项目、任务和问题的自定义表单。 这是默认设置。</p> 
      <p>选中此选项时：</p> 
       <ul> 
       <li>当对象正在等待审批时，所有审批者（以及有权编辑自定义表单的任何其他用户）都可以对自定义表单进行更改，而不管当前审批路径或审批步骤如何。</li> 
       <li>在审批流程中对自定义表单所做的更改不会影响更改之前所做的任何审批决策。</li> 
       <li> <p>无论此设置如何，都会以相同的方式跟踪对项目、任务或问题所做的任何更改。 </p> <p>例如，如果您添加了要在更新流中跟踪的自定义表单字段，则对表单的任何更改都将在对象的更新流中跟踪。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许用户撤消刚创建、等待批准的请求</td> 
      <td> <p>选择此选项可配置用户是否可以撤回其第一个状态的问题或待批准的请求。 通过配置请求队列，您可以将问题或请求的第一个状态与批准流程相关联。 </p> 
      <p>有关请求队列的详细信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>。</p> 
      <p>执行下列操作之一：</p> 
       <ul> 
       <li>选择此选项可允许用户撤消对问题或请求的第一个状态的批准。 在这种情况下，他们可以在处于未决批准状态的新问题或请求上看到“撤消”&lt;按钮。 当他们选择撤回问题时，将收到警告，指出问题也将被删除。 在确认将其召回后，该问题将被删除。 </li> 
       <li> <p>取消选择此选项可防止用户调用其第一个状态为未决批准的问题或请求。 他们看不到新问题或请求上的“撤消”按钮，必须获得批准。 这是默认选项。</p> 
       <p>有关查看等待审批的项目的详细信息，请参阅<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看审批</a>。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存更改。**
