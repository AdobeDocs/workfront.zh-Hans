---
product-area: projects
navigation-topic: manage-tasks
title: 编辑列表中的任务
description: 您可以通过编辑列表中显示的字段来编辑任务列表中的任务信息。 有关编辑任务的其他方法的信息，请参阅编辑任务。
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 2%

---

# 编辑列表中的任务 {#edit-tasks-in-a-list}

您可以通过编辑列表中显示的字段来编辑任务列表中的任务信息。 有关编辑任务的其他方法的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或任务及项目的更高权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 有关编辑列表中的任务的注意事项 {#considerations-about-editing-tasks-in-a-list}

编辑列表中的任务是一种同时更改多个任务的快速方法，可清楚地查看更改可能会如何影响项目时间表。

编辑列表中的任务时，请考虑以下事项：

* 与在“编辑”框中编辑任务时需要对该任务的“管理”权限不同，您只能编辑列表中具有Contribute权限的任务。 这允许您编辑任务的以下有限信息：

   * 描述
   * 状态
   * 完成百分比
   * 自定义表单信息

     >[!NOTE]
     >
     >只有在您具有更新任务自定义字段的权限时，才能在列表中编辑该字段。

   * 记录小时数
   * 修改分配
   * 查看财务信息
   * 添加费用、任务或问题

* 您可以编辑以下列表中的任务：

   * 项目的任务部分
   * 项目的子任务部分
   * 任务报告

     >[!NOTE]
     >
     >默认情况下，Workfront会自动将您对任务所做的更改保存在“子任务”部分或任务报告中。

* 您可以控制Workfront何时将对任务所做的更改保存到列表中。 您的更改可以自动保存，也可以手动保存。

  有关在Workfront保存您对列表中的任务所做的更改时进行配置的信息，请参阅本文中的“编辑列表中的任务时[选择保存选项”](#select-a-save-option-when-editing-tasks-in-a-list)部分。

* 其他用户必须先刷新其页面，然后才能查看您对任务所做的更新。

## 在列表中编辑任务时选择保存选项 {#select-a-save-option-when-editing-tasks-in-a-list}

您可以决定对列表中的任务所做的更改在发生时自动保存的位置，或者是否要手动保存每个更改。

>[!IMPORTANT]
>
>根据您是自动还是手动保存任务，在编辑列表中的任务时，可能会覆盖其他人的信息。 有关Workfront如何保存您与其他用户同时进行的任务更改的信息，请参阅[在任务列表中保存并发更改概述](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md)。

当您将更改保存在已选择自动或自动以及发生更改作为更新类型的项目的列表中，Workfront会更新项目时间线以及所有项目内和跨项目依赖关系。 如果项目较大或存在大量依赖关系，则时间线计算可能需要较长时间。 某些编辑任务列表的方法可能比其他方法更快，具体取决于您选择用于保存更改的方法。

您可以控制Workfront何时将对任务所做的更改保存到列表中。 存在以下情况： 

* 您可以让Workfront在每次更新后自动保存更改。

  有关信息，请参阅本文中的[编辑列表中的任务并自动保存更改](#edit-tasks-in-a-list-and-automatically-save-changes)部分。

* 使用“保存”按钮可控制一次应用多个更改的时间。

  有关信息，请参阅本文中的[编辑列表中的任务并手动保存更改](#edit-tasks-in-a-list-and-manually-save-changes)部分。

### 编辑列表中的任务并自动保存更改 {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>如果您的项目具有超过2000个任务或具有大量依赖关系，则保存更改和所有项目依赖关系可能会较慢。

在自动保存任务列表更改时，请考虑以下事项：

* 您可以将自定义视图应用于任务列表，并编辑您有权更新的任何与任务相关的字段。
* 无法撤消自动保存的更改。 这是默认设置。
* 当项目更新类型为自动或自动且发生更改时，Workfront会在每次更改后自动重新计算项目的时间表以及所有项目内和跨项目依赖关系。 有关项目更新类型的信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

要编辑列表中的任务并自动保存更改，请执行以下操作：

1. 转到项目，然后单击&#x200B;**任务**&#x200B;部分。
1. 单击列表顶部的&#x200B;**计划模式菜单** ![](assets/qs-list-mode-or-save-mode-icon-small.png)，并确保已选择&#x200B;**自动保存**&#x200B;选项。

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 编辑您有权手动更新的任何字段。

   ![](assets/inline-editing-a-task-350x26.png)

1. （可选）按&#x200B;**Escape**&#x200B;取消更改。
1. 按Enter键以保存对任务和项目时间线所做的更改。
1. （可选）右键单击要修改的任务。

   或

   单击任务名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon-task-list.png)。

1. （可选）从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新选项卡中打开</strong></td> 
      <td>在新的浏览器选项卡中打开任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>编辑</strong></td> 
      <td><p>打开<strong>编辑任务</strong>框，您可以在其中编辑任务。</p><p>有关编辑任务的信息，请参阅<a href="#edit-tasks-in-a-list" class="MCXref xref">编辑列表中的任务</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td><p>删除任务。</p><p>有关删除任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td><p>将任务缩进一个级别。 </p><p>此选项仅在独立任务中显示。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td><p>将任务凸排一级。 </p><p>此选项仅在子任务中显示。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">在上面插入任务</td> 
      <td>在选定任务上方插入任务。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下面插入任务</td> 
      <td>在选定任务下插入任务</td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制</td> 
      <td><p>在同一项目中创建任务的重复版本。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制到</td> 
      <td><p>将任务复制到另一个项目。</p><p>有关复制和复制任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">移至</td> 
      <td><p>将任务移动到另一个项目。</p><p>有关移动任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">移动任务</a>。</p></td> 
     </tr> 
    </tbody> 
   </table>

   更改会自动保存，您无法撤消它们。

### 编辑列表中的任务并手动保存更改 {#edit-tasks-in-a-list-and-manually-save-changes}

您可以手动保存对列表中的任务所做的更改。 以这种方式保存更改时，您可以灵活地在保存之前撤消更改。

>[!TIP]
>
>* 在“子任务”部分或任务报告中编辑列表任务时，无法撤消对这些任务所做的更改。
>* 您可以撤消的更改数没有限制。 您可以逐个撤消所有这些任务，直到达到任务的原始状态。
>

在任务列表中手动保存更改时，请考虑以下事项：

* 要手动保存任务列表更改，您需要具有管理任务和项目的权限。
* 您无法编辑项目。 已禁用编辑项目的选项。
* 您不能更新项目标头中的信息。 在任务列表中手动保存更改时，只能执行以下操作：

   * 订阅项目。
   * 将项目添加到收藏夹列表。
   * 单击列表中的任务名称以打开任务。

* 批量编辑任务。 选择多个任务时，“编辑”图标处于禁用状态。
* 只有在保存更改后，Workfront才会触发有关您对任务所做更改的通知。

有两种方法可手动保存对列表中任务的更改。 下面介绍了这两种方法。

* [选择“手动保存标准”选项时，在任务列表中手动保存更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [选择“手动保存时间线计划”选项时，在任务列表中手动保存更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 选择“手动保存标准”选项时，手动保存任务列表中的更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>如果您的项目有超过2000个任务，或者如果它有许多依赖项，则可能需要一段时间才能直观地识别您对任务所做的更改以及这些更改如何影响所有项目依赖项。 在这种情况下，如果您的项目具有超过2000个任务或具有大量依赖关系，则保存更改可能需要更长的时间。

选择“手动保存标准”选项后更新列表中的任务时，请考虑以下事项：

* 您可以将自定义视图应用于任务列表，并编辑您有权在该视图中管理的任何任务相关字段。
* 当项目更新类型为自动或自动且发生更改时，在单击保存后，Workfront会计算项目的时间线以及所有项目内和跨项目依赖关系。 有关项目更新类型的信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

要在选择“手动保存标准”选项时编辑列表中的任务，请执行以下操作：

1. 转到项目，然后单击&#x200B;**任务**&#x200B;部分。
1. 单击列表顶部的&#x200B;**计划模式**&#x200B;菜单![](assets/qs-list-mode-or-save-mode-icon-small.png)并选择&#x200B;**手动保存**，然后单击&#x200B;**标准** > **应用**。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   此时将显示一个工具栏设置，其中包含用于撤消、重做和保存更改的选项。

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 单击您有权手动更新的任何字段。 该字段将变为可编辑，您可以进行更改。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按Enter暂时保存所做的更改。
1. （可选）单击&#x200B;**撤消图标** ![](assets/undo-icon-on-task-list.png)以撤消更改并将字段恢复到其原始状态。
1. （可选且有条件）单击&#x200B;**重做图标** ![](assets/redo-icon-on-task-list.png)以恢复您回复的更改。

1. （可选）右键单击要修改的任务。

   或

   单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon-task-list.png)。

1. （可选）从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新标签页中打开</strong> </td> 
      <td>在新的浏览器选项卡中打开任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td>有关删除任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td> <p>将任务缩进一个级别。 </p> <p>此选项仅在独立任务中显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td> <p>将任务凸排一级。 </p> <p>此选项仅在子任务中显示。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在上面插入任务</td> 
      <td>在选定任务上方插入任务。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下面插入任务</td> 
      <td>在选定任务下插入任务</td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制</td> 
      <td> <p>在同一项目中创建任务的重复版本。 </p> <p>有关复制和复制任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 当您更改任务的时间表时，Workfront会更新所有项目内依赖项和跨项目依赖项。
1. 如果要永久保留任务更改并保存项目的时间表，请单击&#x200B;**保存**。

#### 选择“手动保存时间线计划”选项时，在任务列表中手动保存更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

保存更改和所有项目依赖项的速度更快。 这不适用于任务数超过2000的项目。

>[!IMPORTANT]
>
>我们建议您在编辑数百个以上、具有大量依赖关系的大量任务列表时使用此选项。 使用此选项，您可以比使用手动保存选项更快地直观地识别更改。

在任务列表中使用“手动保存时间线计划”选项时，请考虑以下事项：

* 您不能将“手动保存时间表计划”选项应用于具有超过2000个任务的项目。
* 您不能将自定义视图、筛选器或分组应用于任务列表。 “视图”、“筛选器”和“分组”下拉菜单以及“敏捷视图”图标被禁用。 默认应用的视图包含有限数量的字段。
* 当项目的“更新类型”为“自动”或“自动”且“更改时”时，在每次更改后将自动计算项目的时间表和所有项目内的依赖项。
* 当项目更新类型为自动或自动且发生更改时，在单击“保存”后计算跨项目依赖关系。 有关项目更新类型的信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

要在使用“手动保存时间线计划”选项时编辑列表中的任务，请执行以下操作：

1. 转到项目，然后单击&#x200B;**任务**&#x200B;部分。
1. 单击列表顶部的&#x200B;**计划模式**&#x200B;菜单![](assets/qs-list-mode-or-save-mode-icon-small.png)并选择&#x200B;**手动保存**，然后单击&#x200B;**时间线计划**>**应用**。

   对于超过2000个任务的项目，此选项呈灰显状态。

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >当您离开此页面时，Workfront会重新启用自动保存选项。

   请注意列表中的以下更改：

   * “视图”、“分组”和“筛选器”下拉菜单被删除，视图由以下字段替换：

      * 任务编号
      * 任务名称
      * 限制类型
      * 持续时间
      * 计划开始日期
      * 规划完成日期
      * 前置任务
      * 分配
      * 状态
      * 完成百分比

   * 移除Agile视图图标。
   * 此时将显示一个工具栏设置，其中包含用于撤消、重做和保存更改的选项。

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 编辑您有权手动更新的任何字段。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按Enter暂时保存所做的更改。
1. （可选）单击&#x200B;**撤消图标** ![](assets/undo-icon-on-task-list.png)以撤消更改并将字段恢复到其原始状态。
1. （可选且有条件）单击&#x200B;**重做图标** ![](assets/redo-icon-on-task-list.png)以恢复您冲销的更改。

1. （可选）右键单击要修改的任务

   或

   单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon-task-list.png)。

1. 从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新标签页中打开</strong> </td> 
      <td>在新的浏览器选项卡中打开任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td>有关删除任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td> <p>将任务缩进一个级别。 </p> <p>此选项仅在独立任务中显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td> <p>将任务凸排一级。 </p> <p>此选项仅在子任务中显示。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在上面插入任务</td> 
      <td>在选定任务上方插入任务。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下面插入任务</td> 
      <td>在选定任务下插入任务</td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制</td> 
      <td> <p>在同一项目中创建任务的重复版本。 </p> <p>有关复制和复制任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 当您更改任务的时间表时，Workfront会更新所有项目内依赖项和跨项目依赖项。
1. 如果要永久保留任务更改并保存项目的时间表，请单击&#x200B;**保存**。

## 使用摘要编辑列表中的任务

1. 转到包含要编辑的任务的项目。
1. 单击左侧面板中的&#x200B;**任务**。

   此时将显示项目中的任务列表。

1. 单击任务名称后面的“更多”菜单![](assets/more-icon-task-list.png)，然后单击&#x200B;**打开摘要**。 选择要编辑的任务，然后单击列表右上角的&#x200B;**打开摘要图标** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png)。

   将打开&#x200B;**摘要**。

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. （可选）单击“摘要”右上角的&#x200B;**X图标**&#x200B;以关闭面板并编辑内联任务。

   按照在列表中编辑任务的步骤内联编辑任务。

   有关编辑列表中任务的信息，请参阅本文中的[有关编辑列表中任务的注意事项](#considerations-about-editing-tasks-in-a-list)。

1. （可选）在&#x200B;**更新**&#x200B;区域为任务键入更新。
1. 单击以下图标或区域之一，转到任务并在任务级别编辑信息：

   | 文档 | 单击&#x200B;**单击此处添加**&#x200B;将文档添加到任务。 |
   |---|---|
   | 详细信息 | 单击可更新有关任务的信息。 |
   | 自定义表单 | 单击以添加或删除自定义Forms或更新表单信息。 |
   | 小时 | 单击以记录小时数。 |
   | 审批 | 单击以添加任务批准。 |

   {style="table-layout:auto"}

1. 完成更新任务后，单击浏览器上的“返回”按钮返回到任务列表。

## 批量编辑任务

您可以同时编辑多个任务。 确保您对任务具有管理权限以便能够编辑它们。

1. 转到包含要批量编辑的任务的项目。
1. 单击左侧面板中的&#x200B;**任务**。
1. 确保已选择&#x200B;**自动保存**&#x200B;选项。

   >[!IMPORTANT]
   >
   >手动保存任务时无法批量编辑任务。

   有关将更改保存到列表中任务的方式的更多信息，请参阅本文中[有关编辑列表中任务的注意事项](#considerations-about-editing-tasks-in-a-list)部分。

1. 在任务列表中选择多个任务。
1. 单击&#x200B;**编辑图标** ![](assets/qs-edit-icon.png)。

   将打开&#x200B;**编辑任务**&#x200B;对话框。

1. 为所选的所有任务指定要更改的信息。

   编辑所有任务的信息与编辑一个任务的信息相同。 如果要编辑任务持续时间，所选任务必须具有相同的任务限制；否则，**持续时间**&#x200B;字段不填充。

   有关编辑任务的详细信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

   >[!NOTE]
   >
   >您在所有选定任务上更改的信息将覆盖单个任务上的现有信息，但&#x200B;**工作总揽**&#x200B;字段除外。 在批量编辑中添加新的被分配人会将该被分配人添加到所有选定的任务。 如果为所选任务分配了其他被分配人，则除了通过批量编辑添加的被分配人外，这些被分配人仍将保持分配状态。

1. 单击&#x200B;**自定义Forms**&#x200B;可编辑附加到所有选定任务的自定义表单。 列表中仅显示活动的自定义表单。

   如果所选任务没有任何常见的自定义表单，则此部分中未列出任何表单。

   您只能编辑表单上附加到所有选定任务且您有权编辑的字段。

1. （可选）在“自定义Forms”部分中，选择&#x200B;**重新计算自定义表达式**&#x200B;选项，以确保附加到所选任务的自定义表单上的所有计算自定义字段都是最新的。
1. 单击&#x200B;**保存更改**。

   您所做的所有更改现在在所有选定任务中均可见。

有关批量编辑自定义表单的信息，请参阅[管理附加到对象的自定义表单](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)中的“批量编辑对象时编辑多个自定义Forms”部分。
