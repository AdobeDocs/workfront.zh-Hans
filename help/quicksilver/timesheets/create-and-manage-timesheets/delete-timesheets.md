---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 删除Adobe Workfront中的工时单
description: 您对时间表配置文件所做的更改对于当前现有的时间表不会立即生效，如创建、编辑和分配时间表配置文件中所述。 要使更改在现有工时单上可见，必须删除已生成的工时单并生成新工时单。 这仅适用于通过将工时单配置文件与用户关联而生成的工时单。
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 删除Adobe Workfront中的工时单

您对时间表配置文件所做的更改对于当前现有的时间表不会立即生效，如 [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). 要使更改在现有工时单上可见，必须删除已生成的工时单并生成新工时单。 这仅适用于通过将工时单配置文件与用户关联而生成的工时单。

>[!NOTE]
>
>不能通过重新生成工时单来重新创建已手动创建的工时单，除非自手动创建工时单以来，用户已与工时单配置文件关联。 删除手动创建的时间表可能会导致数据丢失。 有关创建单个工时单的信息，请参阅 [创建一次性工时单](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Adobe Workfront管理员或组管理员可以为系统中的每个人生成时间表。 有关手动生成工时单的详细信息，请参阅：

* [手动生成工时单](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [创建和管理组的时间表配置文件](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 无法恢复已删除的时间表。
>* 我们建议您不要删除过去的工时单，因为这些工时单不会根据工时单配置文件自动生成。 如果希望在新工时单中立即显示对工时单配置文件所做的更改，则可以删除当前和未来工时单并手动生成它们。
>* 删除工时单时，不会删除针对任务、问题和项目记录的工时。 只有一般工时数会随时间表一起删除。 在单独的文本编辑器中，记下与时间表关联的一般小时数。 删除工时单后，您可以将其记录到新的工时单中。
>


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
   <td> <p>您必须对工时单具有管理访问权限。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 删除列表中的时间表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **工时单**. 的 **全部** 筛选器默认处于选中状态，它会显示您有权查看的所有时间表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）执行下列操作之一以更新工时单列表中的过滤器：

   * 选择 **我的时间表批准** ，以仅查看您批准的时间表

      或

      选择 **我的工时表** 以仅查看您的工时单。

      这会将“我的时间表审批”或“我的时间表”过滤器应用于时间表列表。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击过滤器图标 ![](assets/filter-nwepng.png) 应用其他过滤器，或创建新过滤器。 有关创建或更新过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   如果您的Workfront管理员或组管理员从“设置”区域的“列表控件”或“布局模板”中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   * [使用布局模板自定义过滤器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （可选）单击 **查看** ![](assets/view-icon.png) 或 **分组** ![](assets/grouping.png) 图标来应用其他视图或分组，或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑过滤器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 选择一个或多个要删除的时间表并单击 **删除**  ![](assets/delete.png) 时间表列表顶部的图标。

1. 单击 **删除**.

   选定的时间表将被删除且无法恢复。

   要生成新的工时单，请确保用户与工时单配置文件相关联，并要求Workfront管理员或组管理员生成新的工时单。

   有关更多信息，请参阅以下内容：

   * [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [手动生成工时单](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [创建和管理组的时间表配置文件](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## 从工时单页中删除工时单

1. 单击 [!UICONTROL **主菜单**] 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击要删除的时间表以将其打开。
1. 单击 [!UICONTROL **更多**] 图标 ![](assets/more-icon.png) 在时间表名称的右侧，单击 **删除**.

   ![从工时单页中删除工时单](assets/delete-timesheet-from-timesheet-page.png)
1. 单击 [!UICONTROL **删除**] 确认。

   时间表已删除，无法恢复。
