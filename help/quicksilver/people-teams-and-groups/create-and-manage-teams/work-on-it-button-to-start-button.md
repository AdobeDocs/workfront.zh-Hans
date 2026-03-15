---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 将工作按钮替换为开始按钮
description: Adobe Workfront的默认配置包括一个工作按钮，用于显示分配给您的项目的任务和问题。
author: Courtney
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 2%

---

# 将[!UICONTROL 处理它]按钮替换为[!UICONTROL 开始]按钮

[!DNL Adobe Workfront]的默认配置包括[!UICONTROL 处理任务]按钮，用于显示分配给您的项目的任务和问题。 当您在分配给您的项目中单击[!UICONTROL 处理它]时，您会向其他用户发出信号，表示您已收到该工作并确认您将处理它。 但是，[!DNL Work On It]按钮不会更新任务或问题状态以指示工作已实际开始。

You can replace the [!DNL Work On It] button with a [!UICONTROL Start] button for a team you belong to. In this case, you click the [!UICONTROL Start] button instead of [!UICONTROL Work On It], which automatically updates the status and the [!UICONTROL Actual Start Date] of the work item, signaling that you started work. For information about the setting of which team might affect your changes in the [!UICONTROL Work On It] button, see the section [Configure the [!UICONTROL Start] button](#configure-the-uicontrol-start-button) in this article.

>[!IMPORTANT]
>
>Clicking the [!UICONTROL Start] button changes the item&#39;s status and [!UICONTROL Actual Start Date]. If someone else has started working on a task or issue (which changed the status to [!UICONTROL In Progress] and populated the [!UICONTROL Actual Start Date]), the button for the item displays as [!UICONTROL Work On It] even when a team you belong to has had the button replaced with a [!UICONTROL Start] button.

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 包</p> </td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Configure the [!UICONTROL Start] button

If you have a [!UICONTROL Plan] license, you can configure the [!UICONTROL Start] button for a team in the [!UICONTROL Edit] team window. Following is how the button works after it is enabled for a team:

* **The team is assigned to a work item**: If a team is assigned to the work item, members on that team see the [!UICONTROL Start] button and the statuses configured for that team.
* **The user belongs to a Home Team**: If no team is assigned to the work item but the user is assigned to a Home Team in their profile, then the user sees the [!UICONTROL Start] button and the statuses configured for that team. This is the scenario we recommend if you want users to use the [!UICONTROL Start] button frequently.
* **The user is assigned to a work item**: If there is no team assigned to the work item and no Home Team assigned to the user but the user is assigned to the work item, then the user sees the [!UICONTROL Start] button and the combined statuses configured for that all teams they are assigned to.
* **未将用户分配给任何团队：**&#x200B;如果没有为该工作项分配任何团队，也没有为该用户（包括主页团队）分配任何团队，并且该项目已分配给该用户，则该用户似乎是[!UICONTROL 处理它]按钮。

>[!NOTE]
>
>此功能当前在
>
>* [!DNL Workfront]移动应用程序
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront]个电子邮件通知
>

To configure the Start button:

{{step1-to-team}}

1. In the **[!UICONTROL Teams]** drop-down menu, select a team.\
   或\
   Click **[!UICONTROL Create new team]**.

1. Click the **[!UICONTROL More]** icon ![](assets/more-icon.png), then click **[!UICONTROL Edit]**.

1. Find the **[!UICONTROL Work On It]** button section near the bottom of the [!UICONTROL Edit Teams] page.
1. Select the **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]** check box.
1. 为每个工作项类型选择一个或多个状态。 如果选择多个状态，则单击“[!UICONTROL 开始]”时会显示一个下拉菜单，您可以在其中选择所需的状态。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。 为用户分配工作项后，用户现在会看到[!UICONTROL 启动任务]或[!UICONTROL 启动问题]按钮，而不是[!UICONTROL 处理它]按钮。

   >[!NOTE]
   >
   >我们建议将团队设置为用户的主页团队，以便在其所有已分配的工作项上显示“开始”按钮。 请参阅下面的[将用户与家庭团队关联](#associate-users-with-a-home-team)。

## Associate users with a Home Team

To associate users with a Home Team:

{{step-1-to-users}}

1. Select the user or users you want to associate with a Home Team.
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. In the **[!UICONTROL Organization]** section, select the **[!UICONTROL Home Team]** field. Start typing the name of the team whose settings you want to associate with the users. 在列表中看到团队时，单击该团队的名称。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。\
   您选择的用户现在与主页团队相关联。

   这些用户现在可以看到任何团队设置，包括与[!UICONTROL 完成]按钮关联的状态。

