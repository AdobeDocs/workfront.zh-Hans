---
product-area: projects
navigation-topic: manage-tasks
title: 将里程碑与任务关联
description: 您可以将里程碑与任务关联，以指示您在项目生命周期中达到重要步骤的时间。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 将里程碑与任务关联

您可以将里程碑与任务关联，以指示您在项目生命周期中达到重要步骤的时间。

## 访问要求

<!--drafted - replace table for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>编辑任务访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在将里程碑与任务关联之前，必须存在以下内容：

* Workfront管理员必须创建里程碑路径，如 [创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* 要将里程碑路径与项目关联，项目必须处于“计划”或“当前”状态。

>[!TIP]
>
>要使用“里程碑”视图获取项目中里程碑进度的最佳概述，您应创建父任务，并将它们与项目的每个主要阶段相关联。 然后，将这些父任务与里程碑路径的每个里程碑相关联。

## 将里程碑与任务关联

1. 转到项目，然后单击 **更多** 图标 ![](assets/more-icon.png)，则 **编辑**.
1. 使用 **设置** 部分，设置要在项目中使用的里程碑路径。
1. 单击&#x200B;**保存**。

   在里程碑路径与项目关联后，可以为任务分配里程碑。

1. 转到任务，然后单击 **更多** 图标 ![](assets/more-icon.png)，则 **编辑**.

   任务和里程碑之间有1:1的关系。 您无法将同一里程碑附加到多个任务。 每个任务可以链接到单个里程碑，也可以将每个里程碑映射到一个任务。

1. 单击 **设置**，然后在 **里程碑** 字段。
1. 单击 **保存**.
1. （可选）在任务列表中，将 **状态图标** 列来标识哪些任务具有里程碑。

   ![](assets/amwt3.png)

1. （可选）在项目列表中，选择 **里程碑** 查看以确定里程碑任务的进度。

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
