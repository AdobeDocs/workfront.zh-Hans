---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 配置任务的完成按钮
description: 完成按钮可自动设置任务或问题的状态。 默认情况下，当被分配人单击其工作项上的完成时，Adobe Workfront将任务标记为已完成。
author: Jenny
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 为任务配置[!UICONTROL 完成]按钮

[!UICONTROL 完成]按钮可自动设置任务或问题的状态。 默认情况下，当被分派人在其工作项上单击“标记为完成”时，[!UICONTROL Adobe Workfront]将任务标记为[!UICONTROL 已完成]。

>[!NOTE]
>
>在Workfront的所有区域中，“完成”按钮显示为“标记为完成”。

## 概述

具有特定权限的用户可以配置[!UICONTROL Done]按钮以将其与系统中的特定状态相关联。 [!UICONTROL Done]按钮有两种方式适用于[!UICONTROL Workfront]中的任务：

* 如果用户已分配主团队，[!DNL Workfront]管理员或具有[!UICONTROL 计划]许可证的用户可以配置[!UICONTROL 完成]按钮以反映团队成员的特定状态。 请参阅本文中的[为团队[!UICONTROL 配置]完成](#configure-the-uicontrol-done-button-for-a-team)按钮。
* 如果用户没有[!UICONTROL 主团队]，但其配置文件中具有[!UICONTROL 其他团队]，则Workfront将搜索与该用户关联的任何团队上的[!UICONTROL 完成]按钮的设置。 选择是随机的，与任何团队关联的状态用于任务。
* 如果用户没有分配主团队，则任务的[!UICONTROL 完成]按钮与完成状态相关联。 此方案中没有可用的配置选项。 [!UICONTROL Done]按钮自动默认为此状态。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront包</p> </td> 
   <td>任何</td> 
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

## 为团队配置[!UICONTROL 完成]按钮

您可以使用[!UICONTROL 完成]按钮更改应用于工作项的状态。 您还可以设置多个状态，并允许用户选择合适的状态。

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后单击&#x200B;**[!UICONTROL 编辑]**。
1. 在&#x200B;**[!UICONTROL 团队设置]**&#x200B;页面的底部找到&#x200B;**[!UICONTROL 完成按钮]**&#x200B;部分。

1. 为每个工作项类型选择一个状态或多个状态。

   >[!NOTE]
   >
   >为任务或问题选择状态时，请考虑以下事项：
   >
   >* 如果您为每种类型的工作项选择一个状态，则当用户单击其项上的[!UICONTROL 完成]时，任务或问题状态将设置为该状态。 如果您为每种类型的工作项设置了多个状态，则会在[!UICONTROL 完成]按钮中添加一个下拉菜单，用户必须选择状态才能更改工作项的状态。
   >* 您只能将系统级状态与[!UICONTROL 完成]按钮相关联。 您无法将组特定的状态与工作项状态相关联。
   >* 当分配给该项的用户将该项置于与[!UICONTROL 完成]按钮关联的状态时，无论您选择的状态是[!UICONTROL 已完成]、[!UICONTROL 已关闭]还是工作状态，该项均显示该用户的[!UICONTROL 完成]。
   >   
   >   
   >  例如，将[!UICONTROL Done]按钮与[!UICONTROL In-Progress]关联会导致将状态从[!UICONTROL New]更改为[!UICONTROL In-Progress]的用户的工作项显示为[!UICONTROL Done]。
   >   
   >* 问题类型可自定义，并且它们的名称可能与您的环境中下面列出的不同。\
   >  以下是默认的任务和问题类型：
   >     
   >   * [!UICONTROL 任务]
   >   * [!UICONTROL 问题]
   >   * [!UICONTROL 请求]
   >   * [!UICONTROL 更改顺序]
   >   * [!UICONTROL 错误报告]

   如果将任务或问题分配给多个用户，则除了为您的团队选择的多个状态之外，您还会在下拉菜单中看到“[!UICONTROL 完成我的部分]”选项。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 将用户与主团队关联

若要使用户能够看到对[!UICONTROL 完成]按钮功能所做的更改，您可以让更改了用户主团队设置的团队。

要将用户与主团队关联，请执行以下操作：

1. 单击&#x200B;**[!UICONTROL 右上角的]**&#x200B;主菜单![](assets/main-menu-icon.png)图标[!DNL Adobe Workfront]。

1. 单击&#x200B;**[!UICONTROL 用户]**，然后选择要与主团队关联的一个或多个用户。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后单击&#x200B;**[!UICONTROL 编辑]**。\
   ![](assets/user-settings-nwe-350x291.png)

1. 在&#x200B;**[!UICONTROL 组织]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 主团队]**&#x200B;字段。 开始键入要将其设置与用户关联的团队的名称。 在列表中看到团队时，单击该团队的名称。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。\
   您选择的用户现在与主团队相关联。
这些用户现在可以看到任何团队设置，包括与[!UICONTROL 完成]按钮关联的状态。
