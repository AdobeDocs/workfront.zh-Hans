---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: 管理Scrum展示板上的故事和问题
description: 您可以将故事或问题从Scrum展示板移动到另一个迭代或积压工作，或从Scrum展示板删除它。 删除文章或问题后，该文章或问题将被移动到回收站保留30天，只有系统管理员才能恢复。
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 管理[!UICONTROL Scrum]展示板上的故事和问题

您可以将故事或问题从[!UICONTROL Scrum]展示板移动到另一个迭代或积压工作，或从[!UICONTROL Scrum]展示板删除它。 删除文章或问题后，该文章或问题将被移动到回收站保留30天，只有系统管理员才能恢复。

要从开发周期中删除任务或问题而不将其删除或发送到积压，请转到项目并从分配列中删除敏捷团队。 这会从Scrum展示板中删除任务或问题，但它仍保留在项目中。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [!UICONTROL Standard]</p> 
   或
   <p>当前： [!UICONTROL Work]或更高版本</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[!UICONTROL Manage]对任务或问题的访问权限 </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从[!UICONTROL Scrum]展示板移动故事或问题

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择Scrum团队或在搜索栏中搜索团队。
1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
1. 单击文章或问题上的&#x200B;**[!UICONTROL 更多]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 移至]**。

   ![从Scrum展示板删除或移动故事](assets/scrum-delete-move-story.png)

1. 在确认消息上，选择以下任一选项：

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 其他迭代]</strong></td>
        <td>选择以将项目移动到另一个迭代，然后选择文章或问题将移动到哪个迭代。 如果未定义未来的小版本，则无法移动项目。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 积压]</strong></td>
        <td>选择以将故事或问题移动到团队的积压。</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >工作项[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]受[!UICONTROL 编辑团队]页面上的设置影响。 有关信息，请参阅[[!UICONTROL 配置Scrum]一文中的](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)配置[将工作项添加到迭代时，日期的应用方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)部分。

1. 单击&#x200B;**[!UICONTROL 移动]**。

## 从[!UICONTROL Scrum]讨论区中删除故事或问题

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择Scrum团队或在搜索栏中搜索团队。
1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
1. 单击文章或问题上的&#x200B;**[!UICONTROL 更多]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 删除文章]**&#x200B;或&#x200B;**[!UICONTROL 删除问题]**。

   ![从Scrum展示板删除或移动故事](assets/scrum-delete-move-story.png)

1. 在确认消息上，单击&#x200B;**[!UICONTROL 是，将其删除]**。
