---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 批准时间表
description: 时间表的批准过程使经理能够查看其直接报告的工作时间。 批准者可以确认记录的所有时间都分配在正确的区域，并确认该期间已记录足够的小时数。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 批准时间表

时间表的批准过程使经理能够查看其直接报告的工作时间。 批准者可以确认记录的所有时间都分配在正确的区域，并确认该期间已记录足够的小时数。

Adobe Workfront提供配置时间表审批以在此区域中提供支持的功能。

有关提交时间表的信息，请参阅 [提交时间表以供审批](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 指定时间表批准者

通常，时间表由职能管理人员或人力资源人员批准。 （项目经理通常不会批准工时单。）

在创建工时单配置文件时定义工时单审批者。 您必须拥有计划许可证才能指定为审批者。

有关指定时间表批准者的详细信息，请参阅 [创建或编辑工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) 在文章中 [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 批准时间表

您可以批准已提交且已指定为审批者的任何工时单。 提交工时单以供审批后，该工时单将列在 **批准** 区域 **主页**  页面。 有关更多信息，请参阅 [批准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

如果Workfront管理员已启用“用户工时单审批”和“用户工时单拒绝”事件处理程序，则在工时单被批准或拒绝后，系统会通知您。 有关启用事件通知的信息，请参阅 [事件通知在Adobe Workfront中可用](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

要批准时间表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击 **工时单**.
1. 选择 **我的时间表批准** ，以仅查看您批准的时间表

   或

   选择 **我的时间表批准** 过滤器。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的“列表控件”或“布局模板”中删除了“我的时间表审批”筛选器，则“我的时间表审批”选项不会显示在时间表列表顶部或筛选器列表中。 有关更多信息，请参阅以下文章：
   * [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 在时间表列表顶部键入关键字以查找特定时间表。 您可以搜索时间范围、所有者或审批者的姓名。
1. 单击要批准的时间表的时间范围。 此时会打开时间表。

   >[!TIP]
   等待批准的工时单的状态为 [!UICONTROL 已提交].


1. 单击 **批准**

   或

   如果要拒绝时间表，请单击 **拒绝** 工时单左下角。

   如果已批准，时间表状态将更改为 **已关闭**.

   如果被拒绝，时间表状态将更改为 **被拒绝**.
