---
product-area: projects
navigation-topic: create-tasks
title: 创建子任务
description: 在Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设为子任务，可以在任务列表上创建子任务。 您还可以将子任务设为主任务。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: fb1f4e609e0cc2b0e9e4d0b36b7ace3fd8937d26
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 创建子任务

在Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设为子任务，可以在任务列表上创建子任务。 您还可以将子任务设为主任务。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关任务访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予对任务的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对项目和父任务具有“添加任务”或更高权限的参与权限</p> <p>创建任务后，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务 </a>. </p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建子任务

* [从任务列表创建子任务](#create-subtasks-from-the-task-list)
* [从任务子任务部分创建子任务](#create-subtasks-from-the-task-subtasks-section)

### 从任务列表创建子任务 {#create-subtasks-from-the-task-list}

1. 转到要创建子任务的项目。
1. 单击 **任务** 的子菜单。
1. （视情况而定）如果要执行子任务的任务尚未直接位于要执行父任务的任务下方，请将其拖动到任务列表中的适当位置。
1. 选择要执行子任务的任务，然后执行下列操作之一：

   * 单击 **缩进** 图标 ![](assets/indent-icon-nwe-33x29.png) 将所选任务作为其正上方任务的子任务。
   * 使用标准英语QWERTY键盘时，按键盘上的Option + >(Mac)或Alt + >(Windows)。 其他语言可能使用Option + 、(Mac)或Alt + 、(Windows)命令缩进。

      >[!TIP]
      >
      >在内联编辑中编辑任务时，键盘快捷键不起作用。 在这种情况下，使用缩进图标 ![](assets/cs1.png) 创建子任务。

   * 将任务拖放到要指定为父任务的任务上。
   >[!NOTE]
   >
   >仅当任务列表按任务编号排序，并且没有对任务列表应用分组时，才能缩进任务。

### 从任务子任务部分创建子任务 {#create-subtasks-from-the-task-subtasks-section}

1. 转到要创建子任务的项目。
1. 单击 **任务** 的子菜单。
1. 单击要在其中创建子任务的任务名称。
1. 单击 **子任务** 的子菜单。
1. 单击 **新任务。**

   按照以下文章中的步骤继续创建子任务： [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. 单击 **保存任务。**

## 将子任务设为主任务

1. 转到要将子任务设为主任务的项目。
1. 单击 **任务** 的子菜单。
1. 选择要执行主任务的子任务。
1. 单击 **外部** 图标 ![](assets/outdent-icon-nwe-31x29.png) 使子任务成为主任务。

   或

   在标准英语QWERTY键盘上，按Option + &lt;(Mac)或Alt + &lt;(Windows)。 其他语言可能使用Option +命令。 (Mac)或Alt + 。 (Windows)。

   >[!NOTE]
   >
   >仅当任务列表按任务编号排序，并且没有对任务列表应用分组时，才能生成任务。
