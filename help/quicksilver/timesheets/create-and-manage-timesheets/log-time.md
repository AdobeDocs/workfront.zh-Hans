---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 日志时间
description: 您可以在Adobe Workfront中记录工作项目的时间(&n)，以指示您在工作项目上花费的小时数。 您还可以记录与工作无关的时间，如休假、病假或在会议中花费的时间。 您登录的时间显示在您的时间表中。
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 27e9cfff363ab38c6469b99a8cbb04439f2df61c
workflow-type: tm+mt
source-wordcount: '2979'
ht-degree: 0%

---

# 日志时间

您可以在Adobe Workfront中记录工作项的时间，以指示您在这些工作项上花费的小时数。 您还可以记录与工作无关的时间，如休假、病假或在会议中花费的时间。 您登录的时间显示在您的时间表中。

有关可登录Workfront的小时数类型的更多信息，请参阅 [管理小时类型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

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
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
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

您必须具有以下访问权限才能执行本文中的步骤并记录项目特定小时数：

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
   <td> <ul><li>查看或更高版本，以记录工时单中的一般工时</li>
   <li> 工作或更高人员可记录项目、任务或问题的小时数</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对您记录时间的工作项类型的访问权限 </p> <p>例如，您需要“编辑”对“问题”的访问权限，才能记录问题的时间</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对您登录时间的工作项目具有包含“记录时间”权限的参与者或更高权限。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在Workfront中记录时间时的注意事项

* 您可以记录项目、任务或问题的时间，也可以直接在工时单中记录时间。

   有关创建工时单的信息，请参阅 [创建一次性工时单](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* 通过工时表以外的工具记录的所有时间，都显示在相应时间段的时间表中。
* 项目中非当前任务和问题未预填充到时间表中。
* 在时间表中记录的时间会立即应用于任务、问题或项目。
* 工时单包括所有记录日期的总时间。 即使将时间轴计算配置为排除周末(如 [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md))。
* 时间表中显示的最大项目数为45个。 如果有45个以上的项目的日期与时间表时间范围匹配，则仅显示最近更新的项目。
* 计费账单记录中包含的小时条目将变暗，无法在工时单中编辑。 有关更多信息，请参阅 [创建帐单记录](../../manage-work/projects/project-finances/create-billing-records.md).

## 日志时间

您可以在Workfront的以下区域登录时间：

* [时间表](#timesheet)
* [主页](#home)
* [项目、任务或问题](#project-task-or-issue)
* [“摘要”面板](#summary-panel)
* [展示板](#boards)
* [移动设备应用程序](#mobile-app)

### 时间表 {#timesheet}

您可以记录时间表上的一般小时数或项目特定小时数。

>[!NOTE]
>
>查看分配给时间表配置文件的用户可以查看时间表选项卡并记录一般小时数。 但是，他们无法记录工时单上显示的分配给他们的任何任务或问题。

1. 单击 [!UICONTROL **主菜单**] 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 [!UICONTROL **工时单**]. 默认情况下，会显示您当前的时间表。
   ![时间表](assets/timesheet-redesigned-nwe.png)

   时间表中预填充了在时间表的时间范围内分配给您的项目。 有关如何预填充工时单的信息，请参阅 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 如果在时间表上没有看到项目，可以添加它。

   >[!NOTE]
   >
   >工时单仅预填充分配给您的项目。 它不会预填充分配给团队或工作角色的项目。
   >
   >对分配给您的团队的项目单击Work On It（处理项目），会将项目分配给您，该项目将显示在您的时间表中。


1. （可选）单击 **全屏** 图标 ![](assets/full-screen.png) 要以全屏模式显示时间表，请单击 **退出 — 全屏** ![](assets/exit-full-screen.png) 图标返回到工时单。

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. （可选）要将项目、任务或问题添加到时间表，请单击 **添加项目** 时间表左上角的下拉菜单，然后单击 **添加项目**, **添加任务**&#x200B;或 **添加问题**.

   此时将显示项目、任务或问题列表。

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. （可选）单击搜索图标 ![搜索项目](assets/search-icon.png) 使用关键字搜索特定项目以添加到工时单。

1. （可选）展开过滤器、查看或分组下拉菜单以应用或自定义一个菜单，并查看您需要的项目信息。

1. 在列表中选择一个或多个项目，然后单击 **添加**.

   >[!NOTE]
   >
   >向时间表添加任务或问题时，也会添加项目。


1. （视情况而定）如果一次添加50个或多个项目，则会显示一条确认消息，其中显示了添加到工时单的项目数。

   单击 **全部添加** 添加所有项目或单击 **取消** 要停止添加选定项目，请 **取消** 来关闭项目列表。

   任务和问题列在项目名称下。

   >[!NOTE]
   >
   >手动添加到时间表的项目将被固定，并将保留在当前和未来的时间表上，直到您手动取消固定它们以删除它们为止。 有关取消固定项目以将其从时间表中删除的信息，请继续执行步骤10。

   <!--(ensure this stays accurate)-->

1. （可选）单击 **折叠** ![](assets/collapse-icon.png) 或 **展开** ![](assets/expand-icon.png) 项目名称旁边的图标，用于显示或隐藏项目的任务和问题列表。


   >[!TIP]
   >
   >   使用标准QWERTY键盘时，在单击时间表中项目的名称后，按下列键集可折叠或展开项目：
   >   * 要展开项目并显示其工作项，请执行以下操作：
      >     * 适用于Windows计算机的Shift + Alt +向上箭头
      >     * Shift + Option +向上箭头(用于Mac计算机)
   >   * 要折叠项目并隐藏其工作项，请执行以下操作：
      >     * 适用于Windows计算机的Shift + Alt +向下箭头
      >     * Shift + Option +向下箭头(用于Mac计算机)。



1. （可选）要手动固定显示在时间表上的项目，请将鼠标悬停在项目名称上，然后单击 **pin** 图标 ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   在单击时间表中的某个项目后使用标准QWERTY键盘时，按下列键集可固定某个项目：
   >   * 选项+ P适用于Windows和Mac计算机。



1. （可选）单击搜索图标 ![](assets/search-icon.png) 然后开始键入关键字，以查找工时单上的项目、任务或问题。

1. （可选）如果您手动添加某个项目（如步骤3-6中所述），并且尚未通过取消固定该项目记录时间，则可以从工时表中删除该项目（项目、任务或问题）。 <!--ensure this stays accurate-->

   您不能根据Workfront系统或组中配置为预填充工时单的工时单首选项(如 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   从手动添加的工时单中删除项目：

   1. 确保没有针对该项目记录任何时间。
   1. 单击 **取消固定** 图标 ![固定项目](assets/pin-icon.png) 项目旁边，以从工时单中取消固定项目。

   >[!TIP]
   >
   >   在单击时间表中的某个项目后使用标准QWERTY键盘时，按下列键集可取消固定某个项目：
   >   * 选项+ P适用于Windows和Mac计算机。



   刷新页面后，该项目将从时间表中删除。

1. （视情况而定）如果您的Workfront或组管理员已 **手动将作业角色分配给小时条目** 设置时，从下拉菜单中选择作业角色。 默认情况下，在将您分配到工作项时指定的角色会显示。 如果未在对象上分配角色，则默认将显示“主角色”。 有关此设置的更多信息，请参阅文章 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![工时单中多个角色的日志时间](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. （可选）单击 **+** 图标以添加另一行，然后从 [!UICONTROL 小时类型] 列来记录不同小时类型的时间。

   ![“小时类型”下拉菜单](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   根据您的操作系统或浏览器以及使用标准QWERTY键盘时的不同，按下列键集以添加另一行：
   >   * Ctrl + Option + +适用于Windows计算机
   >   * 适用于Mac计算机的Cmd + Option + +


   小时类型可用，具体取决于在系统、项目和用户级别定义的内容，如 [定义工时单的工时类型和可用性](define-hour-types-and-availability.md).

   关闭时间表后，无法更改小时类型。

   >[!TIP]
   >
   >如果您之前已记录时间，并且现在已停用您选择的小时类型，则记录时间的整行将灰显。 选择另一个小时类型并刷新页面会从下拉列表中选择已停用的小时类型选项，这样您就无法向该小时类型添加其他小时。
   >
   >如果要将停用的小时类型与过去记录的时间关联，请考虑为要记录其他时间的工作项目添加新行，并选择新的小时类型。

1. 单击 **删除** 图标  ![](assets/delete.png) 作业角色旁边，以将其删除。 为角色记录的任何时间也会被删除。

   >[!TIP]
   >
   >   根据您的操作系统或浏览器以及使用标准QWERTY键盘时，按下列键集以删除行：
   >   * Ctrl + Option + — 适用于Windows计算机
   >   * Cmd + Option + — 适用于Mac计算机



1. 在时间表的时间轴部分中指定要在任意给定日期登录的时间，然后单击小时框外以保存小时条目。 小时会自动保存。 您记录时间的行以浅蓝色突出显示，小时进入框以深蓝色列出。

   ![工时单中的日志时间框](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   您可以在数小时或数天内记录时间。 此设置由具有计划许可证的用户或系统管理员配置，如 [配置时间是以小时还是天记录](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >如果您记录时间的作业角色已更改，并且 **手动将作业角色分配给小时条目** 设置被禁用，您必须手动保存时间条目。 只有在没有为已更改的作业角色记录的任何时间时，时间表才会自动保存您的时间。
   >
   >如果角色已更改，并且 **手动将作业角色分配给小时条目** 设置后，您可以记录时间或更新角色，并且更改会自动保存。

1. （可选）在时间表标题的“超时”字段中指定超时量。

   >[!TIP]
   >
   >您无法记录超过工时单上当前总工时数的加班小时数。 例如，如果迄今为止已在时间表上记录了7小时，则无法记录8小时的加班时间。

1. （可选）单击 **注释** 为小时条目添加评论。

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   在单击小时输入框后使用标准QWERTY键盘时，按下列键集以打开评论框：
   >   * Shift + F2(适用于Windows和Mac计算机)。


1. 单击 **完成** 来保存评论。

   >[!TIP]
   >
   >   使用标准QWERTY键盘时，从评论框内按下列键集以保存评论：
   >   * Ctrl + Enter（Windows计算机）。
   >   * Cmd +返回Mac计算机。



1. （可选）单击 **显示注释** 在工具栏中，在工作项目下显示小时条目评论。

   ![在工时单中项目下列出的注释](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   您对时间表所做的所有更改都会自动保存。

1. （可选）单击任务或问题的行，然后单击 **打开摘要** 用于添加有关任务或问题的更新或更新信息的时间表右上角。 将在右侧打开“摘要”面板。

   ![summary-panel-for task-opened-in-timese](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   您的更新显示在与记录时间关联的工作项的“更新”区域。

   >[!TIP]
   >
   >您无法对项目或“一般时间”小时条目进行注释。

1. 单击 [!UICONTROL **关闭摘要**] 关闭“摘要”面板并返回工时单。

1. （可选）单击 [!UICONTROL **更新**] 在左侧面板中，添加时间表的更新。 有关Workfront更新的更多信息，请参阅 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redied-timeslet-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **关闭**:完成更新时间表时关闭该时间表。 仅当您的时间表未与审批者关联时，此选项才可用。

   * **提交以供审批：** 此选项仅在时间表有审批者时可用。 保存更改并提交以供审批。 您可以在关闭时间表后通过单击 **召回**，则不会在以下情况中发生更改。 有关更多信息，请参阅 [提交时间表以供审批](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **拒绝**:当您是时间表审批者，并且时间表已提交您以供审批时，将显示此选项。 单击它可将时间表的状态更改为“已拒绝”，并且时间表保持打开状态。

   * **批准**:当您是时间表审批者，并且时间表已提交您以供审批时，将显示此选项。 单击它可将工时单的状态更改为“已批准”并关闭工时单。
   >[!TIP]
   >
   >如果您是系统管理员，并且时间表与审批者关联，则“拒绝”和“批准”选项也会显示在您的时间表上。

1. （视情况而定）如果已关闭或已提交工时单以供审批，请单击以下选项之一：

   * **重新打开**:此选项适用于已关闭且没有批准者的时间表或已批准的时间表。 重新打开时间表以修改小时条目。
   * **召回**:此选项适用于已提交以供审批但尚未获得批准或拒绝的时间表。 单击 **召回** 重新打开工时单并修改工时条目。

### 主页 {#home}

您可以在主页中记录特定于项目的时间。

有关使用“主页”区域的一般信息，请参阅 [使用主页区域](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

要从“主页”区域记录工作项的时间，请执行以下操作：

1. 在 **工作列表** 区域，选择要记录时间的项目。
1. 在右侧面板中，单击 **日志时间**.

   ![](assets/log-time-home-350x181.png)

1. 在 **输入小时** 下拉菜单中，选择相应的小时类型。\
   小时类型可用，具体取决于在系统、项目和用户级别定义的内容，如 [定义工时单的工时类型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. （视情况而定）如果您的Workfront或组管理员已 **手动将作业角色分配给小时条目** 设置时，从下拉菜单中选择作业角色。 默认情况下，在将您分配到工作项时指定的角色会显示。 如果未在对象上分配角色，则默认将显示“主角色”。 有关此设置的更多信息，请参阅文章 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. 指定要记录的时间，然后单击 **日志时间**.

### 项目、任务或问题 {#project-task-or-issue}

您可以记录项目、任务或问题的特定时间。

#### 记录时间所需的权限

要记录项目、任务或问题的小时数，您需要具有特定权限。 您可以在项目、任务或问题的两个位置登录时间：

* [“更新”选项卡](#updates-tab)
* [“小时”选项卡](#hours-tab)

##### “更新”选项卡{#updates-tab}

在您登录项目、任务或问题的“更新”选项卡的小时之前，需要满足以下条件：

* 您必须拥有工作或计划许可证。
* 您必须至少拥有项目、任务或问题的“参与”权限，才能访问“日志时间”。\
   有关授予项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* 如果要将时间直接记录到项目，Workfront管理员必须在 [!UICONTROL **工时单和小时数** ]> [!UICONTROL **首选项**].\
   有关允许用户直接将小时记录到项目的更多信息，请参阅 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### “小时”选项卡{#hours-tab}

在您登录项目、任务或问题的“小时”选项卡之前，需要满足以下条件：

* 您必须是系统管理员。

或者，您必须具备以下所有条件：

* 您必须拥有具有时间表和小时的管理访问权限的计划许可证。 有关授予对工时单和工时的管理访问权限的详细信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* 您必须至少拥有项目的Contribute权限，并且有权访问“日志时间”。 有关授予项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* 如果要直接将时间记录到项目，Workfront管理员必须在“工时单和小时数”>“首选项”下启用“直接记录项目的时间”设置。 有关允许用户直接将小时记录到项目的更多信息，请参阅 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

要记录项目、任务或问题的时间，请执行以下操作：

1. 导航到项目、任务或问题。
1. 在左侧面板中，选择 **小时**.
1. 单击 **日志时间**.

   此时将显示“日志小时数”对话框。

1. 指定以下信息：

   * **所有者：** 默认情况下，您的名称会显示在此字段中。\
      如果您正在记录其他用户的小时数，请指定其姓名。

   * **小时**:输入项目、任务或问题的小时数。
   * **小时类型**:从下拉菜单中选择一个小时类型（如果它与默认显示的类型不同）。

      根据您的系统中配置的小时类型，此处的选项可能会有所不同。 有关配置小时类型的更多信息，请参阅 [定义工时单的工时类型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **作业角色**:（视情况而定）如果您的Workfront或组管理员已 **手动将作业角色分配给小时条目** 设置，选择 **作业角色** 下拉菜单中。 默认情况下，将在您被分配到对象时指定的角色会显示。 如果未在对象上分配角色，则默认将显示主角色。 有关此设置的更多信息，请参阅文章 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. 单击 **日志小时数**.

### “摘要”面板

您可以在“摘要”面板中记录任务和问题的时间。
有关更多信息，请参阅 [概要概述](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### 展示板 {#boards}

您可以在Workfront主板上的连接卡上登录时间。 这与记录任务或问题的时间相同，而记录在卡片上的小时则保存在连接的任务或问题上。
有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### 移动设备应用程序 {#mobile-app}

您可以从Workfront移动设备应用程序中记录时间。
有关更多信息，请参阅 [Adobe Workfront for Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) 或 [Adobe Workfront for iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
