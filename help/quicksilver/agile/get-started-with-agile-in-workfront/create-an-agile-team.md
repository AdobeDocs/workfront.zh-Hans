---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 创建Agile团队
description: Adobe Workfront使agile团队能够以递增、有条理的方式完成工作。
author: Jenny
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 1%

---

# 创建敏捷团队

<!--Audited: 01/2024-->

[!DNL Adobe Workfront]允许Agile团队以递增、有条理的方式完成工作。

组织中的任何用户都可以查看Agile团队并查看团队的所有敏捷组件，包括积压、迭代、故事板和单个故事。 但是，只有对工作具有[!UICONTROL 编辑]权限的团队成员才能更改分配给团队的工作。

[!DNL Workfront]支持以下Agile方法：

* **[!UICONTROL Scrum]**：团队有需要完成的积压工作。 当团队准备好处理特定工作块时，该工作会从积压工作移动到迭代。 有关管理Scrum团队的更多详细信息，请参阅[敏捷团队中的Scrum](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md)。

* **[!UICONTROL Kanban]：**&#x200B;团队在Kanban视图中跨预定状态移动工作。 默认状态为：积压、处理中和完成。 有关管理Kanban团队的更多详细信息，请参阅[敏捷团队中的Kanban](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>计划创建新的Agile团队</p>
  <p>将团队转换为Agile团队的工作方式或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 确定敏捷方法

您可以为敏捷团队使用Scrum或Kanban敏捷方法。 每种方法都提供了多种好处。 敏捷团队的工作方式决定了您选择使用的敏捷方法。

[!DNL Workfront]中的Scrum和Kanban敏捷方法都允许您在故事板中移动故事以指示状态更改和故事的进度。

[!DNL Workfront]中的Scrum和Kanban敏捷方法在以下方面有所不同：

### 在[!DNL Workfront]中使用Kanban的好处

[!DNL Kanban]中的[!DNL Workfront]敏捷方法使您能够更轻松地在Agile故事板中移动故事，同时限制正在进行的工作量。 使用[!DNL Kanban] Agile方法时没有开始和结束日期。

以下功能支持此方法：

* 在[!DNL Kanban]敏捷故事板上显示积压。
有关详细信息，请参阅[将积压工作添加到[!UICONTROL Kanban]展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)。

* 配置当其他项目移至等同于“完成”的状态时，将积压中的项目自动添加到[!UICONTROL Kanban]敏捷故事板中。
有关详细信息，请参阅文章[配置Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)中的[配置要自动从积压工作中添加的故事](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)部分。

* 配置要在[!UICONTROL Kanban]敏捷故事板上显示的进行中的工作(WIP)限制。
有关详细信息，请参阅[在Kanban展示板上管理正在进行的工作(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)。

### 在[!DNL Workfront]中使用Scrum的好处

[!DNL Workfront]中的Scrum敏捷方法允许您向敏捷迭代添加一组故事并为该迭代创建故事板。 迭代基于您定义的开始和结束日期。

以下功能支持此方法：

* 包含[!UICONTROL Scrum]故事板上的问题
* 包括Agile团队积压的问题
* 子任务可以显示在[!UICONTROL Scrum]故事板上
* 查看燃尽图以查看迭代期间历程的进度
有关详细信息，请参阅[敏捷燃尽图概述](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

## 创建敏捷团队

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后单击&#x200B;**[!UICONTROL 创建新团队]**。

   ![选择“创建新团队”](assets/create-new-team.png)

   此时将显示“新建团队”框。

1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL团队名称]</strong> </td> 
      <td>键入新Agile团队的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL这是Agile团队]</strong> </td> 
      <td>选择此选项可将此新团队配置为Agile团队。</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[！UICONTROL处于活动状态]</strong> </td> 
      <td>选择此选项以激活此团队。 其他用户对非活动的团队不可见以分配给工作。 </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[！UICONTROL组]</strong> </td> 
      <td> <p>开始键入要添加到团队中的组的名称，然后在该名称出现在下拉列表中时选择该名称。</p> <p><b>注释</b></p> <p> 将团队分配给组或子组后，该组或子组的任何组管理员都可以管理团队，而无需成为团队成员。 组管理员可以从[！UICONTROL主菜单]转到[！UICONTROL团队]区域，然后单击[！UICONTROL切换团队]箭头<img src="assets/switch-team-icon.png" alt="“切换团队”图标">列出分配给其管理的组的所有团队。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL团队成员]</strong> </td> 
      <td>开始键入要加入团队的用户的名称，然后在名称出现在下拉列表中时选择该名称。<br>重复此过程以将多个用户添加到团队。<br>由于用户可能位于多个团队中，因此他们可以同时位于敏捷和非敏捷团队中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL描述]</strong> </td> 
      <td><p>键入团队描述。</p> <p>选择团队时，描述显示在[！UICONTROL团队]区域的右上角。</p>
      <p>如果描述较长，则可以单击该描述以在弹出窗口中显示完整描述。 如果您有权编辑[！UICONTROL团队设置]，则还可以直接在弹出窗口中编辑描述。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 创建]**。

   有关配置Agile团队的信息，请参阅以下文章：

   * [配置[!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [配置[!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 将现有团队转换为Agile团队

您可以将现有团队转换为Agile团队：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要转换为Agile团队的团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有具有[!UICONTROL Standard]、[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。
   ![选择编辑](assets/edit-team-settings.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 这是Agile团队]**。

1. 在&#x200B;**[!UICONTROL 方法]**&#x200B;部分中，选择团队将使用&#x200B;**[!UICONTROL Scrum]**&#x200B;还是&#x200B;**[!UICONTROL Kanban]**&#x200B;敏捷方法。

1. 单击&#x200B;**保存更改**。

   团队将另存为Agile团队。 在编辑团队时，您可以将新团队配置为Scrum或Kanban团队。

   有关更多信息，请参阅以下文章：

   * [配置[!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [配置[!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
