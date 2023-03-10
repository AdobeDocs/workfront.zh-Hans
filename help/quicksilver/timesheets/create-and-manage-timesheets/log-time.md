---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 记录时间
description: 您可以在&nbsp；Adobe Workfront中记录工作项的时间，以指示您处理这些工作项的小时数。 您还可以记录与工作无关的时间，如休假、病假或会议时间。 您的登录时间显示在您的时间表中。
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '3000'
ht-degree: 0%

---

# 记录时间

您可以在Adobe Workfront中记录工作项的时间，以指示您在这些工作项上花费的小时数。 您还可以记录与工作无关的时间，如休假、病假或会议时间。 您的登录时间显示在您的时间表中。

有关可登录Workfront的小时类型的更多信息，请参阅 [管理小时类型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 访问要求

<!--drafted for P&P - replace the table:

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
   <td> <p>Current license: Light or higher</p>
   <p>Review or higher</p> 
   <p><b>NOTE</b></p>

   <ul><li>Reviewers can log only General Hours in a timesheet</li>
   <li>You must have a Work license or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限，才能执行本文中的步骤并记录特定于项目的小时数：

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
   <td> <p>审核或更高</p> 
   <p><b>注释</b></p>

<ul><li>查看者只能在时间表中记录常规小时数</li>
   <li>您必须拥有工作许可证或更高许可证才能记录项目、任务或问题的小时数</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑您记录时间的工作项类型的访问权限 </p> <p>例如，您需要对问题的编辑访问权限，以记录问题的时间</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在您记录时间的工作项的Contribute或更高权限，包括“记录小时数”权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在Workfront中记录时间时的注意事项

* 您可以记录项目、任务或问题的时间，也可以直接在时间表中记录时间。

   有关创建时间表的信息，请参阅 [创建一次性时间表](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* 通过非时间表工具记录的所有时间都会显示在相应时间段的时间表中。
* 非当前项目中的任务和问题不会预填充到时间表中。
* 在时间表中记录的时间会立即应用于任务、问题或项目。
* 时间表包括所有已记录日期的总时间。 始终包括周末，即使时间线计算已配置为排除它们（如中所述） [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md))。
* 时间表中显示的最大项目数为45。 如果日期与时间表时间范围匹配的项目超过45个，则仅显示最近更新的项目。
* 已记帐记帐记录中包含的小时条目将灰显，无法在时间表中编辑。 有关更多信息，请参阅 [创建开票记录](../../manage-work/projects/project-finances/create-billing-records.md).

## 记录时间

您可以在Workfront的以下区域记录时间：

* [时间表](#timesheet)
* [主页](#home)
* [项目、任务或问题](#project-task-or-issue)
* [摘要面板](#summary-panel)
* [展示板](#boards)
* [移动应用程序](#mobile-app)

### 时间表 {#timesheet}

您可以在时间表上记录常规小时数或项目特定小时数。

>[!NOTE]
>
>查看分配给时间表配置文件的用户可查看时间表选项卡并记录常规小时数。 但是，他们无法记录时间表上显示的任何分配给他们的任务或问题的小时数。

1. 单击 [!UICONTROL **主菜单**] 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 [!UICONTROL **时间表**]. 默认情况下显示您当前的工时表。
   ![时间表](assets/timesheet-redesigned-nwe.png)

   该时间表已预填充在该时间表的时间范围内分配给您的项目。 有关如何预填充时间表的信息，请参阅 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 如果在时间表上没有看到某个项目，则可以添加该项目。

   >[!NOTE]
   >
   >时间表只会预填充分配给您的项目。 它不会预先填充分配给您的团队或工作角色的项目。
   >
   >在分配给您团队的项目上单击处理它会将项目分配给您，该项目将显示在您的时间表中。


1. （可选）单击 **全屏** 图标 ![](assets/full-screen.png) 以全屏模式显示时间表，然后单击 **退出全屏** ![](assets/exit-full-screen.png) 图标以返回到时间表。

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. （可选）要将项目、任务或问题添加到时间表，请单击 **添加项目** 下拉菜单，然后单击 **添加项目**， **添加任务**，或 **添加问题**.

   此时将显示项目、任务或问题的列表。

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. （可选）单击搜索图标 ![搜索项目](assets/search-icon.png) 使用关键字搜索特定项目以添加到时间表。

1. （可选）展开过滤器、视图或分组下拉菜单以应用或自定义一个下拉菜单，并查看所需的项目信息。

1. 在列表中选择一个或多个项目，然后单击 **添加**.

   >[!NOTE]
   >
   >将任务或问题添加到时间表时，也会添加项目。


1. （视情况而定）如果您一次添加50个或更多项目，则会显示一条确认消息，其中显示添加到时间表的项目数量。

   单击 **全部添加** 以添加所有项目，或单击 **取消** 停止添加选定的项目，然后 **取消** 以关闭项目列表。

   任务和问题列在项目的名称下。

   >[!NOTE]
   >
   >您手动添加到时间表的项目已固定，并将停留在当前和未来的时间表中，直到您手动取消固定它们以将其删除。 有关取消固定项目以将其从时间表中删除的信息，请继续执行步骤10。

   <!--(ensure this stays accurate)-->

1. （可选）单击 **折叠** ![](assets/collapse-icon.png) 或 **展开** ![](assets/expand-icon.png) 项目名称旁边的图标，用于显示或隐藏项目的任务和问题列表。


   >[!TIP]
   >
   >   使用标准QWERTY键盘时，在单击时间表中的项目名称后，按下面一组键折叠或展开该项目：
   >   * 要展开项目并显示其工作项，请执行以下操作：
      >     * Windows计算机的Shift + Alt +向上箭头
      >     * 适用于Mac计算机的Shift + Option +向上箭头
   >   * 要折叠项目并隐藏其工作项，请执行以下操作：
      >     * Windows计算机的Shift + Alt +向下箭头
      >     * Mac计算机的Shift + Option +向下箭头。



1. （可选）要手动固定自动显示在时间表上的项目，请将鼠标悬停在该项目的名称上，然后单击 **固定** 图标 ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   在单击时间表中的项目后使用标准QWERTY键盘时，请按以下一组键以固定项目：
   >   * Option + P(适用于Windows和Mac计算机)。



1. （可选）单击搜索图标 ![](assets/search-icon.png) 并开始键入关键字以在时间表上查找项目、任务或问题。

1. （可选）如果您手动添加了某个项目（如步骤3-6中所述），并且尚未通过取消固定来记录时间，则可以从时间表中删除该项目（项目、任务或问题）。 <!--ensure this stays accurate-->

   您无法根据配置为预填充时间表的Workfront系统或组中的时间表偏好设置，自动删除时间表中包含的项目（如中所述） [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   要从工时表中删除手动添加的项目，请执行以下操作：

   1. 确保没有针对该项目记录任何时间。
   1. 单击 **取消固定** 图标 ![固定项目](assets/pin-icon.png) ，以从时间表取消固定该项目。

   >[!TIP]
   >
   >   单击时间表中的项目后使用标准QWERTY键盘时，请按以下一组键取消固定项目：
   >   * Option + P(适用于Windows和Mac计算机)。



   刷新页面后，该项目将从时间表删除。

1. （视情况而定）如果您的Workfront或组管理员启用了 **手动将工作角色分配给小时条目** 设置时，从下拉菜单中选择工作角色。 默认情况下，将显示分配给工作项时指定的角色。 如果您未在该对象上分配角色，则您的主要角色将显示为默认角色。 有关此设置的更多信息，请参阅文章 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![在时间表中记录多个角色的时间](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. （可选）单击 **+** 图标以添加另一行，然后从 [!UICONTROL 小时类型] 列来记录不同小时类型的时间。

   ![小时类型下拉菜单](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   根据您的操作系统或浏览器，在使用标准QWERTY键盘时，请按以下一组键以添加另一行：
   >   * 对于Windows计算机，按Ctrl + Option + +
   >   * 适用于Mac计算机的Cmd + Option + +


   可用小时类型取决于在系统、项目和用户级别定义的内容，如中所述 [定义工时表的小时类型和可用性](define-hour-types-and-availability.md).

   工时表关闭后无法更改小时类型。

   >[!TIP]
   >
   >如果您以前记录时间，而您选择的小时类型现在已停用，则记录时间的整行将灰显。 选择其他小时类型并刷新页面将从下拉列表中删除已停用的小时类型选项，因此您无法向该小时类型添加其他小时。
   >
   >如果要将停用的小时类型与过去记录的时间相关联，请考虑为要记录额外时间的工作项添加一个新行，并选择新的小时类型。

1. 单击 **delete** 图标  ![](assets/delete.png) ，以将其删除。 同时也会删除为角色记录的任何时间。

   >[!TIP]
   >
   >   根据您的操作系统或浏览器，在使用标准QWERTY键盘时，请按以下一组键以删除行：
   >   * Ctrl + Option + — 适用于Windows计算机
   >   * Cmd + Option + — 适用于Mac计算机



1. 在时间表的时间线部分指定您要在任何给定天上登录的时间量，然后单击小时框外部以保存小时条目。 小时数会自动保存。 您记录时间的行以浅蓝色突出显示，小时条目框以深蓝色列出。

   ![时间表中的记录时间框](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   您以小时或天为单位记录时间。 此设置由拥有计划许可证的用户或系统管理员配置，如中所述 [配置时间是以小时还是天为单位记录](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >如果您记录时间的工作角色已更改，并且 **手动将工作角色分配给小时条目** 设置已被禁用，您必须手动保存时间条目。 仅当不再记录已更改的工作角色的时间时，时间表才会再次自动节省您的时间。
   >
   >如果角色已更改，并且 **手动将工作角色分配给小时条目** 设置已启用，您可以记录时间或更新角色，并且您的更改会自动保存。

1. （可选）在时间表标题的加班字段中指定加班时间。

   >[!TIP]
   >
   >您不能记录的加班小时数大于时间表上当前的总小时数。 例如，到目前为止，如果您在时间表上记录了7小时，则无法记录8小时的加班。

1. （可选）单击 **注释** 为小时条目添加评论。

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   在单击小时输入框后使用标准QWERTY键盘时，请按以下一组键以打开注释框：
   >   * Shift + F2，适用于Windows和Mac计算机。


1. 单击 **完成** 以保存注释。

   >[!TIP]
   >
   >   使用标准QWERTY键盘时，从注释框内，按下面一组键以保存注释：
   >   * 对于Windows计算机，按Ctrl + Enter。
   >   * Mac计算机的Cmd + Return。



1. （可选）单击 **显示评论** 在工具栏中，在工作项下显示小时条目注释。

   ![在时间表项目下列出的备注](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   您对时间表所做的所有更改都会自动保存。

1. （可选）单击任务或问题的行，然后单击 **打开摘要** ，以添加更新或更新有关任务或问题的信息。 右侧将打开“摘要”面板。

   ![summary-panel-for-task-open-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   您的更新显示在与记录时间关联的工作项的更新区域中。

   >[!TIP]
   >
   >您无法评论项目或常规时间小时条目。

1. 单击 [!UICONTROL **关闭摘要**] 以关闭“摘要”面板并返回到时间表。

1. （可选）单击 [!UICONTROL **更新**] 然后，在左侧面板中为时间表添加更新。 有关Workfront更新的更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesign-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **关闭**：完成更新后关闭时间表。 仅当您的时间表未与批准者关联时，此选项才可用。

   * **提交以供审批：** 仅当时间表上有审批者时，此选项才可用。 保存更改并提交以供审批。 在关闭时间表后，您可以通过单击 **撤消**，如果尚未获得批准。 有关更多信息，请参阅 [提交工时表以供审批](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **拒绝**：当您是时间表批准者并且时间表已提交给您进行批准时，会显示此选项。 单击该选项会将时间表的状态更改为“已拒绝”，并且时间表保持打开状态。

   * **批准**：当您是时间表批准者并且时间表已提交给您进行批准时，会显示此选项。 单击该选项会将时间表状态更改为“已批准”并关闭时间表。
   >[!TIP]
   >
   >当您是系统管理员并且时间表与批准者相关联时，拒绝和批准选项也会显示在您的时间表上。

1. （视情况而定）如果您已关闭或已提交时间表以供审批，请单击以下选项之一：

   * **重新打开**：此选项适用于您已经关闭并且没有批准者的时间表，或者已经批准的时间表。 重新打开时间表以修改小时条目。
   * **撤消**：此选项适用于已提交审批但尚未批准或拒绝的时间表。 单击 **撤消** 以重新打开时间表并修改小时条目。

### 主页 {#home}

您可以在主页中记录特定于项目的时间。

有关使用“主页”区域的一般信息，请参阅 [使用“主页”区域](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

要从主页区域记录工作项的时间，请执行以下操作：

1. 在 **工作列表** 区域，选择要记录时间的项目。
1. 在右侧面板中，单击 **记录时间**.

   ![](assets/log-time-home-350x181.png)

1. 在 **输入小时** 下拉菜单中，选择相应的小时类型。\
   可用小时类型取决于在系统、项目和用户级别定义的内容，如中所述 [定义工时表的小时类型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. （视情况而定）如果您的Workfront或组管理员启用了 **手动将工作角色分配给小时条目** 设置时，从下拉菜单中选择工作角色。 默认情况下，将显示分配给工作项时指定的角色。 如果您未在该对象上分配角色，则您的主要角色将显示为默认角色。 有关此设置的更多信息，请参阅文章 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. 指定要记录的时间，然后单击 **记录时间**.

### 项目、任务或问题 {#project-task-or-issue}

您可以记录项目、任务或问题的项目特定时间。

#### 记录时间所需的权限

要记录项目、任务或问题的小时数，您需要具有特定权限。 您可以在项目、任务或问题的两个位置记录时间：

* [“更新”选项卡](#updates-tab)
* [“小时”选项卡](#hours-tab)

##### “更新”选项卡{#updates-tab}

在项目、任务或问题的更新选项卡上记录小时数之前，需要满足以下条件：

* 您必须拥有工作或计划许可证。
* 您必须至少拥有对项目、任务或问题的贡献权限才能访问记录小时数。\
   有关授予项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* 如果要直接将时间记录到项目，Workfront管理员必须启用“直接在项目上记录时间”设置，该设置位于 [!UICONTROL **时间表和小时数** ]> [!UICONTROL **首选项**].\
   有关允许用户直接将小时数记录到项目的更多信息，请参阅 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### “小时”选项卡{#hours-tab}

在项目、任务或问题的小时数选项卡上记录小时数之前，需要满足以下条件：

* 您必须是系统管理员。

或者，您必须具备以下所有条件：

* 您必须拥有对时间表和小时数具有管理访问权限的计划许可证。 有关授予对时间表和小时数的管理访问权限的更多信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* 您必须至少具有项目的Contribute权限，并且有权访问记录小时数。 有关授予项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* 如果要直接将时间记录到项目，您的Workfront管理员必须在“时间表和小时数”>“首选项”下启用直接在项目上记录时间设置。 有关允许用户直接将小时数记录到项目的更多信息，请参阅 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

要记录项目、任务或问题的时间，请执行以下操作：

1. 导航到项目、任务或问题。
1. 在左侧面板中，选择 **小时**.
1. 单击 **记录时间**.

   此时将显示记录小时数对话框。

1. 指定以下信息：

   * **所有者：** 默认情况下，您的名称会显示在此字段中。\
      如果要记录另一个用户的小时数，请指定其名称。

   * **小时**：输入项目、任务或问题的小时数。
   * **小时类型**：从下拉菜单中选择小时类型（如果它与默认显示的类型不同）。

      根据系统中配置的小时类型，此处的选项可能会有所不同。 有关配置小时类型的更多信息，请参见 [定义工时表的小时类型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **工作角色**：（视情况而定）如果您的Workfront或组管理员已启用 **手动将工作角色分配给小时条目** 设置，选择 **工作角色** 下拉菜单中。 默认情况下，将显示指定给对象时指定的角色。 如果您未在该对象上分配“角色”，则您的“主要角色”将显示为默认值。 有关此设置的更多信息，请参阅文章 [配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. 单击 **记录小时数**.

### 摘要面板

您可以在“摘要”面板中记录任务和问题的时间。
有关更多信息，请参阅 [摘要概述](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### 展示板 {#boards}

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您可以在Workfront展示板上的已连接信息卡上记录时间。 这是与任务或问题的记录时间相同的过程，卡片上记录的小时数保存在连接的任务或问题上。
有关更多信息，请参阅 [在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### 移动应用程序 {#mobile-app}

您可以从Workfront移动设备应用程序记录时间。
有关更多信息，请参阅 [适用于Android的Adobe Workfront](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) 或 [适用于iOS的Adobe Workfront](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
