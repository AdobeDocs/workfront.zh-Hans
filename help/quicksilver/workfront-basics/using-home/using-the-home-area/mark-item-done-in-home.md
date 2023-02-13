---
product-area: projects
navigation-topic: use-the-home-area
title: 在“主页”区域中将项目标记为“完成”
description: 如果您是任务或问题受分派人，则可以将任务或问题标记为完成。 将任务或问题标记为完成时，任务或问题的状态将更改为完成。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 将项目标记为 [!UICONTROL 完成] 在 [!UICONTROL 主页] 面积

如果您是任务或问题受分派人，则可以将任务或问题标记为完成。 将任务或问题标记为 [!UICONTROL 完成]，则任务或问题的状态将更改为 [!UICONTROL 完成].

>[!NOTE]
>
>您看不到 [!UICONTROL 完成] 按钮，除非您是分配给任务或问题的资源之一。

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

## 将任务或问题标记为 [!UICONTROL 完成]

只有分配给任务或问题的用户才能将其标记为 [!UICONTROL 完成].

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 在 **[!UICONTROL 工作列表]**，找到要处理的任何项目。
1. 执行以下任一操作：

* 单击 **[!UICONTROL 完成]** 在工作项上。\
   请参阅 [了解 [!UICONTROL 完成] 按钮](#understand-the-options-of-the-done-button) 有关此按钮显示方式的更多详细信息。

* 选择要标记为完成的项目，然后在右侧面板中，单击 **[!UICONTROL 更新状态]**，然后将项目的状态更改为等于 [!UICONTROL 完成] 或 [!UICONTROL 已关闭].

## 了解 [!UICONTROL 完成] 按钮

默认情况下，单击 [!UICONTROL 完成] 按钮将该项目的状态更改为 [!UICONTROL 完成] （对于任务）或 [!UICONTROL 已解决] （对于问题）。

您的 [!DNL Adobe Workfront] 管理员可以自定义与哪些状态关联 [!UICONTROL 完成] 按钮，并将这些自定义项应用于您的主团队。

取决于与 [!UICONTROL 完成] 按钮或为任务或问题分配的资源数，以及显示的内容 [!UICONTROL 完成] 按钮。

* [[!UICONTROL 完成] 与一个状态关联的按钮](#done-button-associated-with-one-status)
* [[!UICONTROL 完成] 与多个状态关联的按钮](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL 完成] 按钮，用于分配给多个资源的项目](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL 完成] 与一个状态关联的按钮

当 [!UICONTROL 完成] 按钮与一个状态关联，并且工作项仅分配给您，此按钮将读取 **[!UICONTROL 完成]**. 单击该任务时，任务或问题的状态将更改为与 [!UICONTROL 完成] 按钮。

![“完成”按钮](assets/Done.png)

要了解与 [!UICONTROL 完成] 按钮，请选中 [!UICONTROL 团队设置] 您的家庭团队 [!UICONTROL “完成”按钮] 部分，如 [编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

如果未将您分配给主团队，则在单击 [!UICONTROL 完成]，如上所述 [了解 [!UICONTROL 完成] 按钮](#understand-the-options-of-the-done-button).

### [!UICONTROL 完成] 与多个状态关联的按钮

当 [!UICONTROL 完成] 按钮可显示单词 **[!UICONTROL 完成]** 下拉菜单中。 在此方案中，您不能简单地单击 [!UICONTROL 完成]. 您必须从下拉菜单中选择状态。 选择最适合工作项完成状态。 通过执行此操作，您将更改工作项的状态。

要了解如何将多个状态与 [!UICONTROL 完成] 按钮，请参阅 [配置 [!UICONTROL 完成] “任务”按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) 和 [配置 [!UICONTROL 完成] 问题按钮](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL 完成] 按钮，用于分配给多个资源的项目

将任务或问题分配给多个资源后，按钮会显示单词 **[!UICONTROL 完成]** 下拉菜单中。 在下拉菜单中，您可以选择在 **[!UICONTROL 完成我的任务]** （可让团队成员知道您已完成部分任务）或与 [!UICONTROL 完成] 按钮（用于完成项目）。 在选择 **[!UICONTROL 完成我的任务]**，则会从工作列表中删除该工作项，但该工作项会保留在仍分配给该工作项的工作列表中。\
如果完成按钮与多个状态关联，则它们将列在 **完成我的任务**.

>[!NOTE]
>
>对于多个受分配者的任务或问题，每个用户都有责任指明他们自己对任务或问题的分配已实际完成。 因此，每个代理人必须单击 [!UICONTROL 完成] 以显示他们已完成在项目上分配给他们的工作。

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
