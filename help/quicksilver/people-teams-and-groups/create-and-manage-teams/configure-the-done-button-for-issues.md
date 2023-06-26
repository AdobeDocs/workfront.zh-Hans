---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 为问题配置“完成”按钮
description: 完成按钮可自动设置任务或问题的状态。 默认情况下，当被分配人单击其工作项上的“完成”时，Adobe Workfront将问题标记为“已解决”。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 0%

---

# 配置 [!UICONTROL 完成] 问题的按钮

此 [!UICONTROL 完成] 按钮可自动设置任务或问题的状态。 默认情况下， [!DNL Adobe Workfront] 将问题标记为 [!UICONTROL 已解决] 当被分派人单击时 [!UICONTROL 完成] 在工作项上。

## 概述

具有特定权限的用户可以配置 [!UICONTROL 完成] 按钮来反映系统中的特定状态。 有3种不同的方式 [!UICONTROL 完成] 按钮适用于中的问题 [!DNL Workfront]：

* 如果用户已分配 [!UICONTROL 主团队]， a [!DNL Workfront] 管理员或具有权限的用户 [!UICONTROL 计划] 许可证可以配置 [!UICONTROL 完成] 按钮以反映团队成员的某些状态。 参见 [配置 [!UICONTROL 完成] “团队”按钮](#configure-the-uicontrol-done-button-for-a-team) 本文章中。
* 如果用户没有 [!UICONTROL 主团队]，但它们具有 [!UICONTROL 其他团队] 在其配置文件中，Workfront搜索 [!UICONTROL 完成] 任何与用户关联的团队上的按钮。 选择是随机的，与任何团队关联的状态用于问题。
* 如果用户没有 [!UICONTROL 主团队] 已分配， [!UICONTROL 完成] 问题的按钮已绑定到系统生成的 [!UICONTROL 已解决] 具有三个字母代码的状态 [!UICONTROL RLV]. 此方案中没有可用的配置选项。 此 [!UICONTROL 完成] 按钮会自动默认为此状态。
* 如果 [!UICONTROL 已解决] ([!UICONTROL RLV])状态已删除，并且用户将该问题标记为 [!UICONTROL 完成] 没有 [!UICONTROL 主团队]，默认问题状态会绑定到设置为默认问题的任何内容， [!UICONTROL 已关闭] 对于分配给问题所属项目的组。 Workfront管理员可以为组配置系统范围的默认设置。 参见 [配置 [!UICONTROL 完成] 按钮时 [!UICONTROL 已解决] 已删除状态](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 本文章中。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>[！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td>删除[！UICONTROL已解决]状态后，需要系统管理员访问权限才能配置[！UICONTROL完成]按钮</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

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
   >  例如，关联 [!UICONTROL 完成] 按钮进行中导致工作项显示为 [!UICONTROL 完成] （对于将状态从“新建”更改为“进行中”的用户）。
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
任何团队设置，包括与关联的状态 [!UICONTROL 完成] 按钮，现在对这些用户可见。

## 配置 [!UICONTROL 完成] 按钮时 [!UICONTROL 已解决] 已删除状态

如果用户没有主团队，则系统范围默认为 [!UICONTROL 已解决] ([!UICONTROL RLV])已被删除，a [!DNL Workfront] 管理员可以配置 [!UICONTROL 已关闭] 项目组的状态。 [!DNL Workfront] 当用户单击 [!DNL Done] 按钮。

### 查找与项目关联的组

当用户创建项目时，其主组会自动分配给该项目。 用户具有 [!UICONTROL 管理] 对项目的访问权限可以在以下位置更改此组： [!UICONTROL 项目详细信息] 部分。 了解什么状态 [!DNL Workfront] 使用处理完成的问题，在这种情况下，您必须了解问题所在的与项目关联的组以及默认状态 [!UICONTROL 已关闭] 此组存在问题。

要查找与项目关联的组，请执行以下操作：

1. 转到项目。
1. 在页面左侧，单击 **[!UICONTROL 项目详细信息]**.
1. 找到 **[!UICONTROL 项目关联]** 部分，然后查找 **[!UICONTROL 组]**.\
   您需要使用这个组名称来检查“设置”区域中的状态。 有关如何更新特定组的默认状态的说明，请参阅以下部分。

### 更新特定组的默认状态

As a [!UICONTROL Workfront] 管理员，您可以更新特定组的状态：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **[!UICONTROL 项目首选项]**，则 **[!UICONTROL 状态]**.

1. 单击 **[!UICONTROL 问题]**，然后在中键入组的名称 **[!UICONTROL 系统状态]** 搜索框。

1. 选择组。
1. 单击 **[!UICONTROL 设置默认状态]** 下拉菜单，然后选择默认状态 [!UICONTROL 已关闭]. [!DNL Workfront] 当用户单击 [!UICONTROL 完成] 按钮。

   >[!IMPORTANT]
   >
   >仅当用户没有分配的主团队且 [!UICONTROL RLV] 已删除状态。

1. 单击&#x200B;**[!UICONTROL 保存]**。
