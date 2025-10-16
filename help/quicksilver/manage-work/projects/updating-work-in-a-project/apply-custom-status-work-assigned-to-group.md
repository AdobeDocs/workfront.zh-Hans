---
product-area: projects
navigation-topic: update-work-in-a-project
title: 将状态应用于与组关联的工作
description: 如果项目与组关联，则您可以将系统级别状态以及与该组关联的自定义状态应用到该项目上的项目、任务或问题。
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# 将状态应用于与组关联的工作

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

如果项目与组关联，您可以将系统级别状态以及与该组关联的自定义状态应用到项目，或应用该项目上的任务和问题。 有关Adobe Workfront中组状态的信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

>[!TIP]
>
>您只能将项目与组关联。 问题和任务从所属的项目继承组。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 更新项目组和状态

当您更新项目的组时，任务、问题或项目的状态可用的选项将更改为匹配组。

1. 转至项目或创建新项目，如[创建项目](../../../manage-work/projects/create-projects/create-project.md)中所述。
1. 单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**编辑**。

1. 在显示的&#x200B;**编辑项目**&#x200B;框中（靠近&#x200B;**概述**&#x200B;部分的底部），从&#x200B;**组**&#x200B;下拉菜单中选择组。

1. 在&#x200B;**状态**&#x200B;下拉菜单中，选择自定义状态。

   >[!NOTE]
   >
   >如果在&#x200B;**组**&#x200B;下拉菜单中选择其他组，则&#x200B;**状态**&#x200B;菜单中的自定义状态会自动更改以与新组关联。
   >
   >
   >![状态下拉列表已展开为项目](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)的自定义状态
   >

1. 选择项目的状态。 您创建并应用于该组的自定义状态将显示在列表中。
