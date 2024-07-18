---
product-area: projects
navigation-topic: update-work-in-a-project
title: 任务和问题的更新条件
description: 任务或问题的完成情况是指在任务或问题上放置一个指示其运行方式的标志。 这与工作项的状态不同，后者指示项目开发的当前阶段。
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# 任务和问题的更新条件

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">有关当前版本的信息，请参阅[2024年第三季度版本概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)。</span>

任务或问题的完成情况是指在任务或问题上放置一个指示其运行方式的标志。 这与工作项的状态不同，后者指示项目开发的当前阶段。

您可以自动或手动设置任务或问题的条件。

默认情况下，我们在此文章中引用的条件值在Workfront中可用。 Adobe Workfront管理员可以为您的环境创建自定义条件，如[创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)中所述。

## 访问要求 {#access-requirements}

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>

对于新许可证：
<ul><li><p>任务标准</p></li>
   <li><p>问题的投稿人或更高版本</p></li></ul>


对于当前许可证：
<ul><li><p>任务的工作或更高</p></li>
   <li><p>有问题的请求或更高版本</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p> <p>编辑对任务和问题的访问权限 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务或问题的或更高权限以查看其完成情况</p>
   <p>管理任务和问题的权限以更新条件</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

您必须分配到任务或问题才能手动更新其条件。

## 找到任务和问题的状况

条件显示为与任务或问题关联的标记。 它们还可以与显示在报告中的数字相关联，而不是与标签关联。 有关将条件与数字关联的更多信息，请参阅[创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。

您可以在Workfront的以下区域找到任务和问题的完成情况：

* <span class="preview">在Workfront或组管理员将其添加到您的布局模板后，显示详细信息页面。 有关信息，请参阅[使用布局模板自定义详细信息视图](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。</span>

* <span class="preview">Workfront或组管理员将任务或问题的标题添加到您的布局模板后。 有关信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。</span>

* 在Workfront或组管理员将其添加到您的布局模板后，显示“摘要”面板。 有关信息，请参阅[使用布局模板自定义主页和摘要](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。

* 在视图或分组中显示Condition字段时报告和列表。

  >[!NOTE]
  >
  >当“条件”一词显示在“日记帐条目”报表的“字段名称”字段中时，这表示已更新项目的条件。 在日记帐分录报表中跟踪“条件”字段时，“新值”和“旧值”将显示与条件关联的编号，而不是其名称。 如果最初没有为任务或问题定义条件，而您稍后更新了它，则捕获更新的日记帐条目会将“条件”字段的“旧编号值”显示为 — 2,147,483,648。

## 通过更新状态自动更新条件

当您分配了任务或问题并且单击&#x200B;**处理它** 、开始任务或开始问题，或更新其状态时，任务或问题的条件会自动更改为与&#x200B;**顺利进行**&#x200B;关联的默认条件。

有关将自定义条件用作默认条件的信息，请参阅以下文章： [将自定义条件设置为任务和问题的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)和[将自定义条件设置为项目的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)。

有关更改任务状态的信息，请参阅[更新任务状态](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md)。

有关更改问题状态的信息，请参阅[更新问题状态](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md)。

有关将“处理此项工作”按钮设置为“开始任务”或“开始问题”按钮的信息，请参阅[将处理此项工作按钮替换为“开始”按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)。

## 手动更新条件

您必须已分配至任务或问题，或拥有任务或问题的管理权限才能为其设置条件。

在视图中显示“条件”字段时，您可以在任务、问题报告或列表中手动更新任务或问题的条件。

>[!NOTE]
>
>您可以要求系统或组管理员将条件字段添加到摘要面板，使其更易于在Workfront的各个区域中进行更新。
>
>有关更多信息，请参阅以下文章：
>
>* [摘要概述](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [使用布局模板自定义主页和摘要](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

要手动更新任务或问题的完成情况，请执行以下操作之一：

<div class="preview">

1. 要在任务或问题标题中更新任务或问题的条件，请执行以下操作：

   1. （视情况而定）如果您的Workfront或组管理员将“条件”字段添加到布局模板的任务或问题标题中，请单击标题中的&#x200B;**条件**&#x200B;字段，然后从以下选项中进行选择：
      * 进展顺利
      * 一些问题
      * 主要障碍

      ![](assets/condition-in-task-header.png)
   1. 单击Enter以保存条件。

1. 要在任务或问题详细信息部分中更新任务或问题的完成情况，请执行以下操作：

   1. （视情况而定）如果您的Workfront或组管理员将“条件”字段添加到布局模板中任务或问题的详细信息部分，请单击左侧面板中的&#x200B;**详细信息**，然后单击&#x200B;**任务条件**&#x200B;或&#x200B;**问题条件**，然后从以下选项中进行选择：
      * 进展顺利
      * 一些问题
      * 主要障碍
1. 单击&#x200B;**保存更改**。 任务或问题的完成情况已更新。

</div>

要更新报告或列表中的任务或问题的条件，请执行以下操作：

1. 转到您拥有管理权限的任务或问题列表。 确保&#x200B;**条件**&#x200B;字段在列表视图中可见。

1. 通过双击现有条件并从下拉菜单中选择新值，更新问题或任务内联的&#x200B;**条件**。

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >可以为您的环境自定义条件，因此您可能会在环境中找到三个以上的条件选项。 条件的名称可能与上面列出的名称不同。 有关在Workfront中自定义条件的信息，请参阅[创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。


1. 在键盘上按&#x200B;**Enter**，或在“条件”字段外部单击以保存新任务或问题条件。

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


