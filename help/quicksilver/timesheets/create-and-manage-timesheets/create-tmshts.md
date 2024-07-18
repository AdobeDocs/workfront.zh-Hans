---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 创建一次性时间表
description: 如果您希望某个时间表不重复，可以手动创建一次性时间表。 在到达时间表结束日期且您需要更多时间表时，您必须创建新时间表。
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# 创建一次性时间表

如果您希望某个时间表不重复，可以手动创建一次性时间表。 在到达时间表结束日期且您需要更多时间表时，您必须创建新时间表。

有关创建时间表配置文件以生成用户周期性时间表而不需要您进一步干预的信息（推荐），请参阅[创建、编辑和分配时间表配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

>[!NOTE]
>
>* 无法为组创建一次性时间表。
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 在创建一次性时间表时，您无法选择要包含在时间表中的特定常规小时类型。 在您系统中激活的所有常规小时类型都会显示在手动创建的时间表中。
>
>  如果您只想选择在时间表中显示的某些常规小时类型，请使用时间表配置文件。 有关时间表配置文件的详细信息，请参阅[创建、编辑和分配时间表配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。
>

## 访问要求

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须对时间表具有管理访问权限。 </p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>。</p> <p><b> 注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建一次性时间表

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**时间表**。 默认情况下已选择&#x200B;**所有**&#x200B;筛选器。 这会显示您有权查看的所有时间表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）执行以下操作之一以更新时间表列表中的过滤器：

   * 选择页面右上角的&#x200B;**我的工时表批准**&#x200B;以仅查看您批准的时间表

     或

     选择&#x200B;**我的时间表**&#x200B;以仅查看您的时间表。

     这会将我的时间表批准或我的时间表过滤器应用到时间表列表。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击“筛选器”图标![](assets/filter-nwepng.png)以应用其他筛选器，或创建新筛选器。 有关创建或更新筛选器的信息，请参阅[在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的列表控件或布局模板中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   > 
   >   * [使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （可选）单击&#x200B;**搜索**&#x200B;图标![](assets/search-icon.png)以键入关键字并搜索特定时间表。 例如，您可以搜索所有者名称的时间表时间范围。

1. （可选）单击&#x200B;**视图** ![](assets/view-icon.png)或&#x200B;**分组** ![](assets/grouping.png)图标以应用不同的视图或分组或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 单击时间表列表顶部的&#x200B;**新建时间表**。

   指定以下信息：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>为</strong>创建工时表 </td> 
      <td>开始输入用户、工作角色或要为其创建时间表的团队的名称，并在它们在列表中显示时单击它们。</td> 
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
      <td>批准者是批准与时间表关联的用户的时间表的用户。 只有具有时间表管理权限的用户才能设置为批准者。 有关时间表管理权限的详细信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>。<br>开始输入时间表批准者的姓名，并在他们出现在列表中时单击他们。<br>您在一个时间表上可以有多个批准者。 在这种情况下，在某位批准者批准该时间表后，该时间表将标记为<strong>已关闭</strong>，并从所有剩余批准者的时间表批准列表中消失。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>可以编辑时间</strong> </td>

   <td> <p>如果要允许批准者在时间表上编辑小时数，请选择此选项。</p>

   此选项与“设置”>“时间表和小时数”>“首选项”区域中的&#x200B;**限制所有者和管理员编辑时间表**&#x200B;设置一起使用。 有关详细信息，请参阅<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">配置工时表和小时首选项</a>。

   存在以下情况：

   <ul>
      <li>启用<b>限制对所有者和管理员编辑时间表</b>选项时：</li>
   <ul><li>批准者只能批准和拒绝时间表，无论<b>可以编辑时间</b>是否启用。 </li>
   <li>时间表所有者的经理只能查看其直接报告的时间表。</li></ul>
   <li>禁用<b>限制对所有者和管理员编辑工时表</b>选项时：</li>
   <ul><li>启用<b>可以编辑时间</b>后，审批者可以提交、重新打开或关闭时间表并可以编辑时间。</li>
   <li>禁用<b>可以编辑时间</b>后，审批者无法提交、重新打开或关闭时间表，也无法编辑时间。 批准者只能批准或拒绝时间表。 </li>
   <li>时间表所有者的经理可以提交、撤消、重新打开和编辑其直接下属的时间表。</li></ul>
   </ul>

   <p><b>注释</b>

   提交时间表以供审批后，您无法再编辑小时数。 要将已提交工时表返回到可编辑状态，请撤消该工时表或让批准者拒绝该工时表。 有关详细信息，请参阅<a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交时间表以供审批</a>和<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准时间表</a>。</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以选择在时间表上隐藏“加班”框。 默认禁用此选项。</td> 
      </tr> 
      </tbody> 
   </table>

1. 单击&#x200B;**创建时间表**。

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 任务和问题出现在用户时间表上的时间

如果任务或问题满足以下任一条件，则分配给用户的任务或问题会自动显示在用户的时间表中：

* 用户已记录任务或问题的小时数
* 任务或问题的计划日期在时间表的日期内
* 任务或问题具有实际开始日期（任务或问题状态为“进行中”）
* 任务或问题已固定到时间表
* 计划完成日期在时间表的日期范围内，状态为“进行中”

如果未选中&#x200B;**使用……**&#x200B;首选项预填充时间表（位于时间表和小时首选项中），则时间表显示状态为“进行中”的问题和任务。 有关时间表和小时首选项的详细信息，请参阅[配置时间表和小时首选项](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。
