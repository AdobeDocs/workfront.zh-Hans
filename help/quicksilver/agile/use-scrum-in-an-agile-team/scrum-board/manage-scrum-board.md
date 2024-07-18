---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: 管理Scrum展示板上的故事和问题
description: 您可以将故事或问题从Scrum展示板移动到另一个迭代或积压工作，或从Scrum展示板删除它。 删除文章或问题后，该文章或问题将被移动到回收站保留30天，只有系统管理员才能恢复。
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 管理[!UICONTROL Scrum]展示板上的故事和问题

您可以将故事或问题从[!UICONTROL Scrum]展示板移动到另一个迭代或积压工作，或从[!UICONTROL Scrum]展示板删除它。 删除文章或问题后，该文章或问题将被移动到回收站保留30天，只有系统管理员才能恢复。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Manage]对任务或问题的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 从[!UICONTROL Scrum]展示板移动故事或问题

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 团队]**。
1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择Scrum团队或在搜索栏中搜索团队。
1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
1. 单击文章或问题上的&#x200B;**[!UICONTROL 更多]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 移至]**。

   ![从Scrum展示板删除或移动故事](assets/scrum-delete-move-story.png)

1. 在确认消息上，选择以下任一选项：

   <table style="table-layout:auto">
    <tr>
        <td><strong>[！UICONTROL其他迭代]</strong></td>
        <td>选择以将项目移动到另一个迭代，然后选择文章或问题将移动到哪个迭代。 如果未定义未来的小版本，则无法移动项目。</td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL积压]</strong></td>
        <td>选择以将故事或问题移动到团队的积压。</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >工作项[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]受[!UICONTROL 编辑团队]页面上的设置影响。 有关信息，请参阅[配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[[!UICONTROL 配置]将工作项添加到迭代时，日期的应用方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)部分。

1. 单击&#x200B;**[!UICONTROL 移动]**。

## 从[!UICONTROL Scrum]讨论区中删除故事或问题

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 团队]**。
1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择Scrum团队或在搜索栏中搜索团队。
1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
1. 单击文章或问题上的&#x200B;**[!UICONTROL 更多]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 删除文章]**&#x200B;或&#x200B;**[!UICONTROL 删除问题]**。

   ![从Scrum展示板删除或移动故事](assets/scrum-delete-move-story.png)

1. 在确认消息上，单击&#x200B;**[!UICONTROL 是，将其删除]**。
