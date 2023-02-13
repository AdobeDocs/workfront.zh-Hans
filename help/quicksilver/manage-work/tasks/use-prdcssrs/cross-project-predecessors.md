---
product-area: projects
navigation-topic: use-predecessors
title: 创建跨项目前置项
description: 跨项目前置任务是另一个项目中的另一个任务（称为后续任务）所依赖的任务。 前置任务是优先于从属（后继）任务的任务。 例如，您可以创建一个依赖项，该依赖项要求在从属任务开始之前将前置任务标记为完成。
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 创建跨项目前置项

跨项目前置任务是另一个项目中的另一个任务（称为后续任务）所依赖的任务。 前置任务是优先于从属（后继）任务的任务。 例如，您可以创建一个依赖项，该依赖项要求在从属任务开始之前将前置任务标记为完成。

与单个项目中的前任一样，Adobe Workfront允许任务依赖于其他项目中的任务。

**示例**

如果一个挖掘公司只有一个挖掘机，并且两个并发项目有需要使用挖掘机的任务，项目经理可以使第一个项目中的任务依赖于第二个项目中的任务，以说明在上一个项目放弃挖掘时挖掘可以开始。
通过跨项目前置任务链接项目时，主项目（具有前置任务的项目）的日期将影响辅助项目（具有后置任务的项目）。

>[!TIP]
>
>您必须重新计算项目的时间轴，才能查看辅助项目的更新日期。 有关重新计算时间轴的更多信息，请参阅 [为项目配置时间轴重新计算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

有关前身关系的更多信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建跨项目前置项

1. 转到将成为您的后继者的任务。
1. 单击 **前置任务** 中。
1. 单击 **添加前置项。**
1. 在 **父项目** 字段中，开始键入包含要依赖于当前任务的任务的项目名称。
1. 当名称显示在下拉列表中时，单击该名称。
1. 在 **任务** 字段中，开始键入要依赖于当前任务的任务名称。
1. 指定以下信息以定义前置任务和从属任务之间的关系：

   * **依赖关系类型：** 选择您希望任务与从属任务的关系。 默认关系为“完成 — 开始”，这意味着前置任务必须在从属任务开始之前完成。 有关各种依赖关系类型的更多信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **滞后：** 指定在强制前置任务完成后，在从属任务开始之前必须经过的时间。 有关各种滞后类型的更多信息，请参阅 [滞后类型概述](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **强制：** 选择此选项后，用户无法提前开始任务来规避两个任务之间的依赖关系。 例如，如果强制执行任务A和任务B之间的关系，则在任务A完成之前，无法启动任务B。 有关强制使用前置命令的详细信息，请参阅 [强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      未选择此选项时，依赖关系会被视为用户的建议。 例如，用户能够在任务A完成之前启动任务B。

1. 单击&#x200B;**保存**。

   具有跨项目前置项的任务将显示前置项所属项目的参考编号和任务编号，在任务列表的“前置项”列中用冒号分隔。

   ![跨项目前身](assets/cross-project-predecessor-in-list-view.png)

   当前任务标记为完成时，前置任务图标将变为绿色。 这表示相关任务已准备就绪。

   将鼠标悬停在此值上，可获取有关上一代产品、项目和日期的更多信息。 单击“详细信息”(Details)框中的跨项目前置项以打开任务。 单击 **请参阅项目** 打开跨项目。

   ![跨项目前置任务详细信息](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   的 **请参阅项目** 选项仅在查看跨项目前置项时显示。

