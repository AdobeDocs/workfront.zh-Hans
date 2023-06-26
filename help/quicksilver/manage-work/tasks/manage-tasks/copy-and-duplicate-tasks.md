---
product-area: projects
navigation-topic: manage-tasks
title: 复制和复制任务
description: 您可以将任务从项目复制到另一个项目，也可以复制同一项目中的任务。
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 1%

---

# 复制和复制任务

您可以将任务从项目复制到另一个项目，也可以复制同一项目中的任务。

您可以一次复制或复制一个或多个任务或父任务。

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
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限 </p> <p>为项目分配或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 复制任务的注意事项

复制任务时，请考虑以下事项：

* 问题不会与任务一起复制。
* 里程碑会传输到复制的任务并从原始任务中删除。
* 将任务从一个项目复制到另一个项目时，可能会重新计算任务日期。 重新计算将考虑新项目使用的时间表和项目的时间表信息。

您可以在Adobe Workfront Web应用程序的以下区域中复制任务：

* 在任务级别，从 **“更多”图标** ![](assets/qs-more-menu-19x7.png) 任务名称的右侧。

  欲了解相关信息，请参见 [在任务级别复制任务](#copy-a-task-at-the-task-level) 章节。

* 在任务列表中，执行下列操作之一：

   * 右键单击任务的名称。
   * 选择任务（或多个任务）并展开 **更多** 图标 ![](assets/more-icon-task-list.png) 在任务列表的顶部。
   * 选择任务并展开 **更多** 图标 ![](assets/more-icon-task-list.png) 在任务名称旁边。

     选择多个任务时，此选项不可用。

  欲了解相关信息，请参见 [复制列表中的任务](#copy-tasks-in-a-list) 章节。

## 复制列表中的任务 {#copy-tasks-in-a-list}

1. 转到包含要复制的一个或多个任务的项目。

   或

   转到任务报告。

1. 单击 **任务** （在左侧面板中）。
1. 单击 **规划模式菜单** ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，则 **自动保存**.

   >[!IMPORTANT]
   >
   >仅当自动保存更改时，才能复制列表中的任务。 有关编辑任务时保存选项的信息，请参阅 [编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 选择要复制的一个或多个任务，然后执行以下操作之一：

   * 单击 **“更多”菜单** 单击任务列表顶部的 **复制到**.
   * 右键单击选定的任务，然后单击 **复制到**.
   * 选择一项任务时，单击 **更多** 菜单 ![](assets/more-icon-task-list.png) 单击列表中的任务名称旁边的，然后单击 **复制到**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. 继续复制任务，如一节中所述 [在任务级别复制任务](#copy-a-task-at-the-task-level) 从步骤4开始。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## 在任务级别复制任务 {#copy-a-task-at-the-task-level}

除了复制任务列表中的任务外，您还可以在打开任务后复制任务。 

1. 通过搜索在Workfront系统中查找任务。
1. 单击任务名称以将其打开。 
1. 单击 **更多** 下拉菜单 ![](assets/qs-more-menu.png) 单击任务名称旁边的，然后单击 **复制** **到**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   此时将显示“复制任务”框。

1. （可选）更新 **任务名称**.

   >[!TIP]
   >
   >选择复制列表中的多个任务时，此字段将灰显且不可编辑。 您可以将鼠标悬停在“任务名称”字段上，此时将显示所有选定任务的列表。
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. 键入的名称 **目标项目** 要将任务复制到 **选择目标项目** 字段。 

   >[!TIP]
   >
   >* 项目名称区分大小写。
   >* 您还可以开始键入参考号或输入项目的ID。 这可以帮助您区分具有相同名称的项目。
   >* 列表中只显示100个项目。

   默认显示当前项目名称。 如果要复制同一项目中的任务，请保留此字段不变。

1. （视情况而定）单击 **请求访问** 以请求对项目的访问权限（如果您无权访问所选项目）。
1. （视情况而定）如果您有权将任务添加到目标项目上的任务之一，请继续将任务复制到选定的目标项目，而不请求访问权限。

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >当Workfront管理员阻止将任务添加到这些项目时，如果所选项目处于未决批准、已完成或终止状态，则会显示类似消息。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. 单击 **选项** 然后，在左侧面板中取消选择您不希望与任务一起复制的任务属性。 默认情况下，将选择所有选项。

   >[!TIP]
   >
   选择，然后取消选择 **全选** 取消选择所有选项。

   取消选择以下选项，不将它们转移到复制的任务。 下表介绍了取消选择这些选项时会发生什么情况：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">约束</td> 
      <td> <p>根据“项目计划模式”设置，任务限制设置为尽可能早或尽可能迟。</p> <p> 选中后，任务的当前限制将转移到复制的任务。 </p> <p>注：在将具有日期特定限制的任务移动或复制到另一个项目时，如果任务的限制日期在新项目的日期之外，则任务限制会更改成“尽快”或“尽可能延迟”，或者调整项目的计划起始日期或计划完成日期。 某些日期特定约束的示例包括：必须开始于、必须完成于、开始时间不早于、开始时间不晚于，等等。 有关任务限制以及任务限制或项目日期如何受到影响的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务限制概述</a> 并寻找特定的限制。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">分配</td> 
      <td> <p>将从任务中删除所有分配。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">批准流程</td> 
      <td>所有批准流程都将从任务中删除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>任务状态为“新建”。 否则，复制的任务将保留现有任务的状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">财务信息</td> 
      <td>删除任务的财务信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>这意味着依赖关系不会传递到复制的任务。 </p> <p>选中后，将保留复制任务组中的前置任务，而删除其他前置任务。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>附加到任务的文档不会转移到复制的任务。 这包括版本、验证和链接文档。</p> <p>这不包括文档审批。 在复制任务时，不能复制文档审批。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任务提醒不会转移到复制的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>登录任务的费用不会转移到复制的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td>Workfront会删除任务的“共享”列表中显示的所有实体的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义数据</td> 
      <td> <p>清除自定义字段的值，并将自定义表单传输到复制的任务。 </p> <p>选中后，自定义字段的表单和值都会转移到复制的任务。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  （可选）单击 **选择父级** 在左侧面板中，选择要成为所复制任务的父级的目标项目中的任务。

   >[!TIP]
   >
   当选择在列表中复制多个任务时，所有选定的任务都会成为选定父级的子级。

   通过执行以下操作之一选择父级：

   * 在任务列表中，选择项目计划中的父项之一。
   * 单击搜索图标 ![“搜索”图标](assets/search-icon.png) 并按名称搜索父任务。

   该任务应显示在列表中。

   ![使用搜索功能移动任务时选择父任务 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父项后，选择父项的单选按钮。 

   如果不选择父任务，则任务将作为主任务而不是子任务复制，并且将它们放在目标项目的任务列表的末尾。 

1. 单击 **复制任务**

   或

   单击 **复制任务** 在列表中选择多个任务时。
复制的任务现在位于指定项目上，并且是选定父任务的子任务，或者是项目上的最后一个任务。

## 复制任务

如果您需要同一项目中的相同任务，则可以快速复制任务列表中的任务。

* [复制任务的注意事项](#considerations-for-duplicating-tasks)
* [复制任务](#duplicate-tasks)

### 复制任务的注意事项 {#considerations-for-duplicating-tasks}

* 仅当任务列表按任务编号排序时，才能复制任务列表中的任务。

* 新任务将与原始任务同名。
* 您无法选择将哪些信息复制到新任务。 默认情况下，几乎所有原始任务中的信息都将转移到复制任务，包括父关系。
* 以下项目未转移到新任务：

   * 记录的小时数
   * 注释
   * 问题
   * 只有属于同一组复制任务的前置任务才会与其后续任务一起复制。

     **示例：** 例如，如果同时复制任务2及其前置任务任务1，则会复制任务2和任务1。 任务1的副本将是任务2副本的前身。 但是，如果您只复制任务2而没有复制其前置任务，则其副本将没有前置任务。

* 复制父任务时，即使未选择子任务，也会复制所有子任务。
* 您可以同时复制多个任务。

  但是，不能同时复制多个非连续的任务。

* 里程碑将移动到新任务并从原始任务中删除。

### 复制任务

1. 转到包含要复制的一个或多个任务的项目。
1. 单击 **任务** （在左侧面板中）。
1. 执行下列操作之一：

   * （视情况而定）单击 **规划模式菜单** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **自动保存**，选择要复制的任务，然后单击 **“更多”菜单** ![](assets/qs-more-menu-29x11.png) > **复制**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * （视情况而定）单击 **规划模式菜单** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **手动保存** > **标准** 或 **时间线规划**，然后执行以下操作：

      1. 选择要复制的一个或多个任务，然后单击 **复制**.
      1. （可选）单击 **撤消** 以撤消更改而不复制任务。
      1. （可选和条件）单击 **重做** 如果您之前已单击 **撤消**，以保留更改并复制任务。

      1. 单击 **保存** 以保存更改。

   1. 编辑列表中的任务
