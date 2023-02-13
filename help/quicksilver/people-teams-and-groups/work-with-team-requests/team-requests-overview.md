---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 团队请求概述
description: 团队请求位于主菜单的“团队”区域。
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 团队请求概述

## 了解团队请求

在 [!UICONTROL 团队] 区域 [!UICONTROL 主菜单]. 单击 [!UICONTROL 团队请求] 图标 ![“请求”图标](assets/request-icon.png) 在左侧面板中查看团队请求。

>[!NOTE]
>
>敏捷团队没有团队请求。

的 [!UICONTROL 团队请求] 选项卡显示当前在下拉列表中选定的团队的等待分配请求。 括号中的数字表示可以处理的项目数量。

团队请求表示未分配给特定用户的待处理工作项。 相反，它会被分配给一个团队，该团队的任何成员都可以自愿接受对该项目的责任。 如果用户自愿处理团队请求，则用户将接受作为他们自己的工作分配。 除团队之外，任务还会分配给单个用户。

>[!NOTE]
>
>协作任务分配不应使用团队请求。 如果需要分配多个用户以一起处理任务，请通过 [!UICONTROL 高级分配] 而不是通过团队请求。 有关更多信息，请参阅 [创建高级分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## 了解 [!UICONTROL 准备开始] 和 [!UICONTROL 全部] 选项

“团队请求”部分顶部有两个选项： [!UICONTROL 准备开始] 和 [!UICONTROL 全部].

的 [!UICONTROL 准备开始] 选项仅显示满足以下所有条件的任务和问题：

* 所有前任都满足其前任依赖类型的条件。\
   例如，如果前置关系的类型为 [!UICONTROL 完成开始] （前置任务必须在从属任务开始之前完成），前置任务必须标记为 [!UICONTROL 完成]. (有关上一任依赖关系类型的详细信息，请参阅 [任务依赖关系类型概述](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* 已登录的用户是分配给这些任务和问题（对于工作请求）的人员，或者将选定的团队分配给这些任务和问题（对于团队请求）。
* 项目状态为 [!UICONTROL 当前].
* 的 [!UICONTROL 预计开始日期] 或 [!UICONTROL 计划开始日期] 已过，或计划在今天日期后的两周内开始(或 [!UICONTROL 预计开始日期] 或 [!UICONTROL 计划开始日期] 已定义)。
* 的 [!UICONTROL 切换日期] 已经发生或将在当前日期后的两周内发生。

>[!NOTE]
>
>如果任务满足前三个条件，并且在当前日期后的两周内具有切换日期，则该任务将显示为 [!UICONTROL 准备开始] 即使计划/预计日期的间隔时间超过两周。 如果任务没有切换日期，则计划/预计日期必须在当前日期后的两周内。

的 [!UICONTROL 全部] 选项显示分配给已登录用户的当前项目的所有任务和问题，或分配给团队的所有任务或问题。
