---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 配置Kanban
description: 您在中创建了Kanban或Scrum敏捷团队 [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# 配置 [!UICONTROL Kanban]

您可以在中创建Agile团队 [!DNL Adobe Workfront] 如中所述 [创建Agile团队](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). 在创建Agile团队时，您可以选择团队用于完成其工作的方法。 您可以从以下选项中进行选择：

* Scrum
* Kanban

本文介绍了如何配置Kanban团队的设置。 在创建敏捷团队并选择Kanban方法之后，您可以参考本文以更新以下设置：

* 故事的估计单位是点还是小时
* 敏捷故事板上的状态列
* 要在敏捷故事板上的故事卡上显示的其他字段
* 正在进行的工作(WIP)限制
* 如何自动添加积压中的故事
* 卡片在Kanban展示板上停留多长时间

有关配置Scrum团队的信息，请参阅 [配置Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## 访问要求

<!--Audited: 12/2023-->

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p> 
   或
   <p>当前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>编辑团队的访问权限</p>  </td> 
  </tr>

</tbody> 
</table>

*要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。

## 配置故事的估计单位为点还是小时

您可以将故事配置为使用点数或小时进行估计。

要配置如何为您的Agile团队估计故事：

{{step1-to-team}}

1. 单击 **[!UICONTROL 切换团队]** 图标 ![](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索框中搜索团队。
1. 选择要管理的Agile团队。
1. 单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-menu.png) ，然后选择 **[!UICONTROL 编辑]**.

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 估计故事位于]** 区域，选择是使用点还是小时来估算文章的大小（工作负荷）。 如果选择“点”，请指定多少小时等于1点。 （默认值为1点= 8小时。） 这是添加到故事的计划小时数。

   **示例：** 如果您已选择估计故事的点数，1点等于8小时，并且故事的估计点数为3，则系统会将24个已计划小时数添加到故事中。

1. 单击 **[!UICONTROL 保存更改]**.

## 在敏捷故事板上配置状态列

您可以为Agile团队定义故事板上的状态。 这些是在故事板上显示的唯一状态。

要定义可用于与Agile团队关联的故事板的状态，请执行以下操作：

{{step1-to-team}}

1. 单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，找到 **[!UICONTROL 故事板]** 区域。

1. （可选）单击 **[!UICONTROL 添加列]** 向故事板添加其他状态列。
1. （可选）使用拖放指示器拖动任意状态列，以重新排列故事板上的状态列。 无法移动第一列，也不能将另一列拖到第一列的前面。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 选择任务状态。

   >[!IMPORTANT]
   >
   >只有锁定的系统范围状态可供选择。 您不能选择特定于组的状态。 第一列的状态始终对应于 **[!UICONTROL 新建]**.

   您可以添加自定义状态，如果 [!DNL Workfront] 管理员已配置它们。 有关更多信息，请参阅 [创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 单击 **[!UICONTROL 保存更改]**.

## 配置要在敏捷故事板上的故事卡上显示的其他字段

将字段添加到故事卡时，字段为仅查看字段，并且仅在填充字段时才显示。

默认情况下，以下类型的数据会显示在任务和问题的故事卡上：

* 带有直接指向任务或问题的链接的新闻稿名称
* 带有直接项目链接的项目名称
* 此链接仅针对故事显示，不针对子任务显示
* 任务或问题描述
* 当前承诺
* 通过调整完成百分比本身或通过调整完成点数或小时数，查看和编辑完成百分比
* 已分配用户

您可以在故事卡上显示其他数据（包括自定义数据）。 出于各种原因，您可能希望在故事卡上显示其他字段。 例如，如果您正在开发周期内为多个客户处理故事，则可能需要显示客户ID，或者您可能需要显示项目开始日期或项目完成日期。

>[!NOTE]
>
>如果您在故事卡上使用自定义字段，则名称中不能包含句点（或点）。

配置分配给敏捷团队的故事卡以显示其他字段：

{{step1-to-team}}

1. 单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，键入字段名称以查找它。

   ![其他字段](assets/agile-additional-fields-kanban.png)

1. 选择要添加的字段的名称。
1. 键入 **[!UICONTROL 显示名称]** 以在故事或问题卡上显示的字段。
1. 单击 **[!UICONTROL 保存更改]**.

## 配置正在进行的工作(WIP)限制

在定义Kanban团队的WIP限制时，可以通过限制该团队当前处理的项目数来控制该团队当前处理的项目数。 [!UICONTROL 新建] 或 [!UICONTROL 进行中] 上的列 [!UICONTROL Kanban] 展示板。

在配置Kanban小组的WIP限制后，您可以查看WIP限制并从以下位置对其进行更新： [!UICONTROL Kanban] 敏捷故事板，如中所述 [管理上的正在进行的工作(WIP)限制 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

要限制Kanban团队的WIP，请执行以下操作：

{{step1-to-team}}

1. 单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Kanban团队。
1. 单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-menu.png)，然后选择 **[!UICONTROL 编辑]**.

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 方法]** 部分，确保选中Kanban。

1. 在 **[!UICONTROL 故事板]** 部分，在 **[!UICONTROL WIP限制]** 字段，指定每个列中允许的最大项数 [!UICONTROL Kanban] 敏捷故事板。 您可以为每个列设置不同的限制。 您可以为每个列设置的最大限制为100。\
   设置后，WIP限制会在 [!UICONTROL Kanban] 敏捷故事板任何时候超过故事板上任何列的限制。 此警告消息仅在第一次超出WIP限制时显示。 此警告消息不显示在任何具有相等状态的列上 [!UICONTROL 完成].\
   WIP限制只是一个视觉上的警告，不会限制您的团队在一列中拥有超过您设置的限制数量的项目。

   ![WIP限制](assets/wip-limit-350x193.png)

1. 单击 **保存更改**.

## 配置从积压自动添加故事

<!-- this functionality needs to be verified-->

您可以将积压中的故事配置为自动添加到 [!UICONTROL Kanban] 将项目从该列移动之后立即展示板。

{{step1-to-team}}

1. 单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Kanban团队。
1. 单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-menu.png)，然后选择 **[!UICONTROL 编辑]**.

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 选择 **[!UICONTROL 从积压自动添加下一个故事]** 配置积压中的下一个项自动添加到 **[!UICONTROL 新建]** 列(在将项目移出 **[!UICONTROL 进行中]** 列。

   用户必须启用 **显示积压** 设置 [!UICONTROL Kanban] 板使此功能生效。 当用户启用 [!UICONTROL 显示积压] 设置 [!UICONTROL Kanban板]，将会执行以下功能：

   每当故事从 [!UICONTROL 进行中] 栏插入故事板上的栏以表示 [!UICONTROL 完成] 状态（或等于以下内容的状态） [!UICONTROL 完成])，则积压栏中的故事会自动移至 [!UICONTROL 新建] 列 [!UICONTROL Kanban板].
从积压中添加时，具有最高优先级的故事会添加到故事板。

1. 单击 **[!UICONTROL 保存更改]**.

## 配置卡在上的停留时间 [!UICONTROL Kanban] 展示板

您可以选择已完成的卡片在 [!UICONTROL Kanban] 展示板。 流失的任务 [!UICONTROL Kanban] 仍然可以在原始项目中访问展示板。

{{step1-to-team}}

1. （可选）单击 **[!UICONTROL 切换团队]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Kanban团队或在搜索栏中搜索团队。
1. 选择Kanban团队。
1. 单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-menu.png) ，然后选择 **[!UICONTROL 编辑]**.

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL “已完成”卡片留在Kanban板上的天数]** 下拉菜单中，选择一个值。

   您可以选择1到30天之间的数字。
1. 单击 **[!UICONTROL 保存更改]**.
