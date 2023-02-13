---
product-area: projects
navigation-topic: manage-projects
title: 选择项目更新类型
description: 通过为项目选择更新类型，您可以控制您对项目时间轴所做的更改在父任务或项目中保存的频率。
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 选择项目更新类型

通过为项目选择更新类型，您可以控制您对项目时间轴所做的更改在父任务或项目中保存的频率。

更新项目时间轴后，将根据对项目所做的更改、项目任务或对时间轴所依赖的其他项目所做的更改重新计算项目时间轴。

例如，对项目上的任务所做的以下更改会触发对项目时间轴的更新：

* 更新任务日期
* 更改任务的前置关系
* 更改父子关系，添加或删除分配以及更改任务约束或持续时间类型。

## 访问要求

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 更新项目的更新类型

当任务更新时，其父对象（父任务或项目）会在更新类型指示的时间更新。  要为项目指定更新类型，请执行以下操作：

1. 转到要指定其更新类型的项目。
1. 单击“更多”菜单 ![](assets/more-icon.png) 在项目名称旁边，单击 **编辑** .

1. 单击  **项目** **设置**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. 在 **更新类型** 字段中，选择是希望Workfront每天自动计算项目的时间轴，还是希望项目经理手动计算项目时间轴。

   从下面列表的选项中进行选择。 

   >[!IMPORTANT]
   >
   >如果项目的时间轴超过15年，Workfront不会自动计算时间轴或在发生更改时计算时间轴。 超过15年的项目更新类型始终为手动。

   * **自动和更改：** 这是默认设置。 每当项目或时间轴所依赖的其他项目中发生更改时，项目时间轴都会更新。 项目时间轴也会在每晚更新。 \
      这是推荐的设置，因为它可确保项目时间轴始终为最新。

      当您更新任务或项目并触发时间轴重新计算时，所有可用日期都会立即显示，从而允许您继续工作。 对于任务超过100个的项目，需要较长计算的日期将变暗。

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      这表示重新计算尚未完成，并且日期可能会发生更改。

   * **仅更改：** 每当项目或时间轴所依赖的其他项目中发生更改时，项目时间轴都会更新；不会进行计划更新。\
      如果您担心系统性能，并且在项目或时间轴所依赖的其他项目中很少发生更改，则可能需要选择此选项。

   * **仅自动：** 项目时间表每天晚上都会更新；所做的更改不会立即更新。\
      如果您担心系统性能，并且在项目或时间轴所依赖的其他项目中每天发生许多更改，则可能需要选择此选项。

      >[!NOTE]
      >
      >如果项目处于“计划”状态，则它不会每天晚上自动重新计算。 它只会在更改时重新计算。

   * **仅手动：** 仅当您选择 **重新计算时间轴**，如文章“手动重新计算”一节中所述 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      如果您同时对项目进行多次更改，并且希望在所有更改（而不是在每次更改后）之后重新计算时间轴，则可能需要选择此选项。

1. 单击&#x200B;**保存**。
