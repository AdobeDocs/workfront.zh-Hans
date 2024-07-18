---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 将“处理此项工作”按钮替换为“开始”按钮
description: Adobe Workfront的默认配置包括“处理此项工作”按钮，用于显示分配给您的项目的任务和问题。
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 将[!UICONTROL 处理]按钮替换为[!UICONTROL 开始]按钮

[!DNL Adobe Workfront]的默认配置包括[!UICONTROL 处理此项工作]按钮，用于显示已分配给您的项目的任务和问题。 在分配给您的项目上单击[!UICONTROL 处理它]时，您向其他用户发出信号，表明您收到了该工作并承认您将处理它。 但是，[!DNL Work On It]按钮不会更新任务或问题状态以指示工作实际上已开始。

您可以将[!DNL Work On It]按钮替换为您所属的团队的[!UICONTROL 开始]按钮。 在这种情况下，您单击[!UICONTROL 开始]按钮而不是[!UICONTROL 处理它]，这会自动更新工作项的状态和[!UICONTROL 实际开始日期]，表示您已开始工作。 有关哪个团队的设置可能会影响您在[!UICONTROL 处理它]按钮中所做更改的信息，请参阅本文中的[配置[!UICONTROL 开始]按钮](#configure-the-uicontrol-start-button)部分。

>[!IMPORTANT]
>
>单击[!UICONTROL 开始]按钮会更改项目的状态和[!UICONTROL 实际开始日期]。 如果其他人已开始处理任务或问题（将状态更改为[!UICONTROL 进行中]并填充了[!UICONTROL 实际开始日期]），则即使您所属的团队已将该按钮替换为[!UICONTROL 开始]按钮，该项目的按钮也会显示为[!UICONTROL 处理该项目]。

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
   <td> <p>计划</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划或许可证类型，请与[!DNL Workfront]管理员联系。

## 配置[!UICONTROL 启动]按钮

如果您拥有[!UICONTROL 计划]许可证，则可以在[!UICONTROL 编辑]团队窗口中为团队配置[!UICONTROL 开始]按钮。 为团队启用按钮后，该按钮的工作方式如下所示：

* **团队已分配给工作项**：如果团队已分配给工作项，则该团队的成员将看到[!UICONTROL 开始]按钮和为该团队配置的状态。
* **用户属于主团队**：如果未将任何团队分配给工作项，但用户在其配置文件中分配给了主团队，则用户会看到[!UICONTROL 开始]按钮和为该团队配置的状态。 如果您希望用户经常使用[!UICONTROL 开始]按钮，我们建议采用这种方案。
* **用户已分配到工作项**：如果没有团队分配到工作项，也没有主团队分配到用户，但用户分配到工作项，则用户会看到[!UICONTROL 开始]按钮以及为用户分配到的所有团队配置的组合状态。
* **用户未分配给任何团队：**&#x200B;如果没有团队分配给工作项，并且用户没有团队（包括主团队），并且该项分配给用户，则用户似乎显示[!UICONTROL 处理此项工作]按钮。

>[!NOTE]
>
>此功能当前在中不可用
>
>* [!DNL Workfront]移动应用
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront]电子邮件通知
>

配置“开始”按钮：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 团队]**。

1. 在&#x200B;**[!UICONTROL 团队]**&#x200B;下拉菜单中，选择一个团队。\
   或\
   单击&#x200B;**[!UICONTROL 创建团队]**。

1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;图标![](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 编辑]**。

1. 在[!UICONTROL 编辑团队]页面底部附近找到&#x200B;**[!UICONTROL 处理此工作]**&#x200B;按钮部分。
1. 选中&#x200B;**[!UICONTROL 将“处理此项工作”按钮更改为“开始”按钮以自动更新项]**&#x200B;的状态。
1. 为每个工作项类型选择一个或多个状态。 如果选择多个状态，则单击[!UICONTROL 开始]时会显示一个下拉菜单，您可以在其中选择所需的状态。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。 用户现在在分配工作项时看到[!UICONTROL 开始任务]或[!UICONTROL 开始问题]按钮，而不是[!UICONTROL 处理它]按钮。

   >[!NOTE]
   >
   >我们建议将团队设置为用户的主团队，以便在其所有分配的工作项上显示“开始”按钮。 请参阅下面的[将用户与主团队关联](#associate-users-with-a-home-team)。

## 将用户与主团队关联

要将用户与主团队关联，请执行以下操作：

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**[!UICONTROL 用户]**，然后选择要与主团队关联的一个或多个用户。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. 在&#x200B;**[!UICONTROL 组织]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 主团队]**&#x200B;字段。 开始键入要将其设置与用户关联的团队的名称。 在列表中看到团队时，单击该团队的名称。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。\
   您选择的用户现在与主团队相关联。

   这些用户现在可以看到任何团队设置，包括与[!UICONTROL 完成]按钮关联的状态。

