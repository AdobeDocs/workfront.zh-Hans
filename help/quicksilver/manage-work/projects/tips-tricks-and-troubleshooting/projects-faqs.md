---
title: 项目常见问题解答
description: 项目常见问题解答
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# 项目常见问题解答

以下是有关项目的常见问题解答。

## 为什么右键单击任务列表中的任务时，“在上面/下面插入任务”缺失？

### 回答

要使用插入选项，任务列表必须按数字排序。 要按数字对列进行排序，请单击 **#** 列标题中的 **任务名称** 按号度任务。

## 实际完成日期是多少？

### 回答

实际完成日期表示完成工作的日期和时间。 有关更多信息，请参阅 [项目实际完成日期概览](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## 为什么缺少缩进/凹出按钮？

### 回答

要使用缩进/凸出按钮，请确保按任务编号对任务进行排序，并且未应用分组。

## 为何无法将项目状态更改为“完成”？

尝试将项目标记为完成时，我收到以下错误消息：

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### 回答

如果您的项目具有以下任一项，则无法将项目的状态更改为完成：

* 任务或问题未完成
* 处于待批准状态的任务或问题

## 为什么无法将项目状态从“完成”更改为“当前”？

### 回答

如果项目将“完成模式”设置为“自动”，则完成所有任务和问题后，项目状态将自动变为“完成”，您无法将其修改为任何其他状态。 项目的“完成”模式必须设置为“手动”才能将完整项目转换为“当前”。 有关信息，请参阅 [项目状态不会从“完成”更改为“当前”](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## 尽管我拥有执行此操作的正确权限，但为何我无法将项目添加到Portfolio?

尽管我拥有正确的权限，但Portfolio的“项目”选项卡上缺少“添加项目”按钮。

### 回答

这是由“Portfolio状态”为“不活动”导致的。 要更改Portfolio的状态，请执行以下操作：

1. 单击 **Portfolio详细信息>概述**.
1. 更改 **状态** to **活动。**

1. 单击&#x200B;**保存**。\
   的 **添加项目** 按钮应该可在 **项目** 选项卡。

## 资源管理器在添加到项目后会获得什么访问权限？

### 回答

资源管理器会自动接收对项目的管理访问权限。 从资源管理器角色中删除用户不会删除其管理共享访问权限。

## 为什么在添加群组时项目状态会发生更改？

### 回答

项目状态会因组的默认状态而发生更改。 在将群组添加到项目时，它会将状态列表更改为为群组设置的默认状态。

有关更多信息，请参阅文章 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 什么是预算状态？

### 回答

预算状态将显示项目当前是否已添加到能力计划员，以及是否已完成预算计算。

以下是预算状态：

* 未包含 — 项目未添加到能力计划器。
* 已包括但未计算 — 项目将添加到能力计划员，但从预算计算中排除。
* 已包括和已计算 — 项目将添加到能力计划员并包含在预算计算中。

## 为什么我无法与团队共享我是其所有者且我在其中拥有管理权限的项目？ 我在项目的共享对话框中找不到团队。

### 回答

Adobe Workfront管理员限制您仅查看您在的访问级别中所属的公司、组和团队。 您要查找的团队不是您所属的团队之一。

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

有关允许用户查看系统中所有团队的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
