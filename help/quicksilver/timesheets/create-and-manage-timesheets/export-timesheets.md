---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 导出工时单列表
description: 作为人员经理或时间表审批者，您可能需要下载时间表列表，以快速查看有关您负责的人员时间表的信息。 您可以通过导出时间表列表来执行此操作。
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# 导出工时单列表

作为人员经理或时间表审批者，您可能需要下载时间表列表，以快速查看有关您负责的人员时间表的信息。 您可以通过导出时间表列表来执行此操作。

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
   <td> <p>查看工时单的或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 导出工时单列表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **工时单**. 的 **全部** 筛选器是默认选中的。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 键入关键字并搜索特定时间表。 例如，您可以搜索设置的时间范围或所有者名称。

1. （可选）执行下列操作之一以更新工时单列表中的过滤器：

   * 选择 **我的时间表批准** ，以仅查看您批准的时间表

      或

      选择 **我的工时表** 以仅查看您的工时单。

      这会将“我的时间表审批”或“我的时间表”过滤器应用于时间表列表。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击过滤器图标 ![](assets/filter-nwepng.png) 应用其他过滤器，或创建新过滤器。 有关创建或更新过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的“列表控件”或“布局模板”中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   * [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （可选）单击 **查看** ![](assets/view-icon.png) 或 **分组** ![](assets/grouping.png) 图标来应用其他视图或分组，或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 选择要导出的时间表，然后单击 **导出**  ![](assets/export-38x15.png) 图标。

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. 从以下选项中选择要将工时单列表导出到的文件类型：

   * PDF景观
   * PDF纵向
   * PDF其他大小
   * Excel
   * Excel (xlsx)
   * 制表符分隔

   时间表列表将以所选格式下载到您的计算机，并包括以下时间表信息：

   * 日期范围
   * 所有者姓名
   * 总小时数
   * 加班金额
   * 批准者名称
   * 状态
