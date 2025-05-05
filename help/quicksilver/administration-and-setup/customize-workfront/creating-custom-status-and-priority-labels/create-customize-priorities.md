---
title: 创建和自定义优先级
description: 您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级重视Adobe Workfront中的项目、任务或问题。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 2%

---

# 创建并自定义优先级

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级重视Adobe Workfront中的项目、任务或问题。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td>
     <p>新增：标准</p>
     <p>或</p>
     <p>当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义现有优先级

作为Workfront管理员，您可以对Workfront中提供的默认优先级进行以下修改：

* 重命名优先级。
* 对优先级重新排序。

  有关如何对优先级重新排序的详细信息，请参阅[为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

* 更改默认优先级。

  有关更改默认优先级的功能的详细信息，请参阅[为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

* 编辑优先级描述。
* 为每个优先级设置一种颜色。

  当您按&#x200B;**优先级**&#x200B;对结果进行分组时，会在图表报告中使用优先级的颜色。

  有关图表报表的详细信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 删除优先级。

  删除现有优先级时，必须选择一个替换优先级。

* 隐藏优先级。

  有关隐藏优先级功能的详细信息，请参阅[为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

  >[!NOTE]
  >
  >在Workfront帐户中，每个对象必须至少具有一个优先级。

默认情况下，为每个对象类型（项目、任务和问题）提供的优先级相同：

* 无
* 低
* 正常
* 高
* 紧急

## 为项目任务或问题创建优先级 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront中提供的默认优先级之外，您还可以添加自己的优先级以反映组织的需求。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项** > **优先级**。

1. 单击您要为（**项目**、**任务**&#x200B;或&#x200B;**问题**）创建优先级的对象类型的选项卡。
1. 单击&#x200B;**添加新优先级**。
1. 为新优先级指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">优先级名称</td> 
      <td>键入优先级名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要性</td> 
      <td> <p>添加新优先级时，默认情况下会为其分配一个数字。 如果该数字与您的需求不匹配，请编辑该数字。</p> <p>对于您选择的对象，每个优先级的<strong>重要性</strong>编号必须是唯一的。<br>优先级的数量反映了项目、任务或问题的重要性：最高优先级对应于最高优先级。</p> <p><b>注意</b>：保存优先级后，无法编辑重要性数字。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>为您的优先级选择一种颜色。</p> <p>优先级的颜色在图表报表和“敏捷团队设置”中使用。 有关图表报表的详细信息，请参阅<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">将图表添加到报表</a>。</p> <p>有关Agile团队设置的更多信息，请参阅中的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认优先级</td> 
      <td> <p>通过选择单选按钮，确定此优先级是否应为默认优先级。</p> <p>如果将某个优先级指定为<strong>默认优先级</strong>，则会自动为Workfront中的所有项目、任务或问题选择该优先级。 <strong>普通</strong>是Workfront中所有对象的默认优先级。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>添加优先级说明以解释其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐藏</td> 
      <td> <p>如果要隐藏优先级，请选择此框。</p><p>选择<b>隐藏</b>选项时，优先级不会在Workfront中的任何位置显示，用户无法为其项目、任务和问题选择它。</p> 
      <p><b>重要信息</b>：我们建议您隐藏不想再使用的优先级，而不是删除它们。 通过隐藏它们，您仍然可以保留所有历史数据，以及已使用此优先级完成的对象，同时阻止人们将来选择此优先级。 </p>
      <p>（可选）您可以通过按所需顺序拖放优先级来更改优先级列表顺序。 这会更改它们在项目、任务和问题中的显示顺序。 这不会更改<b>重要性</b>数字。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

有关将优先级应用于项目、任务和问题的说明，请参阅以下文章：

* [了解并更新项目优先级](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任务优先级](../../../manage-work/tasks/task-information/task-priority.md)
* [更新问题优先级](../../../manage-work/issues/issue-information/update-issue-priority.md)
