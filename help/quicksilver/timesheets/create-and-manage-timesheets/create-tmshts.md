---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 创建一次性工时单
description: 如果您希望的时间表不是重复的，可以手动创建一次性使用的时间表。 当到达时间表的结束日期并且需要更多的时间表时，您必须创建新的时间表。
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 创建一次性工时单

如果您希望的时间表不是重复的，可以手动创建一次性使用的时间表。 当到达时间表的结束日期并且需要更多的时间表时，您必须创建新的时间表。

有关创建工时单配置文件以为用户生成定期工时单而无需您进一步干预（推荐）的信息，请参阅 [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* 不能为组创建一次性工时单。

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 创建一次性工时单时，您不能选择要包含在工时单中的特定一般工时类型。 系统中激活的所有常规小时类型都以手动创建的时间表显示。
>
>  如果只想选择在工时单中显示的某些一般工时类型，请使用工时单配置文件。 有关时间表配置文件的详细信息，请参阅 [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>您必须对工时单具有管理访问权限。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p><b> 注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建一次性工时单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **工时单**. 的 **全部** 筛选器是默认选中的。 此时会显示您有权查看的所有时间表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）执行下列操作之一以更新工时单列表中的过滤器：

   * 选择 **我的时间表批准** ，以仅查看您批准的时间表

      或

      选择 **我的工时表** 以仅查看您的工时单。

      这会将“我的时间表审批”或“我的时间表”过滤器应用于时间表列表。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击过滤器图标 ![](assets/filter-nwepng.png) 应用其他过滤器，或创建新过滤器。 有关创建或更新过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的“列表控件”或“布局模板”中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   > 
   >   * [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 键入关键字并搜索特定时间表。 例如，您可以搜索所有者名称的时间表时间范围。

1. （可选）单击 **查看** ![](assets/view-icon.png) 或 **分组** ![](assets/grouping.png) 图标来应用其他视图或分组，或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 单击 **新时间表** 时间表列表顶部。

   指定以下信息：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>为以下人员创建工时表</strong> </td> 
      <td>开始输入用户、职务角色或您为其创建工时单的团队的名称，并在列表中显示时单击这些名称。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>开始日期</strong> </td> 
      <td>这是时间表的开始日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>结束日期</strong> </td> 
      <td> 这是时间表的结束日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>审批者</strong> </td> 
      <td>批准者是为与时间表关联的用户批准时间表的用户。 只能将具有时间表管理权限的用户设置为批准者。 有关工时单管理权限的详细信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.<br>开始输入时间表批准者的名称，并在列表中显示时单击这些名称。<br>一个时间表上可以有多个批准者。 在这种情况下，在其中一个批准者批准时间表后，时间表将被标记为 <strong>已关闭</strong> 然后它会从所有剩余批准者的时间表批准列表中消失。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>可以编辑时间</strong> </td>

   <td> <p>如果要允许批准者编辑工时单上的工时，请选择此选项。</p>

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

   提交工时单以供审批后，您便无法再编辑工时。 要将提交的时间表返回到可编辑状态，请回调时间表或让审批者拒绝时间表。 有关更多信息，请参阅 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交时间表以供审批</a> 和 <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准时间表</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以选择隐藏工时单上的“超时”框。 默认情况下，此选项处于禁用状态。</td> 
      </tr> 
      </tbody> 
   </table>

1. 单击 **创建工时单**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 当任务和问题显示在用户的工时单上时

如果任务或问题满足以下任一条件，则分配给用户的任务或问题会自动显示在用户的时间表上：

* 用户已记录任务或问题的小时数
* 任务或问题的计划日期在时间表日期之内
* 任务或问题具有实际开始日期（任务或问题状态为“进行中”）
* 任务或问题被固定到时间表
* 计划完成日期在时间表的日期范围内，并且状态为“进行中”

如果 **预填充时间表……** 首选项（位于“工时单”和“工时”首选项中）被取消选中，此时工时表会显示状态为“进行中”的问题和任务。 有关工时单和小时首选项的详细信息，请参阅 [配置工时单和工时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
