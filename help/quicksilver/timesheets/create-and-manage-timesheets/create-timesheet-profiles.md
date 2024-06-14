---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 创建、编辑和分配时间表配置文件
description: 您可以创建、编辑和分配时间表配置文件，以便为用户生成周期性时间表，而无需您的任何进一步干预。 这可以节省您的时间并确保用户之间的一致性。
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# 创建、编辑和分配时间表配置文件

您可以创建、编辑和分配时间表配置文件，以便为用户生成周期性时间表，而无需您的任何进一步干预。 这节省了您的时间，并确保用户之间的以下内容保持一致：

* 时间表时间范围
* 审批者
* 常规小时类型

有关手动创建时间表的详细信息，请参阅 [创建一次性时间表](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：标准 </p>
 <p>或</p> 
<p>当前：计划 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须对时间表具有管理访问权限。 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 创建或编辑周期性工时表

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>要在当前时间表中启用时间表配置文件更改，您必须删除现有时间表，然后生成新时间表。 有关说明，请参阅 [删除Adobe Workfront中的工时表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) 和 [手动生成工时表](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. 如果要创建或编辑在整个系统中使用的时间表配置文件，请单击 **时间表和小时数**.

   或

   如果您创建或编辑组的时间表配置文件，请单击 **组**，然后单击组的名称。

1. 单击 **周期性时间表**.
1. 要创建新的时间表配置文件，请单击 **新建配置文件**.

   或

   要编辑现有时间表配置文件，请选择要编辑的时间表配置文件，然后单击 **编辑**.

   此时会显示新的或现有的周期性时间表。


1. 在 **设置详细信息** 选项卡，键入 **名称** 和 **描述** （对于时间表配置文件）并提供以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>具有管理访问权限的组</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>如果要创建系统级时间表配置文件，请将此字段留空。</p> <p>任何可以编辑用户帐户的用户都可以将系统级时间表附加到其他用户。</p> <p>只有Workfront管理员可以编辑系统级时间表配置文件。</p> </li> 
      </ul> 
     <ul> 
      <li> <p>如果您在为所管理的组创建时间表配置文件，请在此处标识该组。</p> <p>这不会将时间表配置文件分配给组中的用户；它仅允许组的管理员修改时间表配置文件。 您将在步骤6中将该配置文件分配给用户。</p>

   <p><b>注意</b>：当组外的用户将时间表配置文件附加到其他用户时，他们将无法查看或附加此时间表配置文件。</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>创建工时表</strong> </td> 
      <td> <p> <p>指定时间表配置文件应何时生成时间表。 时间表可以设置为每周、每两周、每半年或每月自动生成。 选择您希望在一周中的哪一天生成时间表。</p>
      <p>每周工时表从生成日期开始。 例如，如果您在每个星期四创建每周时间表，则时间表上一周的第一天是星期四。</p>


   <p><b>注意</b>：Workfront始终同时创建两个时间表：第一个时间表始终包含当前日期，第二个时间表从第一时间表的时间范围结束时开始。</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>审批者</strong></p> </td> 
      <td> <p> <p>批准者是批准与时间表关联的用户的时间表的用户。 您最多可以在一个时间表上将7个用户识别为批准者。 确定多个用户对于确保审批者在某人不在办公室时可用非常有用。 当用户提交时间表进行批准时，所有批准者都会收到通知。 仅需要一个用户批准时间表才能将其批准。</p> <p>只有具有时间表管理权限的用户才能设置为批准者。 有关时间表管理权限的详细信息，请参见 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>使用下拉菜单选择时间表的批准者（如果需要批准者）。 您可以从以下选项中进行选择：</p> 
      <ul> 
      <li><strong>无</strong>：时间表不需要批准。</li> 
      <li><strong>他们的经理</strong>：这是由系统设置的默认审批者。 在这种情况下，在提交工时表供审批时，被指定为其经理的用户将审批该工时表。</li> 
      <li><strong>特定人员：</strong> 您可以按名称将特定用户指定为时间表批准者。 您在一个时间表上可以有多个批准者。 在这种情况下，在某位批准者批准该时间表后，该时间表将标记为 <strong>已关闭</strong> 并且它从所有剩余批准者的时间表批准列表中消失。</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可以编辑时间 </strong> </td> 
      <td> <p> <p>选择此选项可允许审批者在时间表上编辑小时数。

   此选项可与 **限制对所有者和管理员编辑的时间表** 设置>时间表和小时数>首选项区域中的设置。 有关更多信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">配置时间表和小时首选项</a>.

   存在以下情况：

   <ul>
      <li>当 <b>限制对所有者和管理员编辑的时间表</b> 选项已启用：</li>
      <ul><li>批准者只能批准和拒绝工时表，无论是否需要 <b>可以编辑时间</b> 是否已启用。 </li>
      <li>时间表所有者的经理只能查看其直接报告的时间表。</li></ul>
      <li>当 <b>限制对所有者和管理员编辑的时间表</b> 选项已禁用：</li>
    <ul><li>当 <b>可以编辑时间</b> 启用，审批者可以提交、重新打开或关闭时间表，并可以编辑时间。</li>
      <li>当 <b>可以编辑时间</b> 已禁用，审批者无法提交、重新打开或关闭时间表，也无法编辑时间。 批准者只能批准或拒绝时间表。 </li>
      <li>时间表所有者的经理可以提交、撤消、重新打开和编辑其直接下属的时间表。</li></ul>
      </ul>

   <p>

   <b>注意</b>：提交时间表以供审批后，您无法再编辑小时数。 要将已提交工时表返回到可编辑状态，请撤消该工时表或让批准者拒绝该工时表。 有关更多信息，请参阅 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交工时表以供审批</a> 和<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准工时表</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>可用小时类型</strong> </td> 
      <td><p>此设置仅引用常规小时类型，而不引用特定于项目的小时类型。 </p>
      <p>默认情况下，用户会在时间表上看到所有常规小时数。 但是，如果贵组织希望仅显示特定用户集的常规小时数，则可以通过在此字段内选择时间表配置文件中的常规小时数，选择需要在时间表上查看的常规小时数。 如果要禁用所有常规小时，请取消选择所有小时类型以生成不带常规小时分区的时间表。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以选择在时间表中隐藏“加班”框。 默认禁用此选项。</td> 
     </tr> 
    </tbody> 
    </table>

1. 单击 **分配人员** 选项卡，将时间表配置文件与特定用户、组或(如果您是Workfront管理员)团队关联。 开始键入用户、组或团队的名称，然后当它出现在下拉列表中时单击它。

   如果您是组管理员，您可以将时间表配置文件分配给您管理的组，但不能分配给团队。 有关更多信息，请参阅 [组管理员分配时间表配置文件的限制](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) 本文章中。

   >[!NOTE]
   >
   >* 您还可以通过编辑用户配置文件将用户与时间表配置文件关联。 有关更多信息，请参阅 [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* 添加组时，“分配人员”选项卡上只显示组名，不显示组成员列表。 如果要查看此处列出的组成员，请单击保存更改，然后单击刚刚创建的时间表配置文件的名称。
   >* 完成这些步骤后，时间表配置文件仅为在当前期间没有现有时间表的已分配用户或组成员生成时间表。

1. 单击 **保存更改**.

   时间表用户档案首次生成时间表时，会为每个用户创建2个时间表。 之后，每次生成新时间表时，都会为每个用户创建时间表。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 组管理员分配时间表配置文件的限制 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

如果您是组管理员，并且访问级别中禁用了管理访问选项时间表和小时数，则可以创建时间表配置文件，但只能将其分配给：

* 您管理的组
* 您有权编辑的属于您管理之群组的个人用户

对于这些组和用户，您将无法访问时间表配置文件生成的时间表。

此外，如果在访问级别中还禁用了“用户管理员（组用户）”选项，则可以将时间表配置文件分配给您管理的组，但仅影响您有权编辑的组中的用户。 如果组包含您无权编辑的用户，则不会将时间表配置文件分配给该组的其他成员。

有关访问级别中的时间表和小时选项的信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

有关访问级别中的用户管理员（组用户）选项的信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 多个周期性工时表配置信息

您的组织可以有多个时间表配置文件，如果存在：

* 不同用户集的独特付薪期间
* 不同用户集的独特审批者
* 不同用户集的独特常规小时要求

一个用户一次不能与多个时间表配置文件关联。 
