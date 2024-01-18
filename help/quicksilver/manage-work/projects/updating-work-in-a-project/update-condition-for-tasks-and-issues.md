---
product-area: projects
navigation-topic: update-work-in-a-project
title: 任务和问题的更新条件
description: 任务或问题的完成情况是指在任务或问题上放置一个指示其运行方式的标志。 这与工作项的状态不同，后者指示项目开发的当前阶段。
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# 任务和问题的更新条件

任务或问题的完成情况是指在任务或问题上放置一个指示其运行方式的标志。 这与工作项的状态不同，后者指示项目开发的当前阶段。

您可以自动或手动设置任务或问题的条件。

Adobe Workfront管理员可以为您的环境创建自定义条件，如中所述 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

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

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 找到任务和问题的状况

条件显示为与任务或问题关联的标记。 它们还可以与显示在报告中的数字相关联，而不是与标签关联。 有关将条件与数字关联的更多信息，请参见 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

您可以在以下区域找到任务和问题的状况：

* 当您被分配到任务或问题时，更新中的任务和问题更新区域。 新的评论体验不支持此功能。 有关信息，请参阅 [新的评论体验](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
* 在视图或分组中显示Condition字段时报告和列表。

>[!NOTE]
>
>当“条件”一词显示在“日记帐条目”报表的“字段名称”字段中时，这表示已更新项目的条件。 在日记帐分录报表中跟踪“条件”字段时，“新值”和“旧值”将显示与条件关联的编号，而不是其名称。 如果最初没有为任务或问题定义条件，而您稍后更新了它，则捕获更新的日记帐条目会将“条件”字段的“旧编号值”显示为 — 2,147,483,648。

## 通过更新状态自动更新条件

当您分配了任务或问题并且单击 **处理此项工作** ，启动任务或启动问题，或更新其状态，任务或问题的条件自动更改为与关联的默认条件 **进展顺利**.

有关使用自定义条件作为默认条件的信息，请参阅相关文章  [将自定义条件设置为任务和问题的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) 和 [将自定义条件设置为项目的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

有关更改任务状态的信息，请参见 [更新任务状态](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

有关更改问题状态的信息，请参阅 [更新问题状态](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

有关将“处理此项工作”按钮设置为“启动任务”或“启动问题”按钮的信息，请参阅 [将“处理此项工作”按钮替换为“开始”按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## 手动更新条件

您必须已分配至任务或问题，或拥有任务或问题的管理权限才能为其设置条件。

在视图中显示“条件”字段时，您可以在任务、问题报告或列表中手动更新任务或问题的条件。


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

要手动更新任务或问题的完成情况，请执行以下操作：

1. 转到您拥有管理权限的任务或问题列表。 确保 **条件** 字段在列表的视图中可见。

1. 更新 **条件** ，方法是双击现有条件并从下拉菜单中选择一个新值。

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >可以为您的环境自定义条件，因此您可能会在环境中找到三个以上的条件选项。 条件的名称可能与上面列出的名称不同。 有关在Workfront中自定义条件的信息，请参阅 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. 按 **输入** ，或单击条件字段外部以保存新任务或问题条件。

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
