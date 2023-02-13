---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 针对问题配置完成按钮
description: 完成按钮可自动设置任务或问题的状态。 默认情况下，当代理人在其工作项上单击完成时，Adobe Workfront会将问题标记为已解决。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# 配置 [!UICONTROL 完成] 问题按钮

的 [!UICONTROL 完成] 按钮可自动设置任务或问题的状态。 默认情况下， [!DNL Adobe Workfront] 将问题标记为 [!UICONTROL 已解决] 受让人单击 [!UICONTROL 完成] 工作项目上。

## 概述

具有特定权限的用户可以配置 [!UICONTROL 完成] 按钮来反映系统中的某些状态。 有3种不同的方式 [!UICONTROL 完成] 按钮适用于 [!DNL Workfront]:

* 如果用户已分配 [!UICONTROL 主队], a [!DNL Workfront] 管理员或具有 [!UICONTROL 计划] 许可证可以配置 [!UICONTROL 完成] 按钮来反映团队成员的某些状态。 请参阅 [配置 [!UICONTROL 完成] 按钮](#configure-the-uicontrol-done-button-for-a-team) 在本文中。
* 如果用户没有 [!UICONTROL 主队] 分配， [!UICONTROL 完成] 问题按钮与系统生成的 [!UICONTROL 已解决] 具有三字母代码的状态 [!UICONTROL RLV]. 此方案中没有可用的配置选项。 的 [!UICONTROL 完成] 按钮将自动默认为此状态。
* 如果 [!UICONTROL 已解决] ([!UICONTROL RLV])状态，并将问题标记为 [!UICONTROL 完成] 否 [!UICONTROL 主队]，则默认问题状态将绑定到默认设置为 [!UICONTROL 已关闭] 对于分配给问题所属的项目的组。 Workfront管理员可以为组配置全系统的默认设置。 请参阅 [配置 [!UICONTROL 完成] 按钮 [!UICONTROL 已解决] 状态已删除](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 在本文中。

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
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td>删除[!UICONTROL Resolved]状态后，需要系统管理员访问权限才能配置[!UICONTROL Done]按钮</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

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
   >  例如，将 [!UICONTROL 完成] 按钮，使工作项显示为 [!UICONTROL 完成] 将状态从“新建”更改为“正在进行”的用户。
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
任何团队设置，包括与 [!UICONTROL 完成] 按钮，此时这些用户便可看到。

## 配置 [!UICONTROL 完成] 按钮 [!UICONTROL 已解决] 状态已删除

如果用户没有“Home Team（家庭团队）”，则系统范围内的 [!UICONTROL 已解决] ([!UICONTROL RLV])已删除， [!DNL Workfront] 管理员可以配置 [!UICONTROL 已关闭] 上的组的状态。 [!DNL Workfront] 在用户单击 [!DNL Done] 按钮。

### 查找与项目关联的组

当用户创建项目时，其“主页”组会自动分配给该项目。 具有 [!UICONTROL 管理] 对项目的访问权限可以在 [!UICONTROL 项目详细信息] 中的“隐藏主体”。 了解状态 [!DNL Workfront] 在这种情况下，您必须了解与问题所在项目关联的组以及的默认状态 [!UICONTROL 已关闭] 此组存在问题。

要查找与项目关联的组，请执行以下操作：

1. 转到项目。
1. 在页面的左侧，单击 **[!UICONTROL 项目详细信息]**.
1. 找到 **[!UICONTROL 项目关联]** 部分，然后查找 **[!UICONTROL 组]**.\
   这是您在“设置”区域中检查状态时需要使用的组名称。 有关如何更新特定组的默认状态的说明，请参阅以下部分。

### 更新特定组的默认状态

As a [!UICONTROL Workfront] 管理员，您可以更新特定组的状态：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **[!UICONTROL 项目首选项]**，则 **[!UICONTROL 状态]**.

1. 单击 **[!UICONTROL 问题]**，然后在 **[!UICONTROL 系统状态]** 搜索框。

1. 选择群组。
1. 单击 **[!UICONTROL 设置默认状态]** 下拉菜单中，然后为 [!UICONTROL 已关闭]. [!DNL Workfront] 当用户单击 [!UICONTROL 完成] 按钮。

   >[!IMPORTANT]
   >
   >仅当用户未分配主团队，并且 [!UICONTROL RLV] 状态已删除。

1. 单击&#x200B;**[!UICONTROL 保存]**。
