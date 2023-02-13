---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: “处理并完成”按钮概述
description: 当您被分配到任务或问题时，可以使用上下文按钮，根据您对工作项的参与情况更改名称和功能。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# “处理并完成”按钮概述

当您被分配到任务或问题时，可以使用上下文按钮，根据您对工作项的参与情况更改名称和功能。

使用上下文按钮接受或完成工作项，您可以让Adobe Workfront更新这些项目上的多个字段，而无需您自己手动更新它们。

## 处理该按钮和完成按钮名称

根据您从哪个Workfront区域访问任务或问题，“处理任务”或“完成”按钮可以更改名称，如以下情景中所述： 

* 当任务或问题首次分配给您且状态为“新建”时，按钮将显示为“处理”。

   ![](assets/nwe-work-on-it-button.png)

   >[!TIP]
   >
   >您可以将“Work On It（处理它）”按钮替换为“Start（开始）”按钮。 有关将“Work On It（处理）”按钮替换为“Start（开始）”按钮的信息，请参阅  [将“Work On It（处理它）”按钮替换为“Start（开始）”按钮](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* 单击“Work On It Accept”（对其进行工作接受）后，按钮将更改为“Mark as done”（标记为完成）或“Done”（完成），具体取决于您在Workfront中访问任务或问题的位置。 有关在何处可以访问Work On It按钮的信息，请参阅部分 [找到“完成并完成”按钮](#locate-the-work-on-it-and-done-button) 在本文中。

   ![](assets/nwe-mark-as-done-button-350x122.png)

* 如果您不是分配给任务或问题的唯一一个，并且您正在从“主页”(Home)区域的“工作列表”(Work List)中访问您的工作项，则按钮将更改为“使用我的部件完成”(Done with my part)。

   ![](assets/home-left-done-with-my-part-button-350x184.png)

## 找到“完成并完成”按钮 {#locate-the-work-on-it-and-done-button}

您可以在Workfront的以下区域中找到对其执行的工作和完成按钮：

* “主页”区域，位于“工作列表”或“详细信息”面板中

   有关在“主页”区域将项目标记为“完成”的信息，请参阅 [在“主页”区域中将项目标记为“完成”](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* 在任务或问题的标题中

   有关对象标头的信息，请参阅 [新对象标头](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* 在列表或负载平衡器的任务或问题摘要面板中

   有关使用“摘要”面板的信息，请参阅 [概要概述](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## 单击“处理并完成”按钮时自动更新的字段概述

使用Work On It（处理它）和Done（完成）按钮的好处是您可以允许Workfront自动更新分配给您的工作项目的信息。

* [“处理It”按钮](#work-on-it-button)
* [“开始”按钮](#start-button)
* [“完成”按钮](#the-done-button)

### “处理It”按钮 {#work-on-it-button}

单击“处理它”后，以下项目也会更新：

* 分配状态从“请求”更新为“工作”

   >[!TIP]
   >
   >“分配状态”字段仅在报表和列表中可见。 有关“分配状态”字段的信息，请参阅 [Adobe Workfront术语表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* 提交日期

   有关提交日期的信息，请参阅 [提交日期概述](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### “开始”按钮 {#start-button}

如果您有权编辑团队，则可以将“Work On It”（处理团队）按钮替换为团队的“Start”（开始）按钮。 当将该团队作为其主团队的用户单击他们分配到的项目上的“开始”按钮时，其工作项目上的其他字段会自动更新。 有关将“Work On It（处理）”按钮替换为“Start（开始）”按钮的信息，请参阅 [将“Work On It（处理它）”按钮替换为“Start（开始）”按钮](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

除了在单击“Work on It”（处理它）按钮时更新的字段外，在单击“Start”（开始）按钮时，以下字段还会自动更新任务或问题：

* 状态
* 实际开始日期

   有关实际开始日期的信息，请参阅 [项目实际开始日期概览](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* 实际完成日期（如果“开始”按钮与等于“完成”或“关闭”的状态关联）。

   有关实际完成日期的信息，请参阅 [项目实际完成日期概览](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>单击“撤消”按钮可将工作项返回到原始状态并删除实际开始日期。
>
>“撤消”按钮在以下区域中不可用：
>
>* 团队请求
>* 任务标题
>


### “完成”按钮 {#the-done-button}

如果您有权编辑团队，则可以为团队配置完成按钮，以在将项目标记为已完成时更新任务或问题状态。 当将该团队作为其主团队的用户单击项目上的完成按钮时，以下字段会自动更新任务或问题：

* 状态
* 分配状态从“工作”更新为“完成”
* 实际完成日期

有关为团队配置完成按钮的信息，请参阅以下文章：

* [为任务配置完成按钮](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [针对问题配置完成按钮](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
