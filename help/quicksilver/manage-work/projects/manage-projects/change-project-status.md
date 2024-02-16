---
product-area: projects
navigation-topic: manage-projects
title: 更改项目的状态
description: 如果需要，您可以手动将项目的状态更新为任何其他状态。 仅当项目的“完成模式”设置为“手动”时，您才可以手动将项目的状态更新为等于“完成”的状态。
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 7363e86f5c507e40955e16843c6776777c7ad823
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 更改项目的状态

<!--Audited: 02/2024-->

如果需要，您可以手动将项目的状态更新为任何其他状态。

仅当项目的“完成模式”设置为“手动”时，您才可以手动将项目的状态更新为等于“完成”的状态。

否则，Adobe Workfront会在项目的所有任务和问题完成并审批后将项目自动标记为完成。

有关项目完成模式的详细信息，请参阅 [编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准 </p> 
   或
   <p>当前：计划 </p>
   </td> 
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

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 有关更新到特定状态的注意事项

* **将项目更新为完成时：** 确保已完成项目中的所有任务和问题。 当项目中存在未完成的任务或问题时，您无法选择项目的“完成”状态或任何其他等于“完成”的状态。 这包括批准任何处于“完成 — 未决批准”状态的任务或问题。
* **将项目从“完成”更新为“当前”时：** 如果项目中的所有任务和问题均已完成，请确保将项目的完成模式设置为手动。 如果项目的完成模式为自动，则项目的状态保持为完成。

## 更改项目状态

1. 转到要更新其状态的项目。
1. 在项目标题中，单击以下位置中状态的名称： **状态** 字段，然后选择新状态。

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   或

   单击 **更多** 菜单 ![](assets/qs-more-menu.png) 单击项目名称旁边的，然后单击 **编辑** 并在 **状态** 字段，然后单击 **保存**.

   项目状态将更新为您选择的状态。
