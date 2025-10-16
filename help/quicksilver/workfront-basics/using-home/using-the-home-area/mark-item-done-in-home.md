---
product-area: projects
navigation-topic: use-the-home-area
title: 在“主页”区域将项目标记为“完成”
description: 如果您是任务或问题受分配人，则可以将任务或问题标记为“已完成”。 将任务或问题标记为“完成”时，任务或问题的状态将更改为“完成”。
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# 在[!UICONTROL 主页]区域将项目标记为[!UICONTROL 完成]

如果您是任务或问题受分配人，则可以将任务或问题标记为“已完成”。 将任务或问题标记为[!UICONTROL 完成]时，任务或问题的状态将更改为[!UICONTROL 完成]。

>[!NOTE]
>
>除非您是分配给任务或问题的资源之一，否则不会看到[!UICONTROL 完成]按钮。

+++ 展开以查看本文中各项功能的访问要求。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> 
   <p>标准</p>
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL Edit]对任务和问题的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>Contribute权限或更高权限可为您需要处理的任务和问题提供内容</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在我的工作小部件中将工作项标记为“已完成”

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）单击&#x200B;**自定义**&#x200B;以添加&#x200B;**我的工作**&#x200B;小组件。
1. 找到工作项，然后在工作项上单击&#x200B;**[!UICONTROL 标记为完成]**。
有关此按钮可能如何显示的更多详细信息，请参阅[了解[!UICONTROL 完成]按钮的选项](#understand-the-options-of-the-done-button)。
   ![我的工作标记为“完成”](assets/my-work-done.png)


## 在“摘要”面板中将工作项标记为“完成”

您可以使用摘要面板，在我的任务和我的问题小组件中将工作项标记为已完成。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）单击&#x200B;**自定义**&#x200B;以添加&#x200B;**我的任务**&#x200B;或&#x200B;**我的问题**&#x200B;小组件。
1. 将鼠标悬停在工作项上，然后单击&#x200B;**摘要**图标。
   ![打开摘要](assets/open-summary-new-home.png)
1. 单击摘要面板顶部的&#x200B;**标记为完成**。


## 了解[!UICONTROL 完成]按钮的选项

默认情况下，单击工作项上的[!UICONTROL 完成]按钮会将该项目的状态更改为[!UICONTROL 完成]（对于任务）或[!UICONTROL 已解决]（对于问题）。

您的[!DNL Adobe Workfront]管理员可以自定义与[!UICONTROL 完成]按钮关联的状态，并将这些自定义应用于您的主团队。

根据与[!UICONTROL Done]按钮关联的状态数或者分配给任务或问题的资源数，[!UICONTROL Done]按钮的外观可能会发生更改。

* [与一个状态关联的[!UICONTROL 完成]按钮](#done-button-associated-with-one-status)
* [与多个状态关联的[!UICONTROL 完成]按钮](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL 完成]按钮（针对分配给多个资源的项）](#done-button-for-items-assigned-to-multiple-resources)

### 与一个状态关联的[!UICONTROL 完成]按钮

当[!UICONTROL Done]按钮与一个状态关联并且工作项仅分配给您时，该按钮显示为&#x200B;**[!UICONTROL Done]**。 单击该按钮后，任务或问题的状态将更改为与[!UICONTROL 完成]按钮关联的状态。

![完成按钮](assets/done-button-status.png)

要了解哪个状态与[!UICONTROL 完成]按钮关联，请按照[!UICONTROL 编辑团队设置]中的说明，查看[!UICONTROL 完成按钮]部分的主团队[团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)。

如果您未分配到主团队，则在单击[!UICONTROL 完成]时将选择默认状态，如上文[了解[!UICONTROL 完成]按钮](#understand-the-options-of-the-done-button)的选项中所述。

### 与多个状态关联的[!UICONTROL 完成]按钮

当[!UICONTROL Done]按钮与多个状态关联时，该按钮显示&#x200B;**[!UICONTROL Done]**&#x200B;一词，后面是一个下拉菜单。 在此方案中，不能简单地单击[!UICONTROL 完成]。 您必须从下拉菜单中选择一个状态。 选择最适合完成工作项目的状态。 这样，您就可以更改工作项的状态。

要了解如何将多个状态与[!UICONTROL Done]按钮相关联，请参阅[为任务配置[!UICONTROL Done]按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)和[为问题配置[!UICONTROL Done]按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)。

### [!UICONTROL 完成]按钮（针对分配给多个资源的项）

将任务或问题分配给多个资源时，按钮显示&#x200B;**[!UICONTROL 完成]**&#x200B;一词，其后是下拉菜单。 在下拉菜单中，您可以选择在&#x200B;**[!UICONTROL 完成我的部分]**（使团队成员知道您已完成您任务的一部分）或与[!UICONTROL 完成]按钮（完成项目）关联的状态之间选择。 选择&#x200B;**[!UICONTROL 完成我的部件]**&#x200B;后，该工作项将从您的工作列表中删除，但仍保留在那些仍分派给该工作项的工作列表内。\
如果“完成”按钮与多个状态关联，则它们列在&#x200B;**完成我的部件**&#x200B;下。

>[!NOTE]
>
>在具有多个受分配人的任务或问题上，每个用户负责指示其在任务或问题上的分配实际上已完成。 因此，每个被分配人都必须单击[!UICONTROL 完成]才能显示已完成分配给他们在项中的工作。

![完成我的部分](assets/done-with-my-part.png)

