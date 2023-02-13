---
product-area: projects
navigation-topic: manage-tasks
title: 在列表中编辑任务
description: 您可以通过编辑列表中显示的字段来编辑任务列表中的任务信息。 有关编辑任务的其他方法的信息，请参阅编辑任务。
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# 在列表中编辑任务 {#edit-tasks-in-a-list}

您可以通过编辑列表中显示的字段来编辑任务列表中的任务信息。 有关编辑任务的其他方法的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为任务和项目提供或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关编辑列表中任务的注意事项 {#considerations-about-editing-tasks-in-a-list}

在列表中编辑任务是同时更改多个任务的一种快速方法，可以清晰地查看所做的更改可能如何影响项目时间轴。

在列表中编辑任务时，请考虑以下事项：

* 与在“编辑框”中编辑任务时需要对该任务拥有管理权限不同，您只能在列表中编辑该任务，并且该任务具有Contribute权限。 这允许您编辑任务的以下有限信息：

   * 描述
   * 状态
   * 完成百分比
   * 自定义表单信息

      >[!NOTE]
      >
      >仅当您有权更新该字段时，才能编辑列表中的任务自定义字段。

   * 日志小时数
   * 修改分配
   * 查看财务信息
   * 添加费用、任务或问题

* 您可以在以下列表中编辑任务：

   * 项目的“任务”部分
   * 项目的子任务部分
   * 任务报告

      >[!NOTE]
      >
      >默认情况下，Workfront会自动将您对子任务部分或任务报表中的任务所做的更改保存到该报表中。

* 您可以控制Workfront何时将您对列表中的任务所做的更改保存到列表中。 您的更改可以自动保存，也可以手动保存。

   有关在Workfront保存您对列表中的任务所做的更改时进行配置的信息，请参阅 [在列表中编辑任务时选择保存选项](#select-a-save-option-when-editing-tasks-in-a-list) 章节。

## 在列表中编辑任务时选择保存选项 {#select-a-save-option-when-editing-tasks-in-a-list}

您可以决定在列表中对任务所做的更改在发生时自动保存到何处，或者是否要手动保存每个更改。

>[!IMPORTANT]
>
>根据您是自动还是手动保存任务，您可能会在编辑列表中的任务时覆盖其他人的信息。 有关Workfront如何保存您对与其他用户同时执行的任务所做的更改的信息，请参阅 [保存任务列表中并发更改的概述](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

当您在项目列表中保存所做更改时，如果某个项目选择了自动或自动更改和更改作为更新类型，则Workfront会更新项目时间轴以及所有项目内和跨项目依赖关系。 如果项目较大或存在大量依赖项，则时间轴计算可能需要较长时间。 根据您选择的保存更改的方法，某些编辑任务列表的方法可能比其他方法更快。

您可以控制Workfront何时将您对列表中的任务所做的更改保存到列表中。 存在以下情形： 

* 您可以在每次更新后让Workfront自动保存更改。

   有关信息，请参阅 [在列表中编辑任务并自动保存更改](#edit-tasks-in-a-list-and-automatically-save-changes) 在本文中。

* 您可以使用“保存”按钮手动控制何时一次应用多个更改。

   有关信息，请参阅 [在列表中编辑任务并手动保存更改](#edit-tasks-in-a-list-and-manually-save-changes) 在本文中。

### 在列表中编辑任务并自动保存更改 {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>如果您的项目有2000项以上的任务，或者如果项目有大量依赖项，则保存更改和所有项目依赖项的速度可能会较慢。

在自动保存任务列表更改时，请考虑以下事项：

* 您可以将自定义视图应用到任务列表，并编辑您有权更新的任何与任务相关的字段。
* 无法反转自动保存的更改。 这是默认设置。
* 当项目更新类型为“自动”或“自动”且“随时更改”时，Workfront会在每次更改后自动重新计算项目的时间轴以及所有项目内和跨项目依赖关系。 有关项目更新类型的信息，请参阅 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要编辑列表中的任务并自动保存更改，请执行以下操作：

1. 转到项目，然后单击 **任务** 中。
1. 单击 **计划模式菜单** ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，并确保 **自动保存** 选项。

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 编辑您有权手动更新的任何字段。

   ![](assets/inline-editing-a-task-350x26.png)

1. （可选）按 **Escape** 以取消更改。
1. 按Enter键保存对任务和项目时间轴所做的更改。
1. （可选）右键单击要修改的任务。

   或

   单击 **更多** 菜单 ![](assets/more-icon-task-list.png) 任务名称的右侧。

1. （可选）从以下选项中进行选择：

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
      <td><p>打开 <strong>编辑任务</strong> 框中，您可以在其中编辑任务。</p><p>有关编辑任务的信息，请参阅 <a href="#edit-tasks-in-a-list" class="MCXref xref">在列表中编辑任务</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td><p>删除任务。</p><p>有关删除任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td><p>按一个级别缩进任务。 </p><p>此选项仅在独立任务中显示。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td><p>按一级排除任务。 </p><p>此选项仅在子任务中显示。 </p></td> 
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
      <td role="rowheader">重复</td> 
      <td><p>在同一项目中创建任务的重复版本。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制到</td> 
      <td><p>将任务复制到其他项目。</p><p>有关复制和复制任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">移至</td> 
      <td><p>将任务移到其他项目。</p><p>有关移动任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">移动任务</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   更改会自动保存，您无法撤消这些更改。

### 在列表中编辑任务并手动保存更改 {#edit-tasks-in-a-list-and-manually-save-changes}

您可以手动保存对列表中的任务所做的更改。 以这种方式保存更改时，您可以灵活地在保存前撤消这些更改。

>[!TIP]
>
>* 在“子任务”部分或任务报表中编辑任务时，无法撤消对列表中的任务所做的更改。
>* 您可以反转的更改数量没有限制。 您可以逐个撤消所有任务，直到达到任务的原始状态。
>


手动保存任务列表中的更改时，请考虑以下事项：

* 要手动保存任务列表更改，您需要权限来同时管理任务和项目。
* 无法编辑项目。 用于编辑项目的选项处于禁用状态。
* 无法更新项目标题中的信息。 只有在手动保存任务列表中的更改时，才能执行以下操作：

   * 订阅项目。
   * 将项目添加到收藏夹列表。
   * 在列表中单击任务名称以打开任务。

* 批量编辑任务。 选择多个任务时，编辑图标会被禁用。
* Workfront仅在保存更改后才会触发有关您对任务所做的更改的通知。

有两种方法可以在列表中手动保存对任务所做的更改。 下面介绍了这两种方式。

* [选择“手动保存标准”选项时，手动保存任务列表中的更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [选择“手动保存时间轴计划”选项时，手动保存任务列表中的更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 选择“手动保存标准”选项时，手动保存任务列表中的更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>如果项目有2000多项任务，或者如果项目有许多依赖项，则可能需要一些时间来直观地识别您对任务所做的更改以及这些更改如何影响所有项目依赖项。 在这种情况下，如果您的项目有2000项以上的任务，或者如果项目有大量依赖项，则保存更改可能需要更长的时间。

在选择“手动保存标准”选项后更新列表中的任务时，请考虑以下事项：

* 您可以将自定义视图应用于任务列表，并编辑您有权在该视图中管理的任何与任务相关的字段。
* 当项目更新类型为“自动”或“自动”且“更改时”时，Workfront会在您单击“保存”后计算项目的时间轴以及所有项目内和跨项目依赖项。 有关项目更新类型的信息，请参阅 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要在选择“手动保存标准”选项时在列表中编辑任务，请执行以下操作：

1. 转到项目，然后单击 **任务** 部分。
1. 单击 **计划模式** 菜单 ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，然后选择 **手动保存**，然后单击 **标准** > **应用**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   此时会显示工具栏设置，其中包含用于撤消、重做和保存更改的选项。

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 单击您有权手动更新的任何字段。 该字段将变得可编辑，您可以进行更改。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按Enter键可临时保存您所做的更改。
1. （可选）单击 **“撤消”图标** ![](assets/undo-icon-on-task-list.png) 反转更改并将字段返回到其原始状态。
1. （可选并视情况而定）单击 **“重做”图标** ![](assets/redo-icon-on-task-list.png) 若要恢复更改，请撤消。

1. （可选）右键单击要修改的任务。

   或

   单击 **更多** 菜单 ![](assets/more-icon-task-list.png).

1. （可选）从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新选项卡中打开</strong> </td> 
      <td>在新的浏览器选项卡中打开任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td>有关删除任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td> <p>按一个级别缩进任务。 </p> <p>此选项仅在独立任务中显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td> <p>按一级排除任务。 </p> <p>此选项仅在子任务中显示。 </p> </td> 
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
      <td role="rowheader">重复</td> 
      <td> <p>在同一项目中创建任务的重复版本。 </p> <p>有关复制和复制任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront会在您更改任务时间轴时更新所有项目内和跨项目依赖关系。
1. 单击 **保存** 当您想要永久更改任务并保存项目时间轴时。

#### 选择“手动保存时间轴计划”选项时，手动保存任务列表中的更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

保存更改和所有项目依赖项的速度都更快。 这不适用于任务超过2000个的项目。

>[!IMPORTANT]
>
>我们建议您在编辑大量具有大量依赖关系的数百个以上任务时使用此选项。 使用此选项，可以比使用“手动保存”选项更快地直观地识别更改。

在任务列表中使用“手动保存时间轴计划”选项时，请考虑以下事项：

* 您不能将“手动保存时间轴计划”选项应用于任务超过2000个的项目。
* 不能将自定义视图、过滤器或分组应用到任务列表。 “视图”、“过滤器”和“分组”下拉菜单以及“敏捷视图”图标处于禁用状态。 默认应用的视图包含有限数量的字段。
* 当项目更新类型为“自动”或“自动”且“更改时”时，在每次更改后，会自动计算项目的时间轴和所有项目内依赖项。
* 单击“保存”(Save)后，如果项目更新类型为“自动”(Automatic)或“自动”(Automatic)和“更改时”(On Change)，则会计算跨项目依赖关系。 有关项目更新类型的信息，请参阅 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要在使用“手动保存时间轴计划”选项时编辑列表中的任务，请执行以下操作：

1. 转到项目，然后单击 **任务** 中。
1. 单击 **计划模式** 菜单 ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，然后选择 **手动保存**，然后单击 **时间轴规划**> **应用**.

   对于具有2000项以上任务的项目，此选项会变暗。

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >从此页面导航离开时，Workfront会重新启用自动保存选项。

   请注意列表中的以下更改：

   * “视图”、“分组”和“过滤器”下拉菜单将被删除，视图将被以下字段替换：

      * 任务编号
      * 任务名称
      * 限制类型
      * 持续时间
      * 计划开始日期
      * 计划完成日期
      * 前置任务
      * 分配
      * 状态
      * 完成百分比
   * 此时会删除Agile视图图标。
   * 此时会显示工具栏设置，其中包含用于撤消、重做和保存更改的选项。

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. 编辑您有权手动更新的任何字段。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按Enter键可临时保存您所做的更改。
1. （可选）单击 **“撤消”图标** ![](assets/undo-icon-on-task-list.png) 反转更改并将字段返回到其原始状态。
1. （可选并视情况而定）单击 **“重做”图标** ![](assets/redo-icon-on-task-list.png) 要恢复更改，请撤消。

1. （可选）右键单击要修改的任务

   或

   单击 **更多** 菜单 ![](assets/more-icon-task-list.png).

1. 从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新选项卡中打开</strong> </td> 
      <td>在新的浏览器选项卡中打开任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td>有关删除任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">删除任务</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">缩进</td> 
      <td> <p>按一个级别缩进任务。 </p> <p>此选项仅在独立任务中显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升级</td> 
      <td> <p>按一级排除任务。 </p> <p>此选项仅在子任务中显示。 </p> </td> 
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
      <td role="rowheader">重复</td> 
      <td> <p>在同一项目中创建任务的重复版本。 </p> <p>有关复制和复制任务的信息，请参阅 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">复制和复制任务</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront会在您更改任务的时间轴时更新所有项目内和跨项目依赖关系。
1. 单击 **保存** 当您想要永久更改任务并保存项目时间轴时。

## 使用“摘要”编辑列表中的任务

1. 转到包含要编辑的任务的项目。
1. 单击&#x200B;**任务** 中。

   此时将显示项目中的任务列表。

1. 单击“更多”菜单 ![](assets/more-icon-task-list.png) 在任务名称后，单击 **打开摘要**. 选择要编辑的任务，然后单击 **“打开摘要”图标** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) 列表右上角。

   的 **概要** 打开。

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. （可选）单击 **X图标** 在“摘要”的右上角，关闭面板并编辑内嵌的任务。

   按照有关在列表中编辑任务的步骤进行内联编辑。

   有关在列表中编辑任务的信息，请参阅 [有关编辑列表中任务的注意事项](#considerations-about-editing-tasks-in-a-list) 在本文中。

1. （可选）在 **更新** 的上界。
1. 单击以下任意图标或区域以转到任务并编辑任务级别的信息：

   | 文档 | 单击 **单击此处添加** 向任务中添加文档。 |
   |---|---|
   | 详细信息 | 单击以更新有关任务的信息。 |
   | 自定义表单 | 单击可添加或删除自定义Forms或更新表单上的信息。 |
   | 小时 | 单击以记录小时。 |
   | 审批 | 单击以添加任务批准。 |

   {style=&quot;table-layout:auto&quot;}

1. 单击浏览器上的“返回”按钮，以在您完成任务更新后返回到任务列表。

## 批量编辑任务

您可以一次编辑多个任务。 确保您对任务具有管理权限，以便能够编辑这些任务。

1. 转到包含要批量编辑的任务的项目。
1. 单击 **任务** 中。
1. 确保 **自动保存** 选项。

   >[!IMPORTANT]
   >
   >手动保存任务时，无法批量编辑任务。

   有关在列表中保存任务更改的方法的更多信息，请参阅部分 [有关编辑列表中任务的注意事项](#considerations-about-editing-tasks-in-a-list) 在本文中。

1. 在任务列表中选择多个任务。
1. 单击 **“编辑”图标** ![](assets/qs-edit-icon.png).

   的 **编辑任务** 对话框。

1. 指定要更改的所有选定任务的信息。

   编辑所有任务的信息与编辑一个任务的信息相同。 如果要编辑任务持续时间，所选任务必须具有相同的任务约束；否则， **持续时间** 字段中不填充。

   有关编辑任务的详细信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >您正在更改的所有选定任务的信息将覆盖有关单个任务的现有信息，但 **分配** 字段。 在批量编辑中添加新的代理人将将该代理人添加到所有选定任务中。 如果其他受分配者被分配给选定的任务，则除了通过批量编辑添加的任务之外，这些受分配者还会被分配。

1. 单击 **自定义Forms** 编辑附加到所有选定任务的自定义表单。 列表中仅显示活动的自定义表单。

   如果所选任务没有任何常见的自定义表单，则此部分中不列出任何表单。

   您只能编辑表单上附加到所有选定任务且您有权编辑的字段。

1. （可选）在自定义Forms部分中，选择 **重新计算自定义表达式** 选项，以确保附加到所选任务的自定义表单上的所有计算量度自定义字段都是最新的。
1. 单击 **保存更改**.

   现在，您所做的所有更改在所有选定任务上均可见。

有关批量编辑自定义表单的信息，请参阅 [管理附加到对象的自定义表单](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
