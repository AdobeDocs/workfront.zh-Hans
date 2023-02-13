---
title: 配置全局批准设置
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 作为Adobe Workfront管理员，您可以确定Workfront中审批流程的全局设置。 这些设置会影响系统中的所有工作项审批流程。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 1%

---

# 配置全局批准设置

作为Adobe Workfront管理员，您可以确定Workfront中审批流程的全局设置。 这些设置会影响系统中的所有工作项审批流程。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>您必须是系统管理员或拥有具有审批流程管理访问权限的计划许可证</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 配置全局批准设置

1. 以Workfront管理员身份登录Workfront 。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **流程** > **批准** .

1. 单击 **设置** 图标 ![](assets/gear-icon-settings.png) 旁边 **批准** 区域名称。

1. 在 **批准设置** 框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加 &lt;number&gt; 计划完成日期的天数，以供审批流程使用</td> 
      <td> <p>指定分钟、小时、天、周或月数，以将时间添加到需要批准的任务的计划完成日期。 选择“已用”分钟、小时、天或周，以添加时间，包括系统工作计划日历中指定的任何周末、节假日和非工作时间。</p> 
      <p>例如，如果在星期五分配了任务，并且该任务的持续时间为3天，则任务完成日期将设置为星期一（假定星期六和星期日是周末）。 如果任务的持续时间为3天（未经过），则任务完成日期将设置为星期三。</p>
      <p><b>注意</b>:如果能够增加额外的时间来审批任务，则会影响任务和项目的时间表。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批者不需要加入项目团队（对于包含角色的审批流程）</td> 
      <td> <p>如果在审批流程包含角色时不需要审批者加入项目团队，请选择此选项。 将批准决策分配给职务角色时，只有在项目中具有与其关联角色的用户才会看到批准。 如果启用此设置，则具有该作业角色的任何用户都会收到批准请求，无论他们是否在项目团队中。 有关编辑用户项目角色的信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理项目团队</a>. </p> 
      <p><b>笔尖</b>:在为角色和选项分配批准时 <b>审批者不需要加入项目团队（对于包含角色的审批流程）</b> 已禁用，但项目团队中没有任何角色与审批时的角色相匹配，则审批会重新分配给项目所有者。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">禁用审批委托</td> 
      <td> <p>选择此选项可禁用系统中用户将批准委派给其他用户的功能。 选择此选项后，用于委派审批的选项将从Workfront中删除，并且任何现有的审批委派都将停止。</p> <p>有关在Workfront中委派批准的更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">委派批准请求</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在项目、任务或问题处于待批准状态时编辑自定义表单</td> 
      <td> <p>选择此选项可允许用户在处于“待批准”状态时编辑项目、任务和问题的自定义形式。 这是默认设置。</p> 
      <p>选择此选项时：</p> 
       <ul> 
       <li>当对象处于待批准状态时，所有批准者（以及有权编辑自定义表单的任何其他用户）都可以对自定义表单进行更改，而无论当前的批准路径或批准步骤如何。</li> 
       <li>在批准流程中对自定义表单所做的更改不会影响在更改之前做出的任何批准决策。</li> 
       <li> <p>对项目、任务或问题所做的任何更改都将以相同的方式进行跟踪，而无论此设置如何。 </p> <p>例如，如果您在更新流中添加了要跟踪的自定义表单字段，则会在对象的更新流中跟踪对表单所做的任何更改。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许用户撤消刚创建、等待批准的请求</td> 
      <td> <p>选择此选项可配置用户是否可以重新调用问题或请求以等待其首次状态的批准。 您可以通过配置请求队列，将问题或请求的第一个状态与批准流程关联。 </p> 
      <p>有关请求队列的更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>.</p> 
      <p>执行下列操作之一：</p> 
       <ul> 
       <li>选择此选项可允许用户重新调用对问题或请求的第一个状态的批准。 在这种情况下，他们可以看到新问题或请求中的“撤回”按钮，该按钮处于待批准状态。 当他们选择回顾问题时，将收到一则警告，指出该问题也将被删除。 在他们确认回访后，该问题即被删除。 </li> 
       <li> <p>取消选择此选项可阻止用户回顾其第一个状态为“等待批准”的问题或请求。 他们在新问题或请求中看不到“撤回”按钮，必须获得批准。 这是默认选项。</p> 
       <p>有关审核等待批准的项目的更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看批准 </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存更改。**
