---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: 在“主页”区域管理工作和团队请求
description: 当工作任务和问题分配给您时，它们会列在[!UICONTROL 主页]区域的[!UICONTROL 工作列表]中。 您可以查看、重新分配、回复、处理或删除请求。 [!UICONTROL 主页]区域的工作请求不限于与请求队列关联的问题。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# 在[!UICONTROL 主页]区域管理工作和团队请求

当工作任务和问题分配给您时，它们会列在[!UICONTROL 主页]区域的[!UICONTROL 工作列表]中。 您可以查看、重新分配、回复、处理或删除请求。 [!UICONTROL 主页]区域的工作请求不限于与请求队列关联的问题。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Edit]对任务和问题的访问权限</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>您需要处理的任务和问题的Contribute权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 查看工作请求

分配给您的工作请求将显示在[!UICONTROL 主页]的左侧面板中。 您可以使用[!UICONTROL 工作列表]顶部的筛选器配置[!UICONTROL 主页]中显示哪些请求。

您可以选择显示准备好处理的项目或您当前处理的项目的筛选器。

本文介绍如何使用[!UICONTROL 主页]区域中的筛选器查看您当前正在处理或可能考虑开始处理的项目。 有关[!UICONTROL 主页]区域中的所有筛选器的信息，请参阅[在[!UICONTROL 主页]区域](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)的工作列表中显示项目。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 单击&#x200B;**[!UICONTROL 筛选器]**&#x200B;下拉菜单。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 单击以下任一选项或两个选项执行任务：

   **[!UICONTROL 准备开始]：**&#x200B;仅显示准备开始的任务和问题。 以下两个语句都必须为true：

   * 这些任务及其父任务没有阻止它们进行处理的前置任务或任务限制。
   * 任务或问题的[!UICONTROL 计划开始日期]已过去或将在未来最多两周。

   **[!UICONTROL 未就绪]**：仅显示尚未准备开始的任务和问题。 以下任一语句必须为true：

   * 这些任务及其父任务可能具有阻止它们进行处理的前置任务或任务限制。
   * 任务或问题的计划开始日期[!UICONTROL 为超过两周的未来]。


1. 单击[!UICONTROL 任务]或[!UICONTROL 问题]下的&#x200B;**[!UICONTROL 处理]**&#x200B;以显示您当前处理的任务和问题。
1. 单击“[!UICONTROL 问题]”下的“**[!UICONTROL 已请求]**”可显示已向您请求（您已被分派给他们）但尚未接受处理的问题。

## 访问团队请求

您可以直接从[!UICONTROL 主页]区域访问分配给您团队的请求。 有关团队请求的更多信息，请参阅[团队请求概述](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md)。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;区域中，单击以展开&#x200B;**[!UICONTROL 团队请求]**&#x200B;分组。

   如果没有分配给团队的请求，则不会显示分组。

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. 单击团队名称。\
   **[!UICONTROL 团队请求]**&#x200B;部分显示并显示分配给您团队的所有请求。 有关处理团队请求的更多信息，请参阅[管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)。

## 重新分配请求

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;区域，选择要重新分配的请求。

1. 单击&#x200B;**[!UICONTROL 工作总揽]**&#x200B;构件并将您自己从请求中移除，然后键入要将该请求重新分配到的用户的名称。

   >[!TIP]
   >
   >如果工作请求仍然处于“准备开始”或“未就绪”状态，您可以使用[!UICONTROL 工作列表]的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单中的&#x200B;**[!UICONTROL 重新分配]**&#x200B;按钮。\
   >![重新分配按钮](assets/reassign-in-left-panel-350x204.png)

1. 如果任务的状态在完成后更改为[!UICONTROL 新建]或[!UICONTROL 进行中]，您必须取消分配用户，保存任务，然后重新分配用户，任务才能重新出现在其“主页工作列表”中。

## 回复请求

您可以回复进一步澄清请求或建议一个新日期的请求。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;区域，选择要回复的请求。
1. 找到为您分配请求的个人。

   您可以在任务的[!UICONTROL 更新]选项卡上找到此信息。 确保启用了&#x200B;**[!UICONTROL 显示系统更新]**&#x200B;选项。

1. 单击&#x200B;**[!UICONTROL 开始新更新]**&#x200B;并开始键入您的回复。
1. 在&#x200B;**[!UICONTROL 通知]**&#x200B;框中输入收件人的名称，然后单击&#x200B;**[!UICONTROL 更新]**。

   >[!TIP]
   >
   >如果工作请求仍然处于“准备开始”或[!UICONTROL 未就绪]状态，您可以使用[!UICONTROL 工作列表]的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单中的&#x200B;**[!UICONTROL 回复]**&#x200B;按钮。\
   >![[!UICONTROL 回复按钮]](assets/reassign-in-left-panel-350x204.png)   >

## 处理请求

单击[!UICONTROL 处理]按钮时，您将向提交请求的用户以及可能分配到请求的任何其他用户指示您将开始处理该请求。 有关处理请求的更多信息，请参阅[管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;区域，选择要处理的请求，然后单击&#x200B;**[!UICONTROL 处理该请求]**。\
   右侧面板中将显示有关问题的信息。

## 删除请求

如果您决定不处理该请求，您可以将任务或问题转换回请求或将其从列表中移除。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;中，指向等待处理的项。
1. 单击&#x200B;**[!UICONTROL 工作总揽]**&#x200B;构件并自行删除。 这会从您的工作列表中移除该工作项。 如果请求未分配给任何其他团队或工作角色，则请求将保留未分配。

   或

   单击[!UICONTROL 主页工作]列表中任务或问题名称右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单图标![](assets/more-icon.png)。

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 从以下选项中选择：

   * **[!UICONTROL 转换为工作请求]：**&#x200B;选择此选项以将工作项转换回工作请求。\

     工作项将转换回请求，并且您仍然会分配到请求。\
      您稍后可以通过再次单击&#x200B;**[!UICONTROL 处理该请求]**&#x200B;来接受请求。

   * **[!UICONTROL 删除]：**&#x200B;选择此选项可从[!UICONTROL 工作列表]中删除请求。\

     您已从请求中取消分配，该请求不再与[!DNL Adobe Workfront]中的您的名称相关联。\
      如果请求未分配给任何其他团队或工作角色，则请求将保留未分配。
