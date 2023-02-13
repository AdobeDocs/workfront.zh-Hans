---
title: 创建和自定义优先级
description: 您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级会重视Adobe Workfront中的项目、任务或问题。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 创建和自定义优先级

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级会重视Adobe Workfront中的项目、任务或问题。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义现有优先级

作为Workfront管理员，您可以对Workfront中提供的默认优先级进行以下修改：

* 重命名优先级。
* 重新排序优先级。

   有关如何重新排序优先级的更多信息，请参阅 [为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue).

* 更改默认优先级。

   有关更改默认优先级的功能的更多信息，请参阅 [为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue).

* 编辑优先级的描述。
* 为每个优先级设置一种颜色。

   在按 **优先级**.

   有关图表报表的详细信息，请参阅 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 删除优先级。

   删除现有优先级时，必须选择替换优先级。

* 隐藏优先级。

   有关隐藏优先级的功能的更多信息，请参阅 [为项目任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >每个对象的Workfront帐户中必须至少具有一个优先级。

默认情况下，为每个对象类型（项目、任务和问题）提供的优先级是相同的：

* 无
* 低
* 正常
* 高
* 紧急

## 为项目任务或问题创建优先级 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront中提供的默认优先级之外，您还可以添加自己的优先级以反映贵组织的需求。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **项目首选项** > **优先事项**.

1. 单击要为(**项目**, **任务**&#x200B;或 **问题**)。
1. 单击 **添加新优先级**.
1. 为新优先级指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">优先级名称</td> 
      <td>键入您的优先级名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要性</td> 
      <td> <p>添加新优先级时，会默认为其分配一个数字。 如果此数字与您的需求不匹配，请编辑此数字。</p> <p>的 <strong>重要性</strong> 对于您选择的对象，每个优先级的编号必须是唯一的。<br>优先级数反映了项目、任务或问题的重要性：最高值对应于最高优先级。</p> <p><b>注意</b>:保存优先级后，便无法编辑重要性编号。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>选择颜色作为优先级。</p> <p>图表报表和“敏捷团队设置”中使用优先级的颜色。 有关图表报表的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">将图表添加到报表</a>.</p> <p>有关敏捷团队设置的更多信息，请参阅中的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认优先级</td> 
      <td> <p>通过选择单选按钮，确定是否应将此设置为默认优先级。</p> <p>如果优先级被指定为 <strong>默认优先级</strong>，则会自动为Workfront中的所有项目、任务或问题选取该参数。 <strong>正常</strong> 是Workfront中所有对象的默认优先级。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>为您的优先级添加描述以解释其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐藏</td> 
      <td> <p>如果要隐藏优先级，请选中此框。</p><p>当您选择 <b>隐藏</b> 选项，则优先级不会在Workfront中的任意位置显示，并且用户无法为其项目、任务和问题进行选择。</p> 
      <p><b>重要信息</b>:我们建议您隐藏不再希望使用的优先级，而不是删除它们。 通过隐藏这些数据，您仍然可以保留所有历史数据，以及已使用此优先级完成的对象，同时防止将来人们选择此优先级。 </p>
      <p>（可选）您可以通过按所需顺序拖放优先级来更改优先级的列表顺序。 这会更改项目、任务和问题的显示顺序。 这不会更改 <b>重要性</b> 数字。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

有关将优先级应用于项目、任务和问题的说明，请参阅以下文章：

* [了解和更新项目优先级](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任务优先级](../../../manage-work/tasks/task-information/task-priority.md)
* [更新问题优先级](../../../manage-work/issues/issue-information/update-issue-priority.md)
