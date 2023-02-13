---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 配置看板
description: 在创建小组期间或之后，您可以为看板敏捷团队配置以下选项。
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 配置 [!UICONTROL 看板]

在创建团队期间或创建团队之后，您可以为敏捷团队配置以下选项。 在 [!DNL Adobe Workfront] 如 [创建敏捷的团队](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 配置文章是以点还是以小时为单位进行估计

您可以配置文章以使用点或小时进行估计。

要配置如何为您的敏捷团队评估故事，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Workfront]，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。
1. 选择要管理的敏捷团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。\
   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 在中估算文章]** 区域，选择是使用点还是小时来估算文章的大小（工作量）。 如果选择“点”，请指定小时数等于1点。 （默认值为1点= 8小时。） 这是添加到文章的计划小时数。

   **示例：** 如果您选择以分来估计文章，而1分等于8小时，而文章估计为3分，则会在文章中添加24个计划小时。

1. 单击 **[!UICONTROL 保存更改]**.

## 在敏捷文章展示板上配置状态列

您可以为敏捷团队定义文章展示板上存在的状态。 这些状态是文章展示板上唯一显示的状态。

要定义可用于与敏捷团队关联的文章展示板的状态，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!UICONTROL Workfront]，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。

1. 选择要管理的敏捷团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** ，找到 **[!UICONTROL 文章展示板]** 的上界。

1. （可选）单击 **[!UICONTROL 添加列]** 向文章板添加其他状态列。
1. （可选）使用拖放指示器拖动任何状态列，以重新排序文章展示板上的状态列。 无法移动第一列，并且不能将另一列拖动到第一列前面。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 选择任务状态。

   >[!IMPORTANT]
   >
   >只能选择系统范围的锁定状态；您无法选择特定于群组的状态。 此外，第一列的状态始终对应 **[!UICONTROL 新建]**.

   您可以添加自定义状态(如果 [!DNL Workfront] 管理员已配置了这些配置；可以按照 [创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 单击 **[!UICONTROL 保存更改]**.

## 配置要在敏捷文章展示板上的文章卡片上显示的其他字段

在向文章卡片中添加字段时，在填充字段时，字段为仅查看字段和仅显示字段。

默认情况下，文章卡片中会显示以下类型的任务和问题数据：

* 带有直接指向任务或问题的链接的文章名称
* 带有直接指向项目的链接的项目名称
* 此链接仅用于文章，而不用于子任务
* 任务或问题说明
* 当前承诺
* 通过调整完成百分比本身或通过调整完成的点数或小时数，查看和编辑完成百分比
* 已分配的用户

您可以在文章卡片上显示其他数据（包括自定义数据）。 出于任何原因，您可能希望在文章卡片上显示其他字段。 例如，如果您在小版本中为多个客户处理文章，或者您可能希望显示项目开始日期或项目完成日期，则可能需要显示客户ID。

>[!NOTE]
>
>如果在文章卡片上使用自定义字段，则该字段的名称中不能包含句点/圆点。

要配置分配给敏捷团队的文章卡片以显示其他字段，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Workfront]，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。

1. 选择要管理的敏捷团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\
   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 字段名称，以将其找到。

   ![其他字段](assets/agile-additional-fields-kanban.png)

1. 选择要添加的字段的名称。
1. 键入 **[!UICONTROL 显示名称]** ，以便在文章或发行卡上显示字段。
1. 单击 **[!UICONTROL 保存更改]**.

## 配置在进工作(WIP)限制

看板 [!DNL Workfront] 允许您通过限制在 [!UICONTROL 正在进行] 列 [!UICONTROL 看板] 展示板。

配置WIP限制后，您可以查看WIP限制，甚至从 [!UICONTROL 看板] 敏捷故事板，如 [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

要限制看板团队的WIP，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。

1. 选择要管理的看板团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 方法]** 部分，确保选中看板。

1. 在 **[!UICONTROL 文章展示板]** 部分，在 **[!UICONTROL WIP限制]** 字段，指定 [!UICONTROL 看板] 敏捷故事板。 您可以为每列设置不同的限制。 您可以为每列设置的最大限制为100。\
   设置后，WIP限制会在 [!UICONTROL 看板] 每当超出文章板上任何列的限制时，便会使用灵活文章板。 仅当首次超出WIP限制时，才会显示此警告消息。 任何状态等于 [!UICONTROL 完成].\
   WIP限制只是一个可视警告，不会限制您的团队在一个列中拥有比您设置的限制更多的项目。

   ![WIP限制](assets/wip-limit-350x193.png)

1. 单击 **保存更改**.

## 配置要自动从积压工作中添加的文章

您可以将积压文章配置为自动添加到 [!UICONTROL 看板] 将项目从该列中移动后立即进入展示板。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. 单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。

1. 选择要管理的看板团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 选择 **[!UICONTROL 自动从积压工作中添加下一篇文章]** 配置要自动从积压工作到 [!UICONTROL 看板] 故事板。

   每当将文章移动到文章展示板上表示“完整”状态（状态等于“完成”）的列中时，就会发生这种情况。 当从积压工作中添加时，具有最高优先级的文章会添加到文章展示板。选择此选项可配置积压工作中的下一个项目，以自动添加到 **[!UICONTROL 正在进行]** 列 **[!UICONTROL 正在进行]** 列。

1. 单击 **[!UICONTROL 保存更改]**.

## 配置信息卡在 [!UICONTROL 看板] 展示板

您可以选择已完成的信息卡在 [!UICONTROL 看板] 展示板。 从 [!UICONTROL 看板] 仍然可以在其原始项目中访问展示板。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新看板团队，或在搜索栏中搜索团队。
1. 选择看板组。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **Edit**.

   仅具有 [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证请参阅此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 已完成卡在看板板上停留的天数]** 下拉菜单中，选择一个值。
1. 单击 **[!UICONTROL 保存更改]**.
