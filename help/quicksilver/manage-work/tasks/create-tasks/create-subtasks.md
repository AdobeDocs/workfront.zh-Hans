---
product-area: projects
navigation-topic: create-tasks
title: 创建子任务
description: 在Adobe Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设置为子任务，可以在任务列表中创建子任务。 您还可以将子任务设置为主任务。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 创建子任务

<!-- Audited: 01/2025 -->

在Adobe Workfront中，任务可以具有父子关系。 子任务称为子任务。 通过将主任务设置为子任务，可以在任务列表中创建子任务。 您还可以将子任务设置为主任务。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>Contribute对项目和父任务的权限，能够添加任务或更高版本</p> <p>在创建任务后，您会自动收到该任务的“管理”权限。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建子任务

您可以从任务列表或任务子任务部分创建子任务。

### 从任务列表创建子任务 {#create-subtasks-from-the-task-list}

1. 转到要创建子任务的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;部分。
1. （视情况而定）如果要生成子任务的任务尚未位于要生成父任务的任务的正下方，请将其拖放到任务列表中的适当位置。
1. 选择要创建子任务的任务，然后执行以下操作之一：

   * 单击&#x200B;**缩进**&#x200B;图标![](assets/indent-icon-nwe-33x29.png)，使所选任务成为其正上方的任务的子任务。
   * 使用标准英语QWERTY键盘时，按键盘上的Option + > (Mac)或Alt + > (Windows)。 其他语言可能使用命令Option + 、 (Mac)或Alt + 、 (Windows)进行缩进。

     >[!TIP]
     >
     >在内联编辑中编辑任务时，键盘快捷键不起作用。 在这种情况下，请使用缩进图标![](assets/indent-icon-nwe-33x29.png)创建子任务。

   * 将任务拖放到要指定为父级任务的任务上。

     >[!NOTE]
     >
     >仅当任务列表按任务编号排序并且任务列表未应用分组时，您才可以缩进任务。

### 从任务的“子任务”部分创建子任务 {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>您的Workfront或组管理员可以使用布局模板删除环境中的子任务部分。

1. 转到要创建子任务的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;部分。
1. 单击要在其中创建子任务的任务的名称。
1. 单击左侧面板中的&#x200B;**子任务**&#x200B;部分（如果存在）。
1. 单击&#x200B;**新建任务。**

   按照以下文章中的步骤继续创建子任务：[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

1. 单击&#x200B;**创建任务。**

## 将子任务变为主任务

1. 转到要将子任务作为主任务的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;部分。
1. 选择要作为主任务的子任务。
1. 单击&#x200B;**减少缩进**&#x200B;图标![](assets/outdent-icon-nwe-31x29.png)使子任务成为主任务。

   或

   在标准英语QWERTY键盘上，按Option + &lt; (Mac)或Alt + &lt; (Windows)。 其他语言可能使用命令Option + 。 (Mac)或Alt + 。 (Windows)升级。

   >[!NOTE]
   >
   >仅当任务列表按任务编号排序并且任务列表未应用分组时，您才可以减少任务编号。
