---
title: 将自定义条件设置为任务和问题的默认条件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 当用户单击“处理任务”或将更新注释添加到他们已分配到的新任务（无需手动为任务设置条件）时，Adobe Workfront会显示任务的默认条件（在“设置”中配置）。 问题也是如此。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 将自定义条件设置为任务和问题的默认条件

当用户单击“处理任务”或将更新注释添加到他们已分配到的新任务（无需手动为任务设置条件）时，Adobe Workfront会显示任务的默认条件（在“设置”中配置）。 问题也是如此。

Workfront使用内置条件“顺利进行”作为任务的默认条件，并单独用于问题。 作为Workfront管理员，您可以将这两种对象类型的默认条件更改为您创建的自定义条件。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将自定义条件设置为任务或问题的默认条件：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **条件**.

1. 单击 **任务** 或 **问题** 选项卡。

1. 单击 **设置默认条件**.
1. 在下拉菜单中，单击您希望作为任务（或问题）的默认条件的自定义条件。
1. 单击&#x200B;**保存**。

>[!NOTE]
>
>* 为任务或问题分配了权限，或者对其具有“管理”权限的用户，可以手动更改其条件。 有关更多信息，请参阅 [任务和问题的更新条件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Workfront附带的三个任务和问题的默认条件是：顺利进行、有些顾虑和主要障碍。 您无法隐藏或删除这些条件，但可以更改其名称和颜色。 或者，您也可以创建新受众以改用，如 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>


有关将自定义条件配置为项目默认条件的信息，请参阅 [将自定义条件设置为项目的默认条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

有关自定义条件的信息，请参阅 [自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
