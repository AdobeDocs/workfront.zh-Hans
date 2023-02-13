---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交时间表以供审批
description: 提交工时单以供审批，让您的经理可以查看您的工作时间。 批准者可以验证所记录的所有时间是否已分配到正确的区域，以及该时间段是否已记录足够的小时数。
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 提交时间表以供审批

提交工时单以供审批，让您的经理可以查看您的工作时间。 批准者可以验证所记录的所有时间是否已分配到正确的区域，以及该时间段是否已记录足够的小时数。

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
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对任务和问题的访问权限或更高权限</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务和问题的权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 提交时间表以供审批

* [提交时间表以供审批](#submit-a-timesheet-for-approval)
* [查看已提交时间表的状态](#view-the-status-of-a-submitted-timesheet)

### 提交时间表以供审批

设置时间表审批者后（如一节中所述） [指定时间表批准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 在文章中 [批准时间表](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md))、 **关闭** 按钮将时间表底部的 **提交以供审批** 按钮。

要提交时间表以供审批，请执行以下操作：

1. 转到已配置为具有审批者的时间表。
1. 日志时间，如 [日志时间](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 单击 **提交以供审批** 启动工时单审批流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   的 **提交以供审批** 按钮替换为 **批准**, **拒绝**&#x200B;和 **召回** 按钮。 时间表的状态将更改为 **已提交**.

   提交工时单以供审批后，审批者会在 **批准** 区域 **主页** 页面。 可能会发生以下情况：

   * 如果他们同意， **召回** 按钮更改为 **重新打开** 和时间表状态更新为 **打开**.
   * 如果他们拒绝， **提交以供审批** 按钮替换 **召回** 按钮和时间表状态更新为 **被拒绝**.

1. （可选）单击 **召回** 如果您需要重新打开时间表并更新您的时间。 有关信息，请参阅 [调回工时单](#recall-a-timesheet) 章节。

### 查看已提交时间表的状态 {#view-the-status-of-a-submitted-timesheet}

在提交时间表后，您可以查看该时间表的状态。

如果Workfront管理员已启用“用户工时单审批”和“用户工时单拒绝”事件处理程序，则在工时单被批准或拒绝后，系统会通知您。 有关启用事件通知的信息，请参阅 [事件通知在Adobe Workfront中可用](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如果没有这些通知，您可以在Workfront的“时间表”区域了解提交的时间表的状态。

要查看时间表的状态，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击 **工时单**. 的 **全部** 筛选器是默认选中的。

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
   >   
   >   
   >   * [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （视情况而定）如果您选择 **我的工时表**，请确保 **标准** 视图，并注意 **状态** 列。

   工时单可能具有以下状态：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">打开</td> 
      <td> <p>您的时间表当前处于打开状态，您可以记录时间。 </p> <p>显示状态为“打开”的已回调时间表。 有关信息，请参阅 <a href="#recall-a-timesheet" class="MCXref xref">调回工时单</a> 章节。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您提交了时间表以供审批，但尚未批准。 您可能会记得已提交的时间表，以继续编辑它。 有关信息，请参阅 <a href="#recall-a-timesheet" class="MCXref xref">调回工时单</a> 章节。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已关闭</td> 
      <td> <p>存在以下情形：</p> 
       <ul> 
        <li> <p>如果时间表没有审批者，则您保存了您的时间并将其关闭。</p> </li> 
        <li> <p>如果时间表有审批者，则您已经将其提交以供审批，并且已获得批准。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">被拒绝</td> 
      <td>您提交了时间表以供审批，审批者拒绝了它。</td> 
     </tr> 
    </tbody> 
   </table>

## 调回工时单 {#recall-a-timesheet}

您可以回顾已提交审批的时间表。 只有未获得批准的时间表才能被召回。

要召回时间表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **工时单**.
1. 单击 **我的工时表** 或选择 **我的工时表** 从 **过滤器** ![](assets/filter-nwepng.png) 下拉菜单。
1. 单击状态为 **已提交**.
1. 单击 **召回**.

   时间表将再次变为可编辑状态，其状态将更改为 **打开**.
