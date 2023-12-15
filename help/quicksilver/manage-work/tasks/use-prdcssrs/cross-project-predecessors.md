---
product-area: projects
navigation-topic: use-predecessors
title: 创建跨项目前置任务
description: 跨项目前置任务是指另一个项目中的另一个任务（称为后续任务）所依赖的任务。 前置任务是优先于从属（后置任务）任务的任务。 例如，您可以创建一个依赖项，要求在启动依赖项任务之前，将前置任务标记为“完成”。
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# 创建跨项目前置任务

<!--Audited: 12/2023-->

跨项目前置任务是指另一个项目中的另一个任务（称为后续任务）所依赖的任务。 前置任务是优先于从属（后置任务）任务的任务。 例如，您可以创建一个依赖项，要求在启动依赖项任务之前，将前置任务标记为“完成”。

Adobe Workfront允许任务依赖于其他项目中的任务，就像它允许单个项目中的前置任务一样。

>[!INFO]
>
>例如，一家挖掘公司只有一个挖掘机，而两个项目的任务需要使用挖掘机。 项目经理可以使第一个项目中的任务成为第二个项目中的任务的前置任务。 这表明，第二个项目可以在第一个项目使用完后开始使用反铲处理。

通过跨项目前置任务链接项目时，主项目（具有前置任务的项目）的日期将影响辅助项目（具有后续任务的项目）。

>[!TIP]
>
>您必须重新计算项目的时间表，才能看到辅助项目的更新日期。 有关重新计算时间线的详细信息，请参阅 [配置项目的时间线重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

有关前置任务关系的详细信息，请参阅 [前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
  <td> <p>新增：标准 </p>
 <p>或</p> 
<p>当前：计划 </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建跨项目前置任务

1. 转到将成为您的后续任务（从属任务）的任务。
1. 单击 **前置任务** 在左侧面板中。
1. 单击 **添加前置任务。**
1. 在 **父项目** 字段中，开始键入项目名称，该项目包含要作为当前任务的前置任务的任务。
1. 当名称出现在下拉列表中时，单击该名称。
1. 在 **任务** 字段中，开始键入要作为当前任务前置任务的名称。
1. 指定以下信息来定义前置任务和从属任务之间的关系：

   * **依赖关系类型：** 选择您希望前置任务与相关任务之间的关系。 默认关系为“完成 — 开始”，这意味着前置任务必须在相关任务开始之前完成。 有关各种依赖关系类型的详细信息，请参见 [任务相关性类型概览](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **滞后时间：** 指定在强制前置任务完成后，在相关任务可以开始之前必须经过的时间量。 有关各种滞后类型的更多信息，请参阅 [滞后类型概述](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **强制：** 如果选择该选项，用户无法提前开始任务，从而避免两个任务之间的依赖关系。 例如，如果强制任务A与任务B之间的关系，则在任务A完成之前无法启动任务B。 有关强制实施前置任务的更多信息，请参阅 [强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     未选择此选项时，依赖项将被视为对用户提出的建议。 例如，用户能够在任务A完成之前启动任务B。

1. 单击&#x200B;**保存**。

   具有跨项目前置任务的任务会在任务列表的前置任务列中显示前置任务所属项目的参考编号和任务编号（以冒号分隔）。

   ![跨项目前置任务](assets/cross-project-predecessor-in-list-view.png)

   将前置任务标记为完成时，前置任务图标会变为绿色。 这表示依赖任务已准备好工作。

   将鼠标悬停在此值上可获取有关前置任务、项目和日期的更多信息。 单击详细信息框中的跨项目前置任务以打开任务。

   单击悬停窗口顶部附近可查看有关前置任务项目的更多信息。

   单击 **查看项目** 以打开前置任务的项目。

   ![跨项目前置任务详细信息](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   此 **查看项目** 选项仅在查看跨项目前置任务时显示。

