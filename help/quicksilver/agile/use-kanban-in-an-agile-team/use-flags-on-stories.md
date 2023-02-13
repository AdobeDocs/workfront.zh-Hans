---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 在看板板上的文章中使用标记
description: 在 [!DNL Kanban] 展示板，标记提供了一个可视指示，指示文章何时准备好进入下一个状态。 这使看板团队在跨状态移动文章时能够使用“拉取”方法，而不是“推送”方法。
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 在 [!UICONTROL 看板] 展示板

在 [!DNL Kanban] 展示板，标记提供了一个可视指示，指示文章何时准备好进入下一个状态。 这将启用 [!UICONTROL 看板] 团队在跨状态移动文章时，会使用“拉取”方法，而不是“推送”方法。

**示例：** 请考虑以下团队使用“拉取”方法的示例：小组的平面设计师奥利维亚完成了她的工作，然后将故事标志设置为“[!UICONTROL 准备拉].&quot; 此标记可以直观地指示团队的撰稿人Tony，该文章已经准备好进入下一个状态。 然后，当托尼准备好开始处理时，他将故事转到下一个状态。

在文章中使用标记时，请考虑以下事项：

* 标记不是状态，而是一个可视指示，表示文章已准备好由团队的其他成员移至下一个状态。
* 标记不会显示在 [!UICONTROL 积压] 列或 [!UICONTROL 完成] 列(或在列的状态等于 [!UICONTROL 完成])。

   有关文章状态的更多信息，请参阅 [在看板板上的文章中使用标记](#updating-the-status-of-stories-and-subtasks)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 在 [!UICONTROL 看板] 展示板

要更改文章中的标记，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后选择新 [!UICONTROL 看板] 团队，或在搜索栏中搜索团队。

1. 转到 [!UICONTROL 看板] 要更改故事上的旗帜的展示板。
1. 展开文章拼贴以查看标记。\
   标记设置为 **[!UICONTROL 在轨]** 默认情况下，每个文章对应。\
   ![看板卡](assets/agile-storycard-kanban-2021-350x308.png)

1. 单击当前标记，然后从以下标记选项中选择：

   * **[!UICONTROL 在轨]:** 文章处于适当的状态，此时无需采取任何操作。\

      这是看板板上每个文章的默认标记。\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL 被阻止]:** 文章无法继续进入下一个状态。 在文章上设置此标志时，文章不计入WIP限制。 (有关WIP限制的详细信息，请参阅文章 [配置看板](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 准备拉]:** 文章已准备好，可由团队的其他成员移至下一个状态。\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
