---
product-area: projects
navigation-topic: manage-issues
title: 分配问题
description: 您可以将问题分配给用户、角色和团队，以指示负责完成问题的人员。 有关分配问题的一般信息，请参阅修改问题分配概述。
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 0%

---

# 分配问题

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第三季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

您可以将问题分配给用户、角色和团队，以指示负责完成问题的人员。 有关分配问题的一般信息，请参阅 [修改问题分配的概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
>
>如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则仍将其分配给工作项目。 在这种情况下，我们建议执行以下操作：
>
>* 将工作项重新分配给活动资源。
>* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

除了本文之外，我们建议您阅读以下文章，以了解有关分配问题的更多信息：

* [修改问题分配的概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [修改列表中多个问题的用户分配](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [在工作负载均衡器中分配工作概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

您可以在单个问题级别将问题分配给一个或多个资源，也可以一次性将多个资源分配给多个问题。

在Adobe Workfront中，分配问题和任务非常类似。 有关分配任务的一般信息，请参见 [修改任务分配的概览](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>向要复制问题的项目分配权限，并能够添加问题。</p> <p> 有关向问题授予权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">授予用户访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 向工作角色、团队和用户进行多个分配的注意事项

将多个资源分配给工作项时，请考虑以下事项：

* 用户可以有多个与其配置文件关联的工作角色。 有关将用户与工作角色关联的信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 任务或问题通常首先分配给一个或多个工作角色或团队。 当项目准备好开始时，可能需要将它们也分配给用户。

  如果已将任务或问题分配给一个或多个角色，并且您还分配了用户，则Adobe Workfront将根据以下规则确定要与其他用户（如果有）关联的工作角色：

   * 如果只分配了一个工作角色，并且该工作角色与用户的主要角色匹配，则任务或问题仅被分配给履行其主要角色的用户。
   * 如果分配了多个角色，并且至少有一个角色与用户的辅助角色匹配，则将任务或问题分配给履行其中一个其他角色(如果存在多个匹配，则Workfront会随机选择其他角色)以及分配的任何其他角色的用户。
   * 如果分配了一个或多个工作角色，但没有与用户的角色匹配，则任务或问题将同时分配给该角色和用户。

* 如果将任务或问题分配给团队并且您还分配了用户，则任务或问题仍会分配给团队和用户。

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
1. 单击 **分配给** 问题标题右上角的 **指定任务** 区域

   或

   如果问题已分配，单击当前分配的名称。

   ![“分配给”按钮](assets/assign-to-button-in-header.png)

1. 执行下列操作之一：

   * 开始键入要分配的用户、角色或团队的名称，然后当该名称出现在列表中时单击它。

     生产环境中的示例图像：
     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

     <span class="preview">“预览”环境中的示例图像：</span>
     ![任务搜索](assets/assignments-expanded-in-task-issue-header.png)

   * （视情况而定）单击 **建议的工作分配** 列表
   * 单击 **分配给我** 以将其分配给您自己
   * 单击 **高级**.

     创建高级工作分配的过程与任务和问题类似。 有关如何进行高级工作分配的信息，请参见 [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。
     >
     >用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
     >
     >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)


1. 单击 **保存** 以完成问题分配。
1. （可选）单击 **X图标** ，位于问题标题上任务区域中的任务名称旁以移除任务。

## 在列表中分配问题

当任何分配字段在列表视图中可见时，您可以在列表或报告中分配问题。 这是指派问题的更快方式。

根据视图中可见的字段，可以将以下实体分配给问题：

| 选项 | 分配的实体 |
|---|---|
| **分配给** | 分配一个用户 |
| **已指定** | 分配一个用户 |
| **分配** | 分配用户、工作角色或团队。 |

要在列表中分配问题，请执行以下操作：

1. 转到问题列表，该列表中具有“任务负责人”、“任务负责人”或“工作总揽”字段。
1. 要分配问题，请执行下列操作之一：

   * 在 **分派给** 或 **已指定** 开始键入要分配给问题的活动用户的名称，然后在列表中显示该用户时单击该用户。

     ![](assets/assigned-to-field-task-list-nwe.png)

   * 在 **指定任务** 字段中，开始键入要分配给问题的活跃用户、工作角色或活跃团队的名称，然后在列表中显示该问题时单击该名称。

     生产环境中的示例图像：
     ![](assets/assignments-field-task-list-nwe.png)

     <span class="preview">“预览”环境中的示例图像：</span>
     ![任务字段](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。
   >
   >用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
   >
   >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. （视情况而定）在“工作总揽”字段中可见时，单击 **“人员”图标** ![](assets/teams.png) 打开“高级任务”框并创建高级任务。 有关更多信息，请参阅 [创建高级工作](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >您不能从“分配至”或“已分配”字段进行高级分配。

1. 将您的代理人添加到问题中后，按Enter或单击页面上的任意位置以保存更改。

## 批量分配问题

1. 转到要批量分配的问题列表。
1. 选择列表中的多个问题。
1. 单击 **“编辑”图标** ![](assets/qs-edit-icon.png).

   此 **编辑问题** 对话框打开。

1. 在 **指定任务** 区域，选择 **被分派人** 框中，然后开始键入要分配给所有问题的用户、工作角色或团队的名称。

   >[!IMPORTANT]
   >
   >如果任何问题已分配，则您在此处指示的资源将添加到问题中，而不是替换问题中的现有资源。

1. （可选）选择 **问题所有者** 列，指明在将多个资源分配给问题时哪个资源是问题的主要被分配人或所有者。 这不适用于团队。
1. （可选）从中选择用户在问题中应履行的角色 **选择角色** 中的下拉菜单 **被分派人的角色** 列。 如果不选择角色，Workfront会自动选择用户的主要角色。

1. （可选）如果要从所有问题中删除现有被分配人，请执行下列操作之一：

   1. 开始键入要从问题中删除的用户、角色或团队的名称，然后当该名称出现在列表上时将其选中并单击 **移除被分派人** 以添加要删除的其他被分配人。
   1. 单击 **移除所有现有被分配人** 以从所有已选问题中移除所有被分配人。

1. 单击 **保存更改**.
1. （可选，视情况而定）当问题列表中显示分配至或分配字段时，单击其中一列以查找问题，然后单击 **X图标** ，以将其从问题中删除。
