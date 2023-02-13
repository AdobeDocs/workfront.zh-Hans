---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 将“Work On It（处理它）”按钮替换为“Start（开始）”按钮
description: Adobe Workfront的默认配置包括Work On It按钮，用于显示分配给您的项目的任务和问题。
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 替换 [!UICONTROL It工作] 按钮 [!UICONTROL 开始] 按钮

[!DNL Adobe Workfront]的默认配置包括 [!UICONTROL It工作] 按钮，以查看已分配给您的项目的任务和问题。 单击 [!UICONTROL It工作] 对于分配给您的项目，您会向其他用户发出信号，表示您收到了该工作，并确认您将会处理该工作。 但是， [!DNL Work On It] 按钮不会更新任务或发出状态以表示工作实际已开始。

您可以将 [!DNL Work On It] 按钮 [!UICONTROL 开始] 按钮。 在这种情况下，您单击 [!UICONTROL 开始] 按钮 [!UICONTROL It工作]，可自动更新状态和 [!UICONTROL 实际开始日期] ，表示您已开始工作。 有关设置哪个团队可能会在 [!UICONTROL It工作] 按钮，请参阅部分 [配置 [!UICONTROL 开始] 按钮](#configure-the-uicontrol-start-button) 在本文中。

>[!IMPORTANT]
>
>单击 [!UICONTROL 开始] 按钮更改项目的状态和 [!UICONTROL 实际开始日期]. 如果其他人已开始处理任务或问题(将状态更改为 [!UICONTROL 正在进行] 并填充 [!UICONTROL 实际开始日期])，则项目的按钮显示为 [!UICONTROL It工作] 即使您所属的团队已将按钮替换为 [!UICONTROL 开始] 按钮。

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
   <td> <p>计划</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 配置 [!UICONTROL 开始] 按钮

如果您有 [!UICONTROL 计划] 许可证，您可以配置 [!UICONTROL 开始] 按钮 [!UICONTROL 编辑] 团队窗口。 以下是为团队启用按钮后按钮的工作方式：

* **该团队被分配给工作项**:如果将团队分配给工作项，则该团队的成员将看到 [!UICONTROL 开始] 按钮以及为该团队配置的状态。
* **用户属于主团队**:如果没有为工作项分配任何团队，但在用户的配置文件中为用户分配了主团队，则用户会看到 [!UICONTROL 开始] 按钮以及为该团队配置的状态。 如果您希望用户使用 [!UICONTROL 开始] 按钮。
* **将用户分配到工作项**:如果没有为工作项分配团队，也没有为用户分配主团队，但为用户分配了工作项，则用户将看到 [!UICONTROL 开始] 按钮，以及为分配给的所有团队配置的组合状态。
* **未将用户分配给任何团队：** 如果没有为工作项分配团队，也没有为用户（包括主团队）分配团队，并且该项目已分配给用户，则用户似乎 [!UICONTROL It工作] 按钮。

>[!NOTE]
>
>此功能当前在
>
>* 的 [!DNL Workfront] 移动设备应用程序
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] 电子邮件通知
>


要配置“开始”按钮，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 团队]**.

1. 在 **[!UICONTROL 团队]** 下拉菜单中，选择一个团队。\
   或\
   单击 **[!UICONTROL 创建团队]**.

1. 单击 **[!UICONTROL 更多]** 图标 ![](assets/more-icon.png)，然后单击 **[!UICONTROL 编辑]**.

1. 查找 **[!UICONTROL It工作]** 按钮部分 [!UICONTROL 编辑团队] 页面。
1. 选择 **[!UICONTROL 将“Work On It（处理它）”按钮更改为“Start（开始）”按钮，以自动更新项目的状态]** 复选框。
1. 为每个工作项类型选择一个或多个状态。 如果选择多个状态，则单击时会显示一个下拉菜单 [!UICONTROL 开始] 其中，您可以选择所需的状态。
1. 单击 **[!UICONTROL 保存更改]**. 用户现在会看到 [!UICONTROL 启动任务] 或 [!UICONTROL 开始问题] 按钮，而不是 [!UICONTROL It工作] 按钮。

   >[!NOTE]
   >
   >我们建议将团队设置为用户的主团队，以便在他们分配的所有工作项目上显示“开始”按钮。 请参阅 [将用户与主团队关联](#associate-users-with-a-home-team) 下。

## 将用户与主团队关联

要将用户与主团队关联，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront].

1. 单击 **[!UICONTROL 用户]**，然后选择要与主团队关联的用户。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 在 **[!UICONTROL 组织]** 选择 **[!UICONTROL 主队]** 字段。 开始键入要与用户关联其设置的团队的名称。 当您在列表中看到团队时，请单击该团队的名称。

1. 单击 **[!UICONTROL 保存更改]**.\
   现在，您选择的用户已与主团队关联。

   任何团队设置，包括与 [!UICONTROL 完成] 按钮。

