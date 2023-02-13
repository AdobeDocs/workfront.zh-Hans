---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 创建、编辑和分配工时单配置文件
description: 您可以创建、编辑和分配工时单配置文件，这些工时单为用户生成定期工时单，无需您进一步干预。 这样可节省您的时间，并确保以下内容在用户之间保持一致 — 编辑我。
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# 创建、编辑和分配工时单配置文件

您可以创建、编辑和分配工时单配置文件，这些工时单为用户生成定期工时单，无需您进一步干预。 这样可节省您的时间，并确保用户之间的以下内容保持一致：

* 时间表时间范围
* 审批者
* 一般小时类型

有关手动创建工时单的详细信息，请参阅 [创建一次性工时单](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须对工时单具有管理访问权限。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用户对特定区域的管理访问权限</a>.</p>  <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建或编辑工时单配置文件

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>要在当前工时单中启用工时单配置文件更改，必须删除现有工时单，然后生成新工时单。 有关说明，请参阅 [删除Adobe Workfront中的工时单](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) 和 [手动生成工时单](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 如果要创建或编辑时间表配置文件以供在整个系统中使用，请单击 **工时单和小时数**.

   或

   如果创建或编辑组的时间表配置文件，请单击 **群组**，然后单击群组的名称。

1. 单击 **时间表配置文件**.
1. 要创建新的时间表配置文件，请单击 **新建用户档案**.

   或

   要编辑现有工时单配置文件，请选择要编辑的工时单配置文件，然后单击 **编辑**.

   此时会显示新的或现有的时间表配置文件。


1. 在 **设置详细信息** 选项卡，键入 **名称** 和 **描述** 用于工时单配置文件并提供以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>有着管理访问权限的组</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>如果要创建系统级时间表配置文件，请将此字段留空。</p> <p>任何能够编辑用户帐户的用户都可以将系统级别的时间表附加到其他用户。</p> <p>只有Workfront管理员才能编辑系统级别的时间表配置文件。</p> </li> 
      </ul> 
     <ul> 
      <li> <p>如果要为您管理的组创建时间表配置文件，请在此处标识该组。</p> <p>这不会将工时单配置文件分配给组中的用户；它仅允许组的管理员修改工时单配置文件。 在步骤6中，您会将用户档案分配给用户。</p> <p><b>注释</b>

   当组外的用户将工时单配置文件附加到其他用户时，他们将无法查看或附加此工时单配置文件。</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>创建时间表</strong> </td> 
      <td> <p> <p>指定时间表配置文件应何时生成时间表。 时间表可设置为每周、每两周、每半月或每月自动生成。 选择希望生产工时单的一周中的某一天。</p> <p><b>注释</b>

   如果将时间表配置文件配置为在星期五创建时间表，则用户无法记录当周的星期五、星期六和星期日的时间表。</p> <p>Workfront始终一次创建两个工时单：第一个时间表始终包括当前日期，第二个时间表在第一个时间表的时间范围结束时开始。</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>审批者</strong></p> </td> 
      <td> <p> <p>批准者是为与时间表关联的用户批准时间表的用户。 您最多可以在时间表上标识7个用户作为批准者。 识别多个用户对于确保在某人不在办公室时有审批者可用非常有用。 当用户提交时间表以供审批时，所有审批者都会收到通知。 只有一个用户需要批准时间表才能获得批准。</p> <p>只能将具有时间表管理权限的用户设置为批准者。 有关工时单管理权限的详细信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>使用下拉菜单选择工时单的审批者（如果需要审批者）。 您可以从以下选项中进行选择：</p> 
      <ul> 
      <li><strong>无</strong>:时间表不需要获得批准。</li> 
      <li><strong>他们的经理</strong>:这是系统设置的默认审批者。 在这种情况下，指定为经理的用户在提交时间表以供审批时批准该时间表。</li> 
      <li><strong>特定人员：</strong> 您可以按名称指定特定用户作为时间表批准者。 一个时间表上可以有多个批准者。 在这种情况下，在其中一个批准者批准时间表后，时间表将被标记为 <strong>已关闭</strong> 然后它会从所有剩余批准者的时间表批准列表中消失。</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可以编辑时间 </strong> </td> 
      <td> <p> <p>选择此选项以允许审批者编辑工时单上的工时。

   此选项与 **将工时单编辑限制为所有者和管理员** 在“设置”>“时间表和小时数”>“首选项”区域中进行设置。 有关更多信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">配置工时单和工时首选项</a>.

   存在以下情形：

   <ul>
      <li>当 <b>将工时单编辑限制为所有者和管理员</b> 选项：</li>
      <ul><li>批准者只能批准和拒绝工时单，而不管 <b>可以编辑时间</b> 是否启用。 </li>
      <li>工时单所有者的经理只能查看其直接报表的工时单。</li></ul>
      <li>当 <b>将工时单编辑限制为所有者和管理员</b> 选项处于禁用状态：</li>
    <ul><li>当 <b>可以编辑时间</b> 启用后，审批者可以提交、重新打开或关闭时间表并编辑时间。</li>
      <li>当 <b>可以编辑时间</b> 禁用时，批准者无法提交、重新打开或关闭时间表，也无法编辑时间。 批准者只能批准或拒绝时间表。 </li>
      <li>时间表所有者的经理可以提交、召回、重新打开和编辑其直接报告的时间表。</li></ul>
      </ul>

   <p><b>注释</b>

   提交工时单以供审批后，您便无法再编辑工时。 要将提交的时间表返回到可编辑状态，请回调时间表或让审批者拒绝时间表。 有关更多信息，请参阅 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交时间表以供审批</a> 和<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准时间表</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>可用小时类型</strong> </td> 
      <td>默认情况下，用户会在时间表上看到所有一般小时数。 但是，如果贵组织只希望为一组特定用户显示特定的一般小时数，则可以通过在此字段中的时间表配置文件中选择这些用户，来选择他们在其时间表中需要查看的一般小时数。 如果要禁用所有一般工时，请取消选择所有工时类型以生成不带一般工时部分的工时单。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以选择在工时单中隐藏“超时”框。 默认情况下，此选项处于禁用状态。</td> 
     </tr> 
    </tbody> 
    </table>

1. 单击 **分配人员** 选项卡，将时间表配置文件与特定用户、组或(如果您是Workfront管理员)团队关联。 开始键入用户、组或团队的名称，然后在下拉列表中显示该名称时单击该名称。

   如果您是组管理员，则可以将时间表配置文件分配给您管理的组，但不能分配给团队。 有关更多信息，请参阅 [组管理员分配时间表配置文件的限制](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) 在本文中。

   >[!NOTE]
   >
   >* 您还可以通过编辑用户配置文件将用户与时间表配置文件关联。 有关更多信息，请参阅 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* 添加群组时，“分配人员”选项卡中只显示群组名称，而不显示群组成员列表。 如果要查看此处列出的组成员，请单击“保存更改”，然后单击刚刚创建的时间表配置文件的名称。
   >* 完成这些步骤后，时间表配置文件将仅为分配的用户或组成员生成时间表，这些用户或组成员没有当前时段的现有时间表。


1. 单击 **保存更改**.

   工时单配置文件首次生成工时单时，为每个用户创建2个工时单。 之后，每次生成新工时单时，每个用户都会创建工时单。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 组管理员分配时间表配置文件的限制 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

如果您是组管理员，并且在访问级别中禁用了管理访问选项工时单和工时，则可以创建工时单配置文件，但只能将其分配给：

* 您管理的组
* 您有权编辑的个人用户，其所在的组由您管理

对于这些组和用户，您将无权访问时间表配置文件生成的时间表。

此外，如果在访问级别中也禁用了“用户管理员（组用户）”选项，则可以将时间表配置文件分配给您管理的组，但它只影响您有权编辑的组中的用户。 如果组中包含您无权编辑的用户，则不会为他们分配时间表配置文件以及组的其余部分。

有关访问级别中的时间表和小时选项的信息，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

有关访问级别中的用户管理员（群组用户）选项的信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 多个定期工时单配置文件

如果存在以下情况，则您组织可以拥有多个时间表配置文件：

* 不同用户集的唯一支付期
* 不同用户集的唯一批准者
* 不同用户集的独特一般小时数要求

一个用户一次不能与多个时间表配置文件关联。 
