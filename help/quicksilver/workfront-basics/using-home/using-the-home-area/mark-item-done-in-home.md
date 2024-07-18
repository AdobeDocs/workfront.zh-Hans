---
product-area: projects
navigation-topic: use-the-home-area
title: 在“主页”区域将项目标记为“完成”
description: 如果您是任务或问题受分配人，则可以将任务或问题标记为“已完成”。 将任务或问题标记为“完成”时，任务或问题的状态将更改为“完成”。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 在[!UICONTROL 主页]区域将项目标记为[!UICONTROL 完成]

如果您是任务或问题受分配人，则可以将任务或问题标记为“已完成”。 将任务或问题标记为[!UICONTROL 完成]时，任务或问题的状态将更改为[!UICONTROL 完成]。

>[!NOTE]
>
>除非您是分配给任务或问题的资源之一，否则不会看到[!UICONTROL 完成]按钮。

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

## 将任务或问题标记为[!UICONTROL 完成]

只有分配给任务或问题的用户可以将其标记为[!UICONTROL 完成]。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. 在&#x200B;**[!UICONTROL 工作列表]**&#x200B;中，找到任何等待处理的项目。
1. 执行以下任一操作：

* 在工作项上单击&#x200B;**[!UICONTROL 完成]**。\
   有关此按钮可能如何显示的更多详细信息，请参阅[了解[!UICONTROL 完成]按钮的选项](#understand-the-options-of-the-done-button)。

* 选择要标记为完成的项，然后在右侧面板中单击&#x200B;**[!UICONTROL 更新状态]**，然后将项的状态更改为等于[!UICONTROL 完成]或[!UICONTROL 已关闭]的状态。

## 了解[!UICONTROL 完成]按钮的选项

默认情况下，单击工作项上的[!UICONTROL 完成]按钮会将该项目的状态更改为[!UICONTROL 完成]（对于任务）或[!UICONTROL 已解决]（对于问题）。

您的[!DNL Adobe Workfront]管理员可以自定义与[!UICONTROL 完成]按钮关联的状态，并将这些自定义应用于您的主团队。

根据与[!UICONTROL Done]按钮关联的状态数或者分配给任务或问题的资源数，[!UICONTROL Done]按钮的外观可能会发生更改。

* [与一个状态关联的[!UICONTROL 完成]按钮](#done-button-associated-with-one-status)
* [与多个状态关联的[!UICONTROL 完成]按钮](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL 完成]按钮（针对分配给多个资源的项）](#done-button-for-items-assigned-to-multiple-resources)

### 与一个状态关联的[!UICONTROL 完成]按钮

当[!UICONTROL Done]按钮与一个状态关联并且工作项仅分配给您时，该按钮显示为&#x200B;**[!UICONTROL Done]**。 单击该按钮后，任务或问题的状态将更改为与[!UICONTROL 完成]按钮关联的状态。

![完成按钮](assets/Done.png)

要了解哪个状态与[!UICONTROL 完成]按钮关联，请按照[编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)中的说明，查看[!UICONTROL 完成按钮]部分的主团队[!UICONTROL 团队设置]。

如果您未分配到主团队，则在单击[!UICONTROL 完成]时将选择默认状态，如上文[了解[!UICONTROL 完成]按钮](#understand-the-options-of-the-done-button)的选项中所述。

### 与多个状态关联的[!UICONTROL 完成]按钮

当[!UICONTROL Done]按钮与多个状态关联时，该按钮显示&#x200B;**[!UICONTROL Done]**&#x200B;一词，后面是一个下拉菜单。 在此方案中，不能简单地单击[!UICONTROL 完成]。 您必须从下拉菜单中选择一个状态。 选择最适合完成工作项目的状态。 这样，您就可以更改工作项的状态。

要了解如何将多个状态与[!UICONTROL Done]按钮相关联，请参阅[为任务配置[!UICONTROL Done]按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)和[为问题配置[!UICONTROL Done]按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)。

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL 完成]按钮（针对分配给多个资源的项）

将任务或问题分配给多个资源时，按钮显示&#x200B;**[!UICONTROL 完成]**&#x200B;一词，其后是下拉菜单。 在下拉菜单中，您可以选择在&#x200B;**[!UICONTROL 完成我的部分]**（使团队成员知道您已完成您任务的一部分）或与[!UICONTROL 完成]按钮（完成项目）相关的状态之间选择。 选择&#x200B;**[!UICONTROL 完成我的部件]**&#x200B;后，该工作项将从您的工作列表中删除，但仍保留在那些仍分派给该工作项的工作列表内。\
如果“完成”按钮与多个状态关联，则它们列在&#x200B;**完成我的部件**&#x200B;下。

>[!NOTE]
>
>在具有多个受分配人的任务或问题上，每个用户负责指示其在任务或问题上的分配实际上已完成。 因此，每个被分配人都必须单击[!UICONTROL 完成]才能显示已完成分配给他们在项中的工作。

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
