---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 团队请求概述
description: 团队请求位于主菜单的团队区域。
author: Jenny
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 团队请求概述

## 了解团队请求

团队请求位于[!UICONTROL 主菜单]的[!UICONTROL 团队]区域。 单击左侧面板中的[!UICONTROL 团队请求]图标![请求图标](assets/request-icon.png)以查看团队请求。

>[!NOTE]
>
>Agile团队没有团队请求。

[!UICONTROL 团队请求]选项卡显示当前在下拉列表中选择的团队等待分配的请求。 括号中的数字表示准备处理的项目数。

团队请求表示未分配给特定用户的待处理工作项。 相反，它会被分配给一个团队，该团队的任何成员都可以自愿承担该项目的责任。 如果用户志愿为团队请求工作，则用户将接受作为自己的工作任务。 除了团队外，任务还会分配给个人用户。

>[!NOTE]
>
>团队请求不应用于协作任务分配。 如果您需要分配多个用户以一起处理一项任务，请通过[!UICONTROL 高级工作]而不是通过团队请求来执行此操作。 有关详细信息，请参阅[创建高级工作](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

## 了解[!UICONTROL 准备开始]和[!UICONTROL 全部]选项

团队请求部分的顶部有两个选项：[!UICONTROL 准备开始]和[!UICONTROL 全部]。

[!UICONTROL 准备开始]选项仅显示满足以下所有条件的任务和问题：

* 所有前置任务均已满足其前置任务依赖关系类型的条件。\
  例如，如果前置任务关系的类型为[!UICONTROL 完成 — 开始]（前置任务必须先完成，相关任务才能开始），则必须将前置任务标记为[!UICONTROL 完成]。 （有关前置任务依赖关系类型的详细信息，请参阅[任务依赖关系类型概述](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。）

* 登录用户是指派给这些任务和问题（对于工作请求）的人员，或者是指派给这些任务和问题（对于团队请求）的选定团队。
* 项目状态为[!UICONTROL 当前]。
* [!UICONTROL 预计开始日期]或[!UICONTROL 计划开始日期]已过期或计划在今天日期后的两周内开始（或未定义[!UICONTROL 预计开始日期]或[!UICONTROL 计划开始日期]）。
* [!UICONTROL 移交日期]已经发生或将在当前日期后的两周内发生。

>[!NOTE]
>
>如果任务满足前三个条件并且移交日期在当前日期的两周内，那么即使计划/预计日期超过两周，任务也会显示为[!UICONTROL 准备开始]。 如果任务没有移交日期，则计划/预计日期必须在当前日期的两周内。

[!UICONTROL 全部]选项显示当前项目中分配给登录用户的所有任务和问题，或分配给团队的所有任务或问题。
