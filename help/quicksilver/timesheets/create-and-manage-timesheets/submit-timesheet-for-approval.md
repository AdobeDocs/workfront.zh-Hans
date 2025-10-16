---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交工时表以供审批
description: 通过提交时间表以供审批，您的经理可以查看您的工作时间。 批准者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# 提交工时表以供审批

<!--Audited: 8/2024-->

通过提交时间表以供审批，您的经理可以查看您的工作时间。 批准者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>浅色或更高 </p>
   <p>审核或更高 </p>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看或更高权限的任务和问题 </p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>查看时间表或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 提交工时表以供审批

* [提交工时表以供审批](#submit-a-timesheet-for-approval)
* [查看已提交工时表的状态](#view-the-status-of-a-submitted-timesheet)

### 提交工时表以供审批

设置时间表批准者后（如文章[批准时间表](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver)中的[指定时间表批准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)部分中所述），时间表底部的&#x200B;**关闭**&#x200B;按钮更改为&#x200B;**提交以供批准**&#x200B;按钮。

要提交工时表以供审批，请执行以下操作：

1. 转到已配置为拥有审批者的时间表。
1. 记录时间，如[记录时间](../../timesheets/create-and-manage-timesheets/log-time.md)中所述。
1. 单击&#x200B;**提交以供审批**&#x200B;以启动时间表审批流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   **提交以供审批**&#x200B;按钮已由&#x200B;**批准**、**拒绝**&#x200B;和&#x200B;**撤消**&#x200B;按钮替换。 时间表状态更改为&#x200B;**已提交**。

   在提交您的时间表以供审批时，审批者会看到&#x200B;**主页**&#x200B;区域的&#x200B;**我的审批**&#x200B;构件中列出的时间表。 可能会出现以下情况：

   * 如果他们批准，**撤消**&#x200B;按钮将更改为&#x200B;**重新打开**，时间表状态将更新为&#x200B;**打开**。
   * 如果他们拒绝它，则&#x200B;**提交以供审批**&#x200B;按钮将替换&#x200B;**撤回**&#x200B;按钮，并且时间表状态将更新为&#x200B;**已拒绝**。

1. （可选）如果需要重新打开时间表并更新时间，请单击&#x200B;**撤消**。 有关信息，请参阅本文中的[撤回时间表](#recall-a-timesheet)部分。

### 查看已提交工时表的状态 {#view-the-status-of-a-submitted-timesheet}

提交时间表后，您可以查看时间表状态。

如果Workfront管理员启用了“批准用户时间表”和“拒绝用户时间表事件处理程序”，则在批准或拒绝时间表后会通知您。 有关启用事件通知的信息，请参阅[事件通知类型](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

如果没有这些通知，您可以在Workfront的“时间表”区域中了解已提交时间表的状态。

要查看时间表的状态，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。
1. 单击&#x200B;**时间表**。 默认情况下已选择&#x200B;**所有**&#x200B;筛选器。

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
   >   
   >   
   >   * [使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （视情况而定）如果您选择&#x200B;**我的时间表**，请确保应用&#x200B;**标准**&#x200B;视图，并注意&#x200B;**状态**&#x200B;列。

   时间表可能具有以下状态：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>您的时间表当前处于打开状态，您可以记录时间。 </p> <p>撤回的工时表显示为“未结”状态。 有关信息，请参阅本文中的<a href="#recall-a-timesheet" class="MCXref xref">撤回时间表</a>部分。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您已提交时间表以供审批，但尚未获得批准。 您可以撤回已提交的时间表以继续编辑它。 有关信息，请参阅本文中的<a href="#recall-a-timesheet" class="MCXref xref">撤回时间表</a>部分。 </td> 
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

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**时间表**。
1. 单击屏幕右上角的&#x200B;**我的时间表**，或从&#x200B;**筛选器**&#x200B;**下拉菜单中选择**&#x200B;我的时间表![](assets/filter-nwepng.png)。
1. 单击状态为&#x200B;**已提交**&#x200B;的工时表的时间范围。
1. 单击&#x200B;**撤消**。

   时间表再次变为可编辑，其状态更改为&#x200B;**打开**。
