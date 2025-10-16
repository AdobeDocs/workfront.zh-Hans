---
title: 项目常见问题解答
description: 本文包含有关Adobe Workfront中项目的最常见常见常见问题解答。
author: Alina
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# 项目常见问题解答

以下是有关项目的常见问题解答。

## 为什么在任务列表中右键单击任务时，会缺少“在上方插入任务”/“在下方插入任务”？

### 答案

要使用插入选项，任务列表必须按数字排序。 要按编号对列进行排序，请单击&#x200B;**任务名称**&#x200B;左侧的列标题中的&#x200B;**#**&#x200B;以按编号重新排序任务。

## 实际完成日期是多长时间？

### 答案

实际完成日期表示完成工作的日期和时间。 有关详细信息，请参阅[项目实际完成日期概览](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md)。

## 为什么缺少缩进/减少缩进按钮？

### 答案

要使用“缩进/减少缩进”按钮，请确保任务按任务编号排序，并且未应用分组。

## 为什么无法将项目状态更改为“完成”？

当我尝试将项目标记为完成时，收到以下错误消息：

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### 答案

如果项目中存在以下任何情况，则无法将项目的状态更改为“完成”：

* 未完成的任务或问题
* 处于未决批准状态的任务或问题

## 为什么无法将项目状态从完成更改为当前？

### 答案

如果项目的“完成模式”设置为“自动”，则一旦完成所有任务和问题，项目的状态就会自动变为“完成”，您无法将其修改为任何其他状态。 必须将项目的“完成模式”设置为“手动”，才能将完整项目转换为“当前”。 有关信息，请参阅[项目状态不会从完成更改为当前](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md)。

## 为什么无法将项目添加到Portfolio，尽管我有正确的权限执行此操作？

尽管我具有正确的权限，但Portfolio的“项目”选项卡上缺少“添加项目”按钮。

### 答案

这是由Portfolio状态为不活动导致的。 要更改Portfolio的状态，请执行以下操作：

1. 单击&#x200B;**Portfolio详细信息>概述**。
1. 将&#x200B;**状态**&#x200B;更改为&#x200B;**活动。**

1. 单击&#x200B;**保存**。\
   **添加项目**&#x200B;按钮现在应显示在&#x200B;**项目**&#x200B;选项卡上。

## 资源管理器在添加到项目时获得什么访问权限？

### 答案

资源管理器会自动获得对项目的管理访问权限。 从资源管理器角色中删除用户不会删除其“管理”共享访问权限。

## 添加组时，项目状态为何会更改？

### 答案

由于组的默认状态，项目状态发生了更改。 将组添加到项目时，项目组会将状态列表更改为为该组设置的默认状态。

有关详细信息，请参阅文章[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

## 预算状态是什么？

### 答案

预算状态将显示项目当前是否添加到Capacity Planner以及预算计算是否已完成。

预算状态如下：

* 未包括 — 项目未添加到能力规划者。
* 包括但未计算 — 项目已添加到Capacity Planner但已从预算计算中排除。
* 包括并计算 — 项目将添加到Capacity Planner并包含在预算计算中。

## 为什么我无法与团队共享我是其所有者且具有管理权限的项目？ 在项目的共享对话框中，我根本找不到该团队。

### 答案

Adobe Workfront管理员限制您仅查看您所属的您的访问级别中的公司、组和团队。 您正在寻找的团队不是您所属的团队之一。

![仅查看他们属于的团队、组和公司](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

有关允许用户查看系统中所有团队的信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
