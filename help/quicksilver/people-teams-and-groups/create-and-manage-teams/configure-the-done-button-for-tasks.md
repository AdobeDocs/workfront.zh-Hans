---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 为任务配置完成按钮
description: 完成按钮可自动设置任务或问题的状态。 默认情况下，当被分配人单击其工作项上的完成时，Adobe Workfront将任务标记为已完成。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 配置 [!UICONTROL 完成] 任务按钮

此 [!UICONTROL 完成] 按钮可自动设置任务或问题的状态。 默认情况下， [!UICONTROL Adobe Workfront] 将任务标记为 [!UICONTROL 已完成] 被分派人在其工作项上单击“完成”时。

## 概述

具有特定权限的用户可以配置 [!UICONTROL 完成] 按钮来反映系统中的特定状态。 有两种不同的方式 [!UICONTROL 完成] 按钮适用于中的任务 [!UICONTROL Workfront]：

* 如果用户已分配主团队，则 [!DNL Workfront] 管理员或具有权限的用户 [!UICONTROL 计划] 许可证可以配置 [!UICONTROL 完成] 按钮以反映团队成员的某些状态。 参见 [配置 [!UICONTROL 完成] “团队”按钮](#configure-the-uicontrol-done-button-for-a-team) 本文章中。
* 如果用户没有 [!UICONTROL 主团队]，但它们具有 [!UICONTROL 其他团队] 在其配置文件中，Workfront搜索 [!UICONTROL 完成] 任何与用户关联的团队上的按钮。 选择是随机的，与任何团队关联的状态用于任务。
* 如果用户没有分配主团队，则 [!UICONTROL 完成] 任务的按钮与完成状态相关联。 此方案中没有可用的配置选项。 此 [!UICONTROL 完成] 按钮会自动默认为此状态。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 计划*</strong></p></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 许可证*</strong></p></td> 
   <td> <p>[！UICONTROL计划] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。

## 配置 [!UICONTROL 完成] “团队”按钮

您可以使用更改应用于工作项的状态 [!UICONTROL 完成] 按钮。 您还可以设置多个状态，并允许用户选择合适的状态。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后单击 **[!UICONTROL 编辑]**.
1. 查找 **[!UICONTROL 完成按钮]** 底部的部分 **[!UICONTROL 团队设置]** 页面。

1. 为每个工作项类型选择一个状态或多个状态。

   >[!NOTE]
   >
   >为任务或问题选择状态时，请考虑以下事项：
   >
   >* 当您为每种类型的工作项选择一个状态时，任务或问题状态会在用户单击时设置为该状态 [!UICONTROL 完成] 在他们的物品上。 如果为每种类型的工作项设置多个状态，则会将下拉菜单添加到 [!UICONTROL 完成] 按钮和用户必须选择一个状态才能更改工作项的状态。
   >* 您只能将系统级别状态与 [!UICONTROL 完成] 按钮。 您无法将组特定的状态与工作项状态相关联。
   >* 当分配给项目的用户将该项目置于与关联的状态时 [!UICONTROL 完成] 按钮时，项目显示为 [!UICONTROL 完成] ，无论您选择的状态是否为 [!UICONTROL 已完成] 或 [!UICONTROL 已关闭] 状态或工作状态。
   >   
   >   
   >  例如，关联 [!UICONTROL 完成] 按钮替换为 [!UICONTROL 进行中] 使工作项显示为 [!UICONTROL 完成] 对于更改状态的用户 [!UICONTROL 新] 到 [!UICONTROL 进行中].
   >   
   >* 问题类型可自定义，并且它们的名称可能与您的环境中下面列出的名称不同。\
   >  以下是默认任务和问题类型：
   >     
   >   * [!UICONTROL 任务]
   >   * [!UICONTROL 问题]
   >   * [!UICONTROL 请求]
   >   * [!UICONTROL 更改顺序]
   >   * [!UICONTROL 错误报告]

   如果任务或问题分配给多个用户，您将看到“[!UICONTROL 完成我的部分]”选项，以及为您的团队选择的多个状态。

1. 单击 **[!UICONTROL 保存更改]**.

## 将用户与主团队关联

要对 [!UICONTROL 完成] 按钮功能对用户可见，您可以使更改其设置的用户的主团队成为团队。

要将用户与主团队关联，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe Workfront].

1. 单击 **[!UICONTROL 用户]**，然后选择要与主团队关联的一个或多个用户。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 组织]** 部分，选择 **[!UICONTROL 主团队]** 字段。 开始键入要将其设置与用户关联的团队的名称。 在列表中看到团队时，单击该团队的名称。

1. 单击 **[!UICONTROL 保存更改]**.\
   您选择的用户现在与主团队关联。
任何团队设置，包括与关联的状态 [!UICONTROL 完成] 按钮现在对这些用户可见。
