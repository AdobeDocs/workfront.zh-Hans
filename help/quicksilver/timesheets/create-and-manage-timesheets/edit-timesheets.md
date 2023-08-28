---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 编辑工时表信息
description: 作为对时间表具有管理访问权限的用户，您可以在Adobe Workfront中编辑有关现有时间表的信息。 例如，您可以编辑所有者、批准者或时间表的时间范围。
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 1%

---

# 编辑工时表信息

作为对时间表具有管理访问权限的用户，您可以在Adobe Workfront中编辑有关现有时间表的信息。 例如，您可以编辑所有者、批准者或时间表的时间范围。

您可以编辑单个时间表上的信息，也可以批量编辑多个时间表。

>[!IMPORTANT]
>
>如果用户与时间表配置文件关联并且时间表是自动生成的，则您对现有时间表进行的更改不会反映在为未来日期生成的时间表中。 所有自动生成的工时表都具有在工时表配置文件中建立的设置。 有关更多信息，请参阅 [创建周期性工时表](../create-and-manage-timesheets/create-timesheet-profiles.md)


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
   <td> <p>您必须对时间表具有管理访问权限。 </p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑工时表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **时间表**.

   此 **全部** 默认情况下选中过滤器以显示您有权查看的所有时间表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 和键入关键字并搜索特定时间表。 例如，您可以搜索时间表时间范围或所有者名称。

1. （可选）执行以下操作之一以更新时间表列表中的过滤器：

   * 选择 **我的工时表批准** ，以仅查看您批准的时间表

     或

     选择 **我的工时表** 以仅查看您的时间表。

     这会将我的时间表批准或我的时间表过滤器应用到时间表列表。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 单击过滤器图标 ![](assets/filter-nwepng.png) 以应用其他过滤器，或创建一个新过滤器。 有关创建或更新过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的列表控件或布局模板中删除了“我的时间表审批”和“我的时间表”过滤器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表顶部或过滤器列表中。 有关更多信息，请参阅以下文章：
   >
   >   
   >   
   * [使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （可选）单击&#x200B;**视图** ![](assets/view-icon.png) 或 **分组** ![](assets/grouping.png) 用于应用其他视图或分组或创建新视图或分组的图标。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 选择一个或多个时间表，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 位于时间表列表顶部。
1. 查看或指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>这是为其创建时间表的用户的名称。 您无法编辑此字段。 </p> <p>选择多个时间表时，不显示该字段。 </p> </td> 
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
      <td role="rowheader"><strong>状态</strong> </td> 
      <td> 这是时间表的状态。
      以下是可能的工时表状态选项： 
      <ul><li><b>打开</b>：时间表处于打开状态，可以编辑小时条目。</li>
      <li><b>已提交</b>：工时表提交给指定的批准者进行批准。</li>
      <li><b>被拒绝</b>：时间表未获得批准者的批准，现在用户可再次编辑时间条目。</li>
      <li><b>已关闭</b>：时间表已被用户关闭或由审批者批准，因此现在已关闭。 您不能向已关闭的工时表添加时间。</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>审批者</strong> </td> 
      <td> <p>批准者是批准与时间表关联的用户的时间表的用户。 只有对时间表具有管理访问权限的用户才能设置为批准者。 </p> <p>有关时间表管理权限的详细信息，请参见 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>开始输入时间表批准者的名称，并在他们出现在列表中时选择他们。</p> <p>您在一个时间表上可以有多个批准者。 在这种情况下，在某位批准者批准该时间表后，该时间表将标记为 <strong>已关闭</strong> 并且它从所有剩余批准者的时间表批准列表中消失。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可以编辑时间</strong> </td> 
      <td> <p>如果要允许批准者在时间表上编辑小时数，请选择此选项。</p> <p>当您选择多个时间表时，此选项不可用。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td> <p>您可以选择在时间表上隐藏“加班”框。</p> <p>此选项默认处于禁用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
