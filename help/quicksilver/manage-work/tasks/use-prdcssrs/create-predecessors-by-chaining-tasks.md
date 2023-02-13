---
product-area: projects
navigation-topic: use-predecessors
title: 通过链接任务创建前置关系
description: 您可以在Adobe Workfront中以多种方式创建前身关系。 一种方法是通过链接任务。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# 通过链接任务创建前置关系

您可以在Adobe Workfront中以多种方式创建前身关系。 一种方法是通过链接任务。

有关前置任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

通过链接任务，您可以允许系统在选定任务上自动创建前置关系，而不是自行在每个任务上手动创建关系。 任务之间仍可以使用不同的前置关系类型。

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 链式任务以创建前置任务关系

1. 转到包含要链接的任务的项目。
1. 单击 **任务** 中。
1. （视情况而定）选择 **自动保存** 在任务列表的右上角，选择要链接的任务。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >手动保存对任务的更改或使用“时间轴规划”模式保存任务时，无法在任务列表中链接任务。

1. 右键单击选定的任务，然后单击 **链**.
1. 从以下依赖关系类型中进行选择：

   * **结束-开始**
   * **结束-结束**
   * **开始-开始**
   * **开始-完成**

   有关前置依赖关系类型的更多信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. （可选）单击 **解链** 如果某些任务以前已被链接。

   >[!CAUTION]
   >
   >批量编辑任务时，只能使用取消链选项来删除连续的前置任务。

   您选定的任务现在由前任关系链接。
