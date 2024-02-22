---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交工时表以供审批
description: 通过提交时间表以供审批，您的经理可以查看您的工作时间。 批准者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# 提交工时表以供审批

通过提交时间表以供审批，您的经理可以查看您的工作时间。 批准者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。

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
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对任务和问题的访问权限或更高</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务或问题的权限或更高</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 提交工时表以供审批

* [提交工时表以供审批](#submit-a-timesheet-for-approval)
* [查看已提交工时表的状态](#view-the-status-of-a-submitted-timesheet)

### 提交工时表以供审批

设置时间表批准者后（如一节所述） [指定时间表批准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 在文章中 [批准工时表](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md))，则 **关闭** 时间表底部的按钮将更改为 **提交以供审批** 按钮。

要提交工时表以供审批，请执行以下操作：

1. 转到已配置为拥有审批者的时间表。
1. 记录时间，如中所述 [记录时间](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 单击 **提交以供审批** 以启动时间表批准流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   此 **提交以供审批** 按钮已替换为 **批准**， **拒绝**、和 **撤消** 按钮。 工时表的状态更改为 **已提交**.

   在提交您的时间表以供审批时，审批者会看到 **审批** 区域 **主页** 页面。 可能会出现以下情况：

   * 如果他们批准， **撤消** 按钮更改为 **重新打开** 和工时表状态更新到 **打开**.
   * 如果他们拒绝， **提交以供审批** 按钮替换 **撤消** 按钮和工时表状态更新到 **被拒绝**.

1. （可选）单击 **撤消** 如果您需要重新打开时间表并更新您的时间。 有关信息，请参见 [撤回时间表](#recall-a-timesheet) 部分。

### 查看已提交工时表的状态 {#view-the-status-of-a-submitted-timesheet}

提交时间表后，您可以查看时间表状态。

如果Workfront管理员启用了“批准用户时间表”和“拒绝用户时间表事件处理程序”，则在批准或拒绝时间表后会通知您。 有关启用事件通知的信息，请参阅 [事件通知类型](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如果没有这些通知，您可以在Workfront的“时间表”区域中了解已提交时间表的状态。

要查看时间表的状态，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。
1. 单击 **时间表**. 此 **全部** 默认情况下，过滤器处于选中状态。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）执行以下操作之一以更新时间表列表中的过滤器：

   * 选择 **我的工时表批准** ，以仅查看您批准的时间表

     或

     选择 **我的工时表** 以仅查看您的时间表。

     这会将我的时间表批准或我的时间表过滤器应用到时间表列表。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击过滤器图标 ![](assets/filter-nwepng.png) 以应用其他过滤器，或创建一个新过滤器。 有关创建或更新过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的列表控件或布局模板中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   >
   >   
   >   
   >   * [使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （视情况而定）如果您选择 **我的工时表**，确保 **标准** 已应用视图，并注意 **状态** 列。

   时间表可能具有以下状态：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">未完成</td> 
      <td> <p>您的时间表当前处于打开状态，您可以记录时间。 </p> <p>撤回的工时表显示为“未结”状态。 有关信息，请参见 <a href="#recall-a-timesheet" class="MCXref xref">撤回时间表</a> 部分。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您已提交时间表以供审批，但尚未获得批准。 您可以撤回已提交的时间表以继续编辑它。 有关信息，请参见 <a href="#recall-a-timesheet" class="MCXref xref">撤回时间表</a> 部分。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已关闭</td> 
      <td> <p>存在以下情况：</p> 
       <ul> 
        <li> <p>如果时间表没有审批者，则您节省了时间并将其关闭。</p> </li> 
        <li> <p>如果时间表有批准者，则表示您已提交该时间表进行批准并已获得批准。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">被拒绝</td> 
      <td>您已提交时间表进行审批，批准者拒绝了它。</td> 
     </tr> 
    </tbody> 
   </table>

## 撤回时间表 {#recall-a-timesheet}

您可以撤消已提交供审批的时间表。 只能撤消未获批准的工时表。

要撤消时间表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 **时间表**.
1. 单击 **我的工时表** 或选择 **我的工时表** 从 **筛选** ![](assets/filter-nwepng.png) 下拉菜单。
1. 单击状态为“ ”的工时表的时间范围 **已提交**.
1. 单击 **撤消**.

   该时间表将再次变为可编辑，并且其状态将更改为 **打开**.
