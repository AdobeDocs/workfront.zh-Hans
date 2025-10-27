---
title: 创建和自定义优先级
description: 您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级重视Adobe Workfront中的项目、任务或问题。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 5706ebd11985b9e67c93686918f8f0327adabdf1
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%

---

# 创建并自定义优先级

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用，正在分阶段发布到生产环境。</span>

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

您可以在Workfront的“设置”区域中控制项目、任务和问题的优先级。 优先级重视Adobe Workfront中的项目、任务或问题。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义现有优先级

作为Workfront管理员，您可以对Workfront中提供的默认优先级进行以下修改：

* 重命名优先级。
* 对优先级重新排序。

  有关如何对优先级重新排序的详细信息，请参阅[为项目、任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

* 更改默认优先级。

  有关更改默认优先级的功能的详细信息，请参阅[为项目、任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

* 编辑优先级描述。
* 为每个优先级设置一种颜色。

  当您按&#x200B;**优先级**&#x200B;对结果进行分组时，会在图表报告中使用优先级的颜色。

  有关图表报表的详细信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 删除优先级。

  删除现有优先级时，必须选择一个替换优先级。

* 隐藏优先级。

  有关隐藏优先级功能的详细信息，请参阅[为项目、任务或问题创建优先级](#create-a-priority-for-a-project-task-or-issue)。

  >[!NOTE]
  >
  >在Workfront帐户中，每个对象必须至少具有一个优先级。

默认情况下，为每个对象类型（项目、任务和问题）提供的优先级相同：

* 无
* 低
* 正常
* 高
* 紧急

## 为项目、任务或问题创建优先级 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront中提供的默认优先级之外，您还可以添加自己的优先级以反映组织的需求。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项** > **优先级**。

1. 单击您要为（**项目**、**任务**&#x200B;或&#x200B;**问题**）创建优先级的对象类型的选项卡。
1. 单击表&#x200B;<span class="preview">**底部的**&#x200B;新行</span>，或单击&#x200B;**添加新优先级**。
1. 为优先级配置以下选项：

   * **优先级名称**：键入优先级名称。
   * **重要性**：添加新优先级时，默认情况下会为其分配一个数字。 如果该数字与您的需求不匹配，请编辑该数字。

     每个优先级的重要性数字必须是唯一的。 优先级的数量反映了项目、任务或问题的重要性：最高优先级对应于最高优先级。

     保存优先级后，无法编辑此数字。

   * **颜色**：选择优先级的颜色。

     优先级的颜色在图表报表和“敏捷团队设置”中使用。 有关图表报表的信息，请参阅[将图表添加到报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。 有关Agile团队设置的信息，请参阅[创建Agile团队](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)。

   * **默认优先级**：选择您希望Workfront自动应用于所有新创建的项目、任务或问题的优先级。

     **普通**&#x200B;是Workfront中所有对象的默认优先级。

     您不能将隐藏优先级设置为默认值。

     <div class="preview">

     默认优先级以图标![默认优先级图标](assets/default-icon.png)指示。 要选择新的缺省值，请执行下列操作之一：

      * 选中优先级名称旁边的复选框，然后在屏幕底部的操作栏中选择&#x200B;**设为默认值**。
      * 将鼠标悬停在优先级名称上，然后单击显示的&#x200B;**更多**&#x200B;菜单。 然后，选择&#x200B;**设为默认值**。

        新的默认优先级使用图标进行标记。

     </div>

   * **描述**：键入优先级描述以说明其功能。
   * <span class="preview">**隐藏选择**</span>&#x200B;或&#x200B;**隐藏**： <span class="preview">选择&#x200B;**是**</span>&#x200B;或选中此复选框以隐藏不再需要的优先级。

     隐藏的优先级不会在Workfront的任何位置显示，因此用户无法为其项目、任务或问题选择它。

     >[!IMPORTANT]
     >
     >我们建议您隐藏这些优先级，而不是删除您不再想要使用的优先级。 这样，您就可以保留已使用优先级完成的对象上的所有历史数据，同时防止他人将来使用优先级。

1. （可选）通过按所需的顺序拖放优先级，以更改优先级的列表顺序。

   这会更改项目、任务或问题的显示顺序。 它不会更改&#x200B;**重要性**&#x200B;数字。

1. 单击&#x200B;**保存**。

有关将优先级应用于项目、任务和问题的说明，请参阅以下文章：

* [了解并更新项目优先级](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任务优先级](../../../manage-work/tasks/task-information/task-priority.md)
* [更新问题优先级](../../../manage-work/issues/issue-information/update-issue-priority.md)
