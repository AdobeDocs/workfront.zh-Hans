---
product-area: projects
navigation-topic: use-predecessors
title: 通过链接任务创建前置任务关系
description: 在Adobe Workfront中，您可以通过多种方式创建前置任务关系。 一种方法是链接任务。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 通过链接任务创建前置任务关系

在Adobe Workfront中，您可以通过多种方式创建前置任务关系。 一种方法是链接任务。

有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

通过链接任务，您可以允许系统在选定任务上自动创建前置任务关系，而不是在每项任务上自己手动创建关系。 任务之间仍可以使用不同的前置任务关系类型。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 链接任务以创建前置任务关系

1. 转到包含要链接的任务的项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. （视情况而定）选择任务列表右上角的&#x200B;**自动保存**，然后选择要链接的任务。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >当您手动保存对任务的更改或使用“时间线计划”模式保存任务时，无法链接任务列表中的任务。

1. 右键单击选定的任务，然后单击&#x200B;**链**。
1. 从以下依赖关系类型中选择：

   * **完成 — 开始**
   * **完成 — 完成**
   * **开始 — 开始**
   * **开始 — 完成**

   有关前置任务依赖关系类型的详细信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. （可选）如果某些任务之前已链接，请单击&#x200B;**取消链接**。

   >[!CAUTION]
   >
   >批量编辑任务时，使用取消链选项仅会删除连续的前置任务。

   您选择的任务现在由前置任务关系链接。
