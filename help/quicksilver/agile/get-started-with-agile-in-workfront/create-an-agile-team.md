---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 创建敏捷团队
description: Adobe Workfront使agile团队能够以递增、有条理的方式完成工作。
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 1%

---

# 创建敏捷团队

[!DNL Adobe Workfront] 使Agile团队能够以增量、有条理的方式完成工作。

组织中的任何用户都可以查看Agile团队并查看团队的所有敏捷组件，包括积压、迭代、故事板和单个故事。 但是，只有团队成员具有 [!UICONTROL 编辑] 对工作的访问权限可对分配给团队的工作进行更改。

[!DNL Workfront] 支持以下agile方法：

* **[!UICONTROL Scrum]**：团队有需要完成的积压工作。 当团队准备好处理特定工作块时，该工作会从积压工作移动到迭代。 有关管理Scrum团队的更多详细信息，请参阅 [敏捷团队中的Scrum](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]：** 团队在Kanban视图中跨预定状态移动工作。 默认状态为：积压、处理中和完成。 有关管理Kanban团队的更多详细信息，请参阅 [敏捷团队中的Kanban](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL计划]以创建一个新的Agile团队；[！UICONTROL工作]或更高版本以将团队转换为Agile团队</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。

## 确定敏捷方法

您可以为敏捷团队使用Scrum或Kanban敏捷方法。 每种方法都提供了多种好处。 敏捷团队的工作方式决定了您选择使用的敏捷方法。

中的Scrum和Kanban敏捷方法 [!DNL Workfront] 允许您跨故事板移动故事以指示故事的状态更改和进度。

中的Scrum和Kanban敏捷方法 [!DNL Workfront] 有以下不同之处：

### 在中使用Kanban的好处 [!DNL Workfront]

此 [!DNL Kanban] 中的敏捷方法 [!DNL Workfront] 让您能够更轻松地在敏捷故事板中移动故事，同时限制进行中的工作量。 使用时没有开始和结束日期 [!DNL Kanban] 敏捷方法。

以下功能支持此方法：

* 在上显示积压 [!DNL Kanban] 敏捷故事板。\
   有关更多信息，请参阅 [将积压添加到 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* 配置积压工作上的项目以自动添加到 [!UICONTROL Kanban] 当其他项目移至等同于“完成”的状态时，敏捷故事板。\
   有关更多信息，请参阅部分 [配置要从积压自动添加的故事](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) 在文章中 [配置Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* 配置要显示在“ ”上的正在进行的工作(WIP)限制 [!UICONTROL Kanban] 敏捷故事板。\
   有关更多信息，请参阅 [在Kanban展示板上管理正在进行的工作(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### 在中使用Scrum的好处 [!DNL Workfront]

中的Scrum敏捷方法 [!DNL Workfront] 允许您向敏捷开发周期添加一组故事并为其创建故事板。 迭代基于您定义的开始和结束日期。

以下功能支持此方法：

* 包含相关问题 [!UICONTROL Scrum] 故事板
* 包括Agile团队积压的问题
* 子任务可以显示在 [!UICONTROL Scrum] 故事板
* 查看燃尽图以查看迭代期间历程的进度\
   有关更多信息，请参阅 [敏捷燃尽图概述](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 创建敏捷团队

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.
1. 单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后单击 **[!UICONTROL 创建新团队]**.

   ![选择“创建新团队”。](assets/create-new-team-350x198.png)

1. 指定以下信息，请参见 [!UICONTROL 新建团队] 对话框：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL团队名称]</strong> </td> 
      <td>键入新Agile团队的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL这是一个Agile团队]</strong> </td> 
      <td>选择此选项可将此新团队配置为Agile团队。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[！UICONTROL组]</strong> </td> 
      <td> <p>开始键入要添加到团队中的组的名称，然后在该名称出现在下拉列表中时选择该名称。</p> <p>注意：将团队分配给组或子组时，该组或子组的任何组管理员都可以管理团队，而无需成为其成员。 组管理员可以从[！UICONTROL主菜单]转到[！UICONTROL团队]区域，然后单击[！UICONTROL切换团队]箭头 <img src="assets/switch-team-icon.png" alt="“切换团队”图标"> 列出分配给其管理组的所有团队。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL团队成员]</strong> </td> 
      <td>开始键入要加入团队的用户的名称，然后在名称出现在下拉列表中时选择该名称。<br>重复此过程以将多个用户添加到团队。<br>由于用户可以位于多个团队中，因此他们可以同时位于敏捷和非敏捷团队中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL描述]</strong> </td> 
      <td><p>键入团队描述。</p> <p>选择团队时，描述显示在[！UICONTROL团队]区域的右上角。</p>
      <p>如果描述较长，则可以单击该描述以在弹出窗口中显示完整描述。 如果您有权编辑[！UICONTROL团队设置]，则还可以直接在弹出窗口中编辑描述。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建]**.

   有关配置Agile团队的信息，请参阅以下文章：

   * [配置 [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [配置 [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 将现有团队转换为Agile团队

您可以将现有团队转换为Agile团队：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.
1. 单击 **[!UICONTROL 切换组]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要转换为Agile团队的团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\
   仅团队成员具有任一个 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。\
   ![](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，选择 **[!UICONTROL 这是Agile团队]**.

1. 在 **[!UICONTROL 方法]** 部分，选择团队是否将使用 **[!UICONTROL Scrum]** 或 **[!UICONTROL Kanban]** 敏捷方法。

1. 单击 **保存更改。**

   有关配置Agile团队的信息，请参阅以下文章：

   * [配置 [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [配置 [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
