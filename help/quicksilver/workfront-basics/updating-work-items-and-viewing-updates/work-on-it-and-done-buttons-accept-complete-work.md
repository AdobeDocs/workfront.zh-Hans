---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 处理此项工作并完成按钮概述
description: 当您被分配到任务或问题时，您可以使用上下文按钮，该按钮会根据您参与工作项目的情况更改名称和功能。
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: a634e29df16d401812fb87ea53521d5028f7fd20
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# 处理此项工作并完成按钮概述

当您被分配到任务或问题时，您可以使用上下文按钮，该按钮会根据您参与工作项目的情况更改名称和功能。

使用上下文按钮接受或完成工作项，您可以让Adobe Workfront更新工作项上的多个字段，而无需自己手动更新。

## 处理它和“完成”按钮名称

根据您从哪个Workfront区域访问您的任务或问题，“处理它”或“完成”按钮可以更改名称，如以下场景中所述： 

* 当任务或问题首次分配给您并且状态为“新建”时，按钮显示为处理它。

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >您可以将“处理此项工作”按钮替换为“开始”按钮。 有关将“处理此项工作”按钮替换为“开始”按钮的信息，请参阅  [将“处理此项工作”按钮替换为“开始”按钮](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* 单击处理它接受后，按钮更改为标记为完成或完成，具体取决于您在Workfront中访问任务或问题的位置。 有关可在何处访问此项工作按钮的信息，请参阅部分 [找到“处理此项工作并完成”按钮](#locate-the-work-on-it-and-done-button) 本文章中。

  ![](assets/nwe-mark-as-done-button-350x122.png)

* 如果您不是唯一一个分配到任务或问题的用户，并且您正在从“主页”区域的“工作列表”访问您的工作项，则该按钮将变为“完成我的部件”。

  ![](assets/home-left-done-with-my-part-button-350x184.png)

## 找到“处理此项工作并完成”按钮 {#locate-the-work-on-it-and-done-button}

您可以在Workfront的以下区域中找到“处理它并完成”按钮：

* 主页区域，在工作列表或详细信息面板中

  有关在“主页”区域中将项目标记为“完成”的信息，请参阅 [在主区域将项目标记为完成](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* 在任务或问题的标题中

  有关对象标题的信息，请参见 [新对象标头](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* 在任务或问题列表或工作负载均衡器的“摘要”面板中

  有关使用“摘要”面板的信息，请参阅 [摘要概述](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## 单击“处理它并完成”按钮时自动更新的字段概述

使用“处理它和完成”按钮的好处是，您可以允许Workfront自动更新分配给您的工作项的信息。

* [处理此项工作按钮](#work-on-it-button)
* [“开始”按钮](#start-button)
* [“完成”按钮](#the-done-button)

### 处理此项工作按钮 {#work-on-it-button}

单击处理它时，以下项目也会更新：

* 分配状态更新从“已请求”到“正在工作”

  >[!TIP]
  >
  >“工作分配状态”字段仅在报告和列表中可见。 有关“分配状态”字段的信息，请参见 [Adobe Workfront术语表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* 提交日期

  有关提交日期的信息，请参见 [提交日期概述](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### “开始”按钮 {#start-button}

如果您有权编辑团队，则可以将“处理它”按钮替换为团队的“开始”按钮。 当以该团队作为其主团队的用户单击关于他们被分配到的项目的“开始”按钮时，其工作项目上的其他字段自动更新。 有关将“处理此项工作”按钮替换为“开始”按钮的信息，请参阅 [将“处理此项工作”按钮替换为“开始”按钮](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

除了在单击处理它按钮时更新的字段外，在单击开始按钮时，以下字段会自动更新任务或问题：

* 状态
* 实际开始日期

  有关实际开始日期的信息，请参阅 [项目实际开始日期概览](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* 实际完成日期（如果“开始”按钮与等于“完成”或“已关闭”的状态相关联）。

  有关实际完成日期的信息，请参阅 [项目实际完成日期概览](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>单击“撤消”按钮会将工作项返回到原始状态并删除实际开始日期。
>
>“撤消”按钮在以下区域不可用：
>
>* 团队请求
>* 任务标题
>

### “完成”按钮 {#the-done-button}

如果您有权编辑团队，则可以配置团队的“完成”按钮，以便在将项目标记为完成时更新任务或问题状态。 当将该团队作为其主团队的用户单击其项目上的完成按钮时，以下字段自动更新任务或问题：

* 状态
* 工作分配状态更新从“正在处理”到“已完成”
* 实际完成日期

有关为团队配置“完成”按钮的信息，请参阅以下文章：

* [为任务配置完成按钮](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [为问题配置“完成”按钮](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
