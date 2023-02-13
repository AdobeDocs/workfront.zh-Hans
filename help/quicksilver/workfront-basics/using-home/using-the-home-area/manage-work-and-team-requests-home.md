---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 在主页区域中管理工作和团队请求
description: 将工作任务和问题分配给您后，将列在 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 的上界。 您可以查看、重新分配、回复、处理或删除请求。 在 [!UICONTROL 主页] 区域不限于与请求队列相关的问题。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# 在 [!UICONTROL 主页] 面积

将工作任务和问题分配给您后，将列在 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 的上界。 您可以查看、重新分配、回复、处理或删除请求。 在 [!UICONTROL 主页] 区域不限于与请求队列相关的问题。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Edit]对任务和问题的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>为您需要处理的任务和问题提供权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 查看工作请求

分配给您的工作请求将显示在 [!UICONTROL 主页]. 您可以配置在中显示哪些请求 [!UICONTROL 主页] 使用位于 [!UICONTROL 工作列表].

您可以选择显示已准备好处理的项目或您当前正在处理的项目的过滤器。

本文介绍了如何在 [!UICONTROL 主页] 区域查看您当前正在处理或可能考虑开始处理的项目。 有关 [!UICONTROL 主页] 区域，请参阅 [在 [!UICONTROL 主页] 面积](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 过滤器]** 下拉菜单。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 单击以下任务选项之一或两者：

   **[!UICONTROL 准备开始]:** 仅显示已准备好启动的任务和问题。 以下两个语句必须都为true:

   * 这些任务及其父代没有前任或任务约束，无法处理这些任务。
   * 的 [!UICONTROL 计划开始日期] 这些任务或问题在过去或将来两周内完成。

   **[!UICONTROL 未就绪]**:仅显示尚未准备好启动的任务和问题。 以下任一语句必须为true:

   * 这些任务及其父代可能具有前任或任务约束，以阻止他们进行工作。
   * 任务或问题具有 [!UICONTROL 计划开始日期] 未来超过两周。



1. 单击 **[!UICONTROL 处理]** 在 [!UICONTROL 任务] 或 [!UICONTROL 问题] 以显示您当前正在处理的任务和问题。
1. 单击 **[!UICONTROL 请求]** 在 [!UICONTROL 问题] 显示您请求（您已分配给他们）但您尚未接受处理的问题。

## 访问团队请求

您可以直接从 [!UICONTROL 主页] 的上界。 有关团队请求的更多信息，请参阅 [团队请求概述](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]** 区域，单击可展开 **[!UICONTROL 团队请求]** 分组。

   如果没有为团队分配请求，则不会显示分组。

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. 单击团队名称。\
   的 **[!UICONTROL 团队请求]** 部分会显示并显示分配给您团队的所有请求。 有关处理团队请求的更多信息，请参阅 [管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 重新分配请求

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]** 区域，选择要重新分配的请求。

1. 单击 **[!UICONTROL 分配]** 小组件，然后从请求中删除您自己，然后键入要将请求重新分配到的用户名称。

   >[!TIP]
   >
   >如果工作请求仍处于“准备开始”或“未准备就绪”状态，则可以使用 **[!UICONTROL 重新分配]** 按钮 **[!UICONTROL 更多]** 菜单 [!UICONTROL 工作列表].\
   >![“重新分配”按钮](assets/reassign-in-left-panel-350x204.png)

1. 如果任务的状态更改为 [!UICONTROL 新建] 或 [!UICONTROL 正在进行] 完成后，必须取消分配用户，保存任务，然后重新分配用户，以便该任务在其“主页工作列表”中重新显示。

## 回复请求

您可以回复进一步阐明请求或提出新日期的请求。

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]** 区域，选择要回复的请求。
1. 找到向您分配请求的个人。

   您可以在 [!UICONTROL 更新] 选项卡。 确保选项 **[!UICONTROL 显示系统更新]** 启用。

1. 单击 **[!UICONTROL 开始新更新]** 然后开始键入您的回复。
1. 在 **[!UICONTROL 通知]** 框，然后单击 **[!UICONTROL 更新]**.

   >[!TIP]
   >
   >如果工作请求仍处于“准备开始”或 [!UICONTROL 未就绪] 状态，您可以使用 **[!UICONTROL 回复]** 按钮 **[!UICONTROL 更多]** 菜单 [!UICONTROL 工作列表].\
   >![[!UICONTROL “回复”按钮]](assets/reassign-in-left-panel-350x204.png)   >

## 处理请求

当您单击 [!UICONTROL It工作] 按钮，则您会向提交请求的用户以及可能被分配给您将要开始处理请求的任何其他用户指示。 有关处理请求的更多信息，请参阅  [管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]** ，选择要处理的请求，然后单击 **[!UICONTROL It工作]**.\
   有关问题的信息显示在右侧面板中。

## 删除请求

如果您决定不处理请求，则可以将任务或问题转换回请求，或将其从列表中删除。

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]**，指向待处理的项目。
1. 单击 **[!UICONTROL 分配]** 小组件，把自己拿下。 这会从工作列表中删除工作项。 如果请求未分配给其他人或其他团队或作业角色，则请求将被保留为未分配。

   或

   单击 **[!UICONTROL 更多]** 菜单图标 ![](assets/more-icon.png) 中任务或问题名称的权限 [!UICONTROL 家庭工作] 列表。

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 从以下选项中进行选择：

   * **[!UICONTROL 转换为工作请求]:** 选择此选项可将工作项转换为工作请求。\

      工作项将转换回请求，并且您仍然被分配给请求。\
      您可以稍后通过单击 **[!UICONTROL 处理它]** 再次。

   * **[!UICONTROL 删除]:** 选择此选项可从 [!UICONTROL 工作列表].\

      您未从请求中分配，并且该请求不再与 [!DNL Adobe Workfront].\
      如果请求未分配给其他人或其他团队或作业角色，则请求将被保留为未分配。
