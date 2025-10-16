---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 创建、编辑和分配时间表配置文件
description: 您可以创建、编辑和分配时间表配置文件，以便为用户生成周期性时间表，而无需您的任何进一步干预。 这可以节省您的时间并确保用户之间的一致性。
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 2%

---

# 创建、编辑和分配时间表配置文件

<!--Audited: 06/2025-->

您可以创建、编辑和分配时间表配置文件，以便为用户生成周期性时间表，而无需您的任何进一步干预。 这节省了您的时间，并确保用户之间的以下内容保持一致：

* 时间表时间范围
* 审批者
* 常规小时类型

有关手动创建时间表的详细信息，请参阅[创建一次性时间表](../../timesheets/create-and-manage-timesheets/create-tmshts.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>对工时表的管理访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建或编辑周期性工时表

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>要在当前时间表中启用时间表配置文件更改，您必须在更改时间表配置文件之前删除现有时间表，然后生成新时间表。 有关说明，请参阅[删除Adobe Workfront中的时间表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)和[手动生成时间表](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)。

{{step-1-to-setup}}

1. 如果您创建或编辑在整个系统中使用的时间表配置文件，请单击&#x200B;**时间表和小时数**。

   或

   如果您创建或编辑某个组的时间表配置文件，请单击&#x200B;**组**，然后单击该组的名称。

1. 单击&#x200B;**周期性工时表**。
1. 要创建时间表配置文件，请单击&#x200B;**新建配置文件**。

   或

   要编辑现有时间表配置文件，请选择要编辑的时间表配置文件，然后单击&#x200B;**编辑**。

   此时会显示新的或现有的时间表配置文件页面。

1. 更新以下信息：

   * **名称**：为时间表配置文件添加名称。 它可以是一个团队或组的名称，其人员共享的时间表相同。 这是必填字段。
   * **描述**：添加有关时间表配置文件的更多信息。
   * **具有管理访问权限的组**：如果您正在创建系统级时间表配置文件，请将此字段留空。

     任何可以编辑用户帐户的用户都可以将系统级时间表附加到其他用户。

     只有Workfront管理员可以编辑系统级时间表配置文件。

     如果您在为所管理的组创建时间表配置文件，请在此处标识该组。

     这不会将时间表配置文件分配给组中的用户；它仅允许组的管理员修改时间表配置文件。 您将在步骤6中将该配置文件分配给用户。

     >[!NOTE]
     >
     >当组外的用户将时间表配置文件附加到其他用户时，他们将无法查看或附加此时间表配置文件。

   * **创建时间表**：指定时间表配置文件应何时生成时间表。 时间表可以设置为每周、每两周、每半年或每月自动生成。 选择您希望在一周中的哪一天生成时间表。

     每周工时表从生成日期开始。 例如，如果您在每个星期四创建每周时间表，则时间表上一周的第一天是星期四。

     >[!NOTE]
     >
     >Workfront始终同时创建两个时间表：第一个时间表始终包含当前日期，第二个时间表从第一时间表的时间范围结束时开始。

   * **批准者**：批准者是批准与时间表关联的用户的时间表的用户。 您最多可以在一个时间表上将7个用户识别为批准者。 确定多个用户对于确保审批者在某人不在办公室时可用非常有用。 当用户提交时间表进行批准时，所有批准者都会收到通知。 仅需要一个用户批准时间表才能将其批准。

     只有具有时间表管理权限的用户才能设置为批准者。 有关时间表管理权限的详细信息，请参阅[授予用户对特定区域的管理访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

     使用下拉菜单选择时间表的批准者（如果需要批准者）。 您可以从下列选项中进行选择：

      * **无**：不需要批准时间表。
      * **他们的经理**：这是系统设置的默认审批者。 在这种情况下，在提交工时表供审批时，被指定为其经理的用户将审批该工时表。
      * **特定人员**：您可以按姓名指定特定用户作为时间表批准者。 您在一个时间表上可以有多个批准者。 在这种情况下，在某位批准者批准该时间表后，该时间表将标记为&#x200B;**已关闭**，并从所有剩余批准者的时间表批准列表中消失。

   * **可以编辑时间**：选择此选项可允许批准者在时间表上编辑小时数。

     此选项与“设置”>“时间表和小时数”>“首选项”区域中的&#x200B;**限制所有者和管理员编辑时间表**&#x200B;设置一起使用。 有关详细信息，请参阅[配置工时表和小时首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

     存在以下情况：

     启用&#x200B;**限制对所有者和管理员编辑时间表**&#x200B;选项时：

      * 批准者只能批准和拒绝时间表，无论是否启用可编辑时间。
      * 时间表所有者的经理只能查看其直接报告的时间表。

     禁用&#x200B;**限制对所有者和管理员编辑工时表**&#x200B;选项时：

      * 启用&#x200B;**可以编辑时间**&#x200B;后，审批者可以提交、重新打开或关闭时间表并编辑时间。
      * 禁用&#x200B;**可以编辑时间**&#x200B;后，审批者无法提交、重新打开或关闭时间表，也无法编辑时间。 批准者只能批准或拒绝时间表。
      * 时间表所有者的经理可以提交、撤消、重新打开和编辑其直接下属的时间表。

     >[!NOTE]
     >
     >提交时间表以供审批后，您无法再编辑小时数。 要将已提交工时表返回到可编辑状态，请撤消该工时表或让批准者拒绝该工时表。 有关详细信息，请参阅[提交时间表以供审批](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)和[批准时间表](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)。

   * **加班**：您可以选择在时间表中隐藏“加班”框。 默认禁用此选项。
   * **可用小时类型**：此设置仅引用常规小时类型，而不引用项目特定的小时类型。

     默认情况下，用户会在时间表上看到所有常规小时数。 但是，如果贵组织希望仅显示特定用户集的常规小时数，则可以通过在此字段内选择时间表配置文件中的常规小时数，选择需要在时间表上查看的常规小时数。 如果要禁用所有常规小时，请取消选择所有小时类型以生成不带常规小时分区的时间表。

   * **提醒通知**：添加提醒通知。 Workfront将向用户发送提醒，要求他们完成或批准时间表。 您必须先创建提醒通知，然后才能将其与时间表配置文件关联。

1. 要将时间表配置文件与特定用户、组或(如果您是Workfront管理员)团队关联，请滚动到页面底部并找到&#x200B;**分配人员**&#x200B;部分。

   开始键入用户、组或团队的名称，然后当它出现在下拉列表中时单击它。

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   如果您是组管理员，您可以将时间表配置文件分配给您管理的组，但不能分配给团队。 有关详细信息，请参阅本文中的[组管理员分配时间表配置文件](#limitations-for-a-group-administrator-assigning-a-timesheet-profile)的限制。

   >[!NOTE]
   >
   >* 您还可以通过编辑用户配置文件将用户与时间表配置文件关联。 有关详细信息，请参阅[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。
   >* 添加组时，“分配人员”选项卡上只显示组名，不显示组成员列表。 如果要查看此处列出的组成员，请单击保存更改，然后单击刚刚创建的时间表配置文件的名称。
   >* 完成这些步骤后，时间表配置文件仅为在当前期间没有现有时间表的已分配用户或组成员生成时间表。

1. 单击&#x200B;**保存**。

1. 在时间表配置文件列表顶部，单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**生成时间表**。

   屏幕底部会显示一条确认消息，确认已成功生成时间表。 新时间表是根据您创建的新用户档案生成的。

   有关详细信息，请参阅[手动生成时间表](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)。

   时间表用户档案首次生成时间表时，会为每个用户创建两个时间表，分别针对包含当前时间以及下一个时间范围的时间表。

   之后，每次生成新时间表时，都会为每个用户创建一个时间表。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 组管理员分配时间表配置文件的限制 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

如果您是组管理员，并且访问级别中禁用了管理访问选项时间表和小时数，则可以创建时间表配置文件，但只能将其分配给：

* 您管理的组
* 您有权编辑的属于您管理之群组的个人用户

对于这些组和用户，您将无法访问时间表配置文件生成的时间表。

此外，如果在访问级别中还禁用了“用户管理员（组用户）”选项，则可以将时间表配置文件分配给您管理的组，但仅影响您有权编辑的组中的用户。 如果组包含您无权编辑的用户，则不会将时间表配置文件分配给该组的其他成员。

有关访问级别中的时间表和小时选项的信息，请参阅[授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

有关访问级别中的用户管理员（组用户）选项的信息，请参阅[授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

## 多个周期性工时表配置信息

您的组织可以有多个时间表配置文件，如果存在：

* 不同用户集的独特付薪期间
* 不同用户集的独特审批者
* 不同用户集的独特常规小时要求

一个用户一次不能与多个时间表配置文件关联。

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->