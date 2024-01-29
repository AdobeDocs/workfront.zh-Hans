---
product-area: projects
navigation-topic: create-tasks
title: 创建子任务
description: 在Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设置为子任务，可以在任务列表中创建子任务。 您还可以将子任务设置为主任务。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 创建子任务

<!-- Audited: 1/2024 -->

在Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设置为子任务，可以在任务列表中创建子任务。 您还可以将子任务设置为主任务。

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新增：标准</p>
   <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>向项目和父任务分配权限，并可添加任务或更高版本</p> <p>在创建任务后，您会自动收到该任务的“管理”权限。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 创建子任务

您可以从任务列表或任务子任务部分创建子任务。

### 从任务列表创建子任务 {#create-subtasks-from-the-task-list}

1. 转到要创建子任务的项目。
1. 单击 **任务** 部分。
1. （视情况而定）如果要生成子任务的任务尚未位于要生成父任务的任务的正下方，请将其拖动到任务列表中的适当位置。
1. 选择要创建子任务的任务，然后执行以下操作之一：

   * 单击 **缩进** 图标 ![](assets/indent-icon-nwe-33x29.png) 使所选任务成为其正上方的任务的子任务。
   * 使用标准英语QWERTY键盘时，按键盘上的Option + > (Mac)或Alt + > (Windows)。 其他语言可能使用命令Option + 、 (Mac)或Alt + 、 (Windows)进行缩进。

     >[!TIP]
     >
     >在内联编辑中编辑任务时，键盘快捷键不起作用。 在这种情况下，请使用“缩进”图标 ![](assets/cs1.png) 创建子任务。

   * 将任务拖放到要指定为父级任务的任务上。

     >[!NOTE]
     >
     >仅当任务列表按任务编号排序并且任务列表未应用分组时，您才可以缩进任务。

### 从任务的“子任务”部分创建子任务 {#create-subtasks-from-the-task-subtasks-section}

1. 转到要创建子任务的项目。
1. 单击 **任务** 部分。
1. 单击要在其中创建子任务的任务的名称。
1. 单击 **子任务** 部分。
1. 单击 **新建任务。**

   请按照下文中介绍的步骤继续创建子任务： [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. 单击 **保存任务。**

## 将子任务变为主任务

1. 转到要将子任务作为主任务的项目。
1. 单击 **任务** 部分。
1. 选择要作为主任务的子任务。
1. 单击 **减少缩进** 图标 ![](assets/outdent-icon-nwe-31x29.png) 使子任务成为主任务。

   或

   在标准英语QWERTY键盘上，按Option + &lt; (Mac)或Alt + &lt; (Windows)。 其他语言可能使用命令Option + 。 (Mac)或Alt + 。 (Windows)升级。

   >[!NOTE]
   >
   >仅当任务列表按任务编号排序并且任务列表未应用分组时，您才可以减少任务编号。
