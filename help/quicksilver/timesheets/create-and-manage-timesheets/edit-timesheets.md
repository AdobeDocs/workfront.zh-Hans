---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 编辑工时单信息
description: 作为对工时单具有管理访问权限的用户，您可以在Adobe Workfront中编辑有关现有工时单的信息。 例如，您可以编辑工时单的“所有者”、“批准者”或时间范围。
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# 编辑工时单信息

作为对工时单具有管理访问权限的用户，您可以在Adobe Workfront中编辑有关现有工时单的信息。 例如，您可以编辑工时单的“所有者”、“批准者”或时间范围。

您可以编辑单个工时单的信息，也可以批量编辑多个工时单。

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
   <td> <p>您必须对工时单具有管理访问权限。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑工时单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **工时单**.

   的 **全部** 筛选器默认处于选中状态，该筛选器显示您有权查看的所有工时单。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 键入关键字并搜索特定的时间表。 例如，您可以搜索时间表时间范围或所有者名称。

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


1. （可选）单击&#x200B;**查看** ![](assets/view-icon.png) 或 **分组** ![](assets/grouping.png) 图标来应用其他视图或分组，或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 选择一个或多个时间表，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 时间表列表顶部。
1. 查看或指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>这是为其创建工时单的用户名称。 您无法编辑此字段。 </p> <p>选择多个工时单时，不显示该字段。 </p> </td> 
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
      <td> <p>批准者是为与时间表关联的用户批准时间表的用户。 只有对工时单具有管理访问权限的用户才能设置为批准者。 </p> <p>有关工时单管理权限的详细信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>开始输入时间表批准者的名称，并在列表中显示时选择它们。</p> <p>一个时间表上可以有多个批准者。 在这种情况下，在其中一个批准者批准时间表后，时间表将被标记为 <strong>已关闭</strong> 然后它会从所有剩余批准者的时间表批准列表中消失。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可以编辑时间</strong> </td> 
      <td> <p>如果要允许批准者编辑工时单上的工时，请选择此选项。</p> <p>当您选择多个工时单时，此选项不可用。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td> <p>您可以选择隐藏工时单上的“超时”框。</p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击保存。
