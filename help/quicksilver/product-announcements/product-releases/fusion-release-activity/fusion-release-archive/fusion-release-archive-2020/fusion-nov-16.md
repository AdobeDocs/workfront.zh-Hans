---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: “Workfront Fusion版本活动：2020年11月16日一周
description: 本页介绍了2020年11月16日这一周Adobe Workfront Fusion中所有增强功能。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Workfront Fusion版本活动： 2020年11月16日开始的一周

本页介绍了2020年11月16日这一周Adobe Workfront Fusion中所有增强功能。

有关所有最近更改的列表，请参阅 [Adobe Workfront Fusion版本活动](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

有关Workfront Fusion中最近的错误修复列表，请参阅 [Workfront维护更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 页面，并检查标记为Workfront Fusion维护更新的任何更新。

## Jira Cloud连接器更新

为了扩展Jira Cloud连接器的使用方式，我们添加了三个新模块：

* 向冲刺添加问题
* 列表记录
* 搜索记录

我们还更新了现有模块，以支持“Sprint”对象类型。 以前，“Sprint”对象只能通过自定义API调用模块访问。

有关更多信息，请参阅 [Jira软件模块](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## 执行ID现在可用于在各种情况下进行映射

方案的执行ID现在在映射面板中可用。 此ID表示方案的特定执行，可用作元数据。 例如，执行ID可以与Fusion创建的记录一起保存，以便您稍后能够确定是哪个Fusion执行创建了该记录。 您可以在映射面板中的常规函数下找到执行ID。

有关方案执行的更多信息，请参阅 [Adobe Workfront Fusion中的方案执行、周期和阶段](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Workfront Fusion 2.0情景的键盘快捷键

为了更方便地构建方案，我们添加了一些键盘快捷键：

* Ctrl/Cmd+Shift+Enter:运行一次方案
* Ctrl/Cmd + Shift + S:保存方案

有关构建Workfront Fusion 2.0情景的更多信息，请参阅 [在Adobe Workfront Fusion中创建方案](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Office 365 Excel连接器的更新

为了扩展Office 365 Excel连接器的使用方式，我们添加了一些新模块。 现在，您可以：

* 触发对工作簿的更改的模块
* 搜索或下载工作簿
* 列出工作表、工作表行、表或表行
* 更新表或工作表行
* 删除表或工作表行
* 检索表的元数据
* 进行自定义API调用

以前可用的模块仍存在于应用程序中。

有关更多信息，请参阅 [Microsoft Office 365 Excel模块](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## 在Workfront应用程序连接中使用OAuth 2.0

我们已更新Workfront连接器以使用OAuth 2.0。此更新意味着更轻松地在Workfront应用程序连接中进行更改。 例如，如果您的连接发生某些更改（如密码），则在您的情景中不再需要更新每个连接。 此外，OAuth2还提供其他好处，例如增强了安全性和使用单点登录(SSO)的功能。

现有连接此时不需要进行任何更改。 但是，如果您想要利用OAuth 2.0的好处，可以重新授权现有连接。

有关更多信息，请参阅 [Adobe Workfront模块](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
