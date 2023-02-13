---
product-area: projects
navigation-topic: manage-issues
title: 分配问题
description: 您可以向用户、角色和团队分配问题，以指明谁负责完成问题。 有关分配问题的常规信息，请参阅修改问题分配概述。
author: Alina
feature: Work Management
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 0%

---

# 分配问题

您可以向用户、角色和团队分配问题，以指明谁负责完成问题。 有关分配问题的一般信息，请参阅 [修改问题分配概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
>
>如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
>
>* 将工作项重新分配给活动资源。
>* 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


除了本文之外，我们建议您阅读以下文章以了解有关分配问题的更多信息：

* [修改问题分配概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [修改列表中多个问题的用户分配](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [工作负载平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

您可以在单个问题级别将问题分配给一个或多个资源，也可以一次将多个资源分配给多个问题。

分配问题和任务在Adobe Workfront中类似。 有关分配任务的一般信息，请参阅 [修改任务分配概述](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限访问项目和任务</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>对要复制问题的项目具有“添加问题”功能的参与权限。</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 对工作角色、团队和用户进行多种分配的注意事项

在为工作项分配多个资源时，请考虑以下事项：

* 用户可以拥有与其配置文件关联的多个作业角色。 有关将用户与作业角色关联的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 任务或问题通常首先分配给一个或多个作业角色或团队。 当项目准备好启动时，可能还需要将它们分配给用户。

   如果任务或问题被分配到一个或多个角色，然后您又分配了一个用户，则Adobe Workfront会根据以下规则确定要与附加用户关联的作业角色（如果有）：

   * 如果只分配了一个作业角色，并且该角色与用户的主角色相匹配，则该任务或问题将仅分配给执行其主角色的用户。
   * 如果分配了多个角色，并且其中至少一个角色与用户的辅助角色匹配，则任务或问题会分配给执行其中一个其他角色(如果存在多个匹配，Workfront将随机选择)的用户，以及分配的任何其他角色。
   * 如果分配了一个或多个作业角色，并且与用户的角色没有匹配，则任务或问题将分配给角色或角色以及用户。

* 如果任务或问题被分配给团队，并且您也分配了用户，则任务或问题仍会同时分配给团队和用户。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## 分配单个问题

1. 转到要分配的问题。
1. 单击 **分配给** 在问题标题的右上角， **分配** 面积

   或

   如果已分配问题，请单击当前分配的名称。

   ![](assets/nwe-assign-to-button-in-header-350x77.png)

1. 执行下列操作之一：

   * 开始键入要分配的用户、角色或团队的名称，然后在列表中显示该名称时单击该名称。

      ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

   * （视情况而定）单击 **建议的分配** 列表
   * 单击&#x200B;**分配给我** 把它分配给自己
   * 单击 **高级**

      创建高级分配与任务和问题类似。 有关如何进行高级分配的信息，请参阅 [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

      >[!TIP]
      >
      >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。


1. 单击 **保存** 完成问题的分配。
1. （可选）单击 **X图标** 在问题题头的“分配”区域中的分配名称旁边，以删除分配。

## 在列表中分配问题

当列表视图中显示任何分配字段时，您可以在列表或报表中分配问题。 这是分配问题的更快方法。

根据视图中显示的字段，您可以为问题分配以下实体：

| 选项 | 已分配的实体 |
|---|---|
| **分配给** | 分配一个用户 |
| **已分派** | 分配一个用户 |
| **分配** | 分配用户、工作角色或团队。 |

要在列表中分配问题，请执行以下操作：

1. 转到视图中具有“分配给”、“分配”或“分配”字段的问题列表。
1. 要分配问题，请执行以下操作之一：

   * 在 **分配给** 或 **已分配** 字段，然后开始键入要分配给问题的活动用户的名称，然后在列表中显示时单击该名称。

      ![](assets/assigned-to-field-task-list-nwe.png)

   * 在 **分配** 字段，然后开始键入要分配给问题的活动用户、作业角色或活动团队的名称，然后在列表中显示时单击该名称。

      ![](assets/assignments-field-task-list-nwe.png)
   >[!TIP]
   >
   >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。


1. （视情况而定）当在“工作总揽”(Assignments)字段中显示时，单击 **“人员”图标** ![](assets/teams.png) 在“工作总揽”(Assignments)框的右上角，打开“高级工作总揽”(Advanced Assignments)框并创建高级工作总揽。 有关更多信息，请参阅 [创建高级分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >您不能从“已分配给”或“已分配”字段进行高级分配。

1. 在将受分配人添加到问题后，按Enter键或单击页面上的任意位置以保存更改。

## 批量分配问题

1. 转到要批量分配的问题列表。
1. 在列表中选择几个问题。
1. 单击 **“编辑”图标** ![](assets/qs-edit-icon.png).

   的 **编辑问题** 对话框。

1. 在 **分配** 区域，选择 **被分派人** ，然后开始键入要分配给所有问题的用户、作业角色或团队的名称。

   >[!IMPORTANT]
   >
   >如果已分配任何问题，则会将您在此处指示的资源添加到问题中，而不是替换问题上的现有资源。

1. （可选）选择 **问题所有者** 列来指示在为问题分配多个资源时，哪个资源是主要被分派人或问题的所有者。 这不适用于团队。
1. （可选）从 **选择角色** 下拉菜单(位于 **被分派人的角色** 列。 如果未选择角色，Workfront会自动选择用户的主角色。

1. （可选）如果要从所有问题中删除现有受分配者，请执行以下操作之一：

   1. 开始键入要从问题中删除的用户、角色或团队的名称，然后在列表中显示该名称时将其选中，然后单击 **删除被分派人** 添加其他要删除的受分配人。
   1. 单击 **删除所有现有的受分配人** 从所有选定问题中删除所有受分配者。

1. 单击 **保存更改**.
1. （可选和视情况而定）当“已分配给”或“分配”字段显示在问题列表中时，单击问题的这些列之一，然后单击 **X图标** 将其从问题中删除的代理人名称旁边。
