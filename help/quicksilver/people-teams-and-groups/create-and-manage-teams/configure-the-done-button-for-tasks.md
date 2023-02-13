---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 为任务配置完成按钮
description: 完成按钮可自动设置任务或问题的状态。 默认情况下，当代理人在其工作项上单击“完成”时，Adobe Workfront会将任务标记为“已完成”。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# 配置 [!UICONTROL 完成] “任务”按钮

的 [!UICONTROL 完成] 按钮可自动设置任务或问题的状态。 默认情况下， [!UICONTROL Adobe Workfront] 将任务标记为 [!UICONTROL 已完成] 当被分派人单击其工作项上的完成时。

## 概述

具有特定权限的用户可以配置 [!UICONTROL 完成] 按钮来反映系统中的某些状态。 有两种不同的方式 [!UICONTROL 完成] 按钮适用于中的任务 [!UICONTROL Workfront]:

* 如果用户已分配了“Home Team”（主团队），则 [!DNL Workfront] 管理员或具有 [!UICONTROL 计划] 许可证可以配置 [!UICONTROL 完成] 按钮来反映团队成员的某些状态。 请参阅 [配置 [!UICONTROL 完成] 按钮](#configure-the-uicontrol-done-button-for-a-team) 在本文中。
* 如果用户未分配“Home Team”（主页团队），则 [!UICONTROL 完成] “任务”按钮将绑定到完整状态。 此方案中没有可用的配置选项。 的 [!UICONTROL 完成] 按钮将自动默认为此状态。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 配置 [!UICONTROL 完成] 按钮

您可以使用 [!UICONTROL 完成] 按钮。 您还可以设置多个状态，并允许用户选择合适的状态。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后单击 **[!UICONTROL 编辑]**.
1. 查找 **[!UICONTROL “完成”按钮]** 部分 **[!UICONTROL 团队设置]** 页面。

1. 为每个工作项类型选择一个或多个状态。

   >[!NOTE]
   >
   >为任务或问题选择状态时，请考虑以下事项：
   >
   >* 当您为每种工作项目类型选择一个状态时，当用户单击时，任务或问题状态将设置为该状态 [!UICONTROL 完成] 在他们的物品上。 如果为每种类型的工作项设置多个状态，则会向 [!UICONTROL 完成] 按钮，用户必须选择状态才能更改工作项的状态。
   >* 您只能将系统级别的状态与 [!UICONTROL 完成] 按钮。 您无法将特定于组的状态与工作项状态关联。
   >* 当分配给该项目的用户将该项目置于与 [!UICONTROL 完成] 按钮时，项目显示为 [!UICONTROL 完成] 无论您选择的状态是否为 [!UICONTROL 已完成] 或 [!UICONTROL 已关闭] 状态或工作状态。

   >   
   >   
   >  例如，将 [!UICONTROL 完成] 按钮 [!UICONTROL 正在进行] 使工作项显示为 [!UICONTROL 完成] 从 [!UICONTROL 新建] to [!UICONTROL 正在进行].
   >   
   >* 问题类型是可自定义的，它们的名称可能与您的环境中下面列出的名称有所不同。\
      >  以下是默认任务和问题类型：
      >     
      >   * [!UICONTROL 任务]
      >   * [!UICONTROL 问题]
      >   * [!UICONTROL 请求]
      >   * [!UICONTROL 更改顺序]
      >   * [!UICONTROL 错误报告]


   如果任务或问题已分配给多个用户，您会看到“[!UICONTROL 完成我的任务]“ ”选项，以及为团队选择的多个状态。

1. 单击 **[!UICONTROL 保存更改]**.

## 将用户与主团队关联

对 [!UICONTROL 完成] 按钮功能，您可以使其设置已更改用户“主团队”的团队。

要将用户与主团队关联，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront].

1. 单击 **[!UICONTROL 用户]**，然后选择要与主团队关联的用户。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 组织]** 选择 **[!UICONTROL 主队]** 字段。 开始键入要与用户关联其设置的团队的名称。 当您在列表中看到团队时，请单击该团队的名称。

1. 单击 **[!UICONTROL 保存更改]**.\
   现在，您选择的用户已与主团队关联。
任何团队设置，包括与 [!UICONTROL 完成] 按钮。
