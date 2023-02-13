---
title: 使用布局模板自定义过滤器、视图和分组
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Workfront管理员，您可以使用布局模板来指定在“过滤器”、“视图”和“分组”下拉菜单中显示的列表控件。 这些菜单显示在整个Workfront的列表上方，如项目的任务列表。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# 使用布局模板自定义过滤器、视图和分组

作为Adobe Workfront管理员，您可以使用布局模板来指定在“过滤器”、“视图”和“分组”下拉菜单中显示的列表控件。 这些菜单显示在整个Workfront的列表上方，例如项目的任务列表：

![](assets/filter-view-grouping-layout-templates.png)

有关布局模板的更多信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问权限级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义过滤器、视图和分组列表控件：

1. 开始使用布局模板，如 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击向下箭头 ![](assets/down-arrow-blue.png) 在 **自定义用户看到的内容**，然后单击 **列表** 下拉菜单（显示）中。

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. 单击向下箭头 ![](assets/down-arrow-blue.png) 在 **选择要自定义的列表**，然后选择要为其自定义过滤器、视图和分组列表控件的Workfront对象类型。

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >如果您选择项目作为要自定义的列表，然后在过滤器部分禁用我所在的项目或我拥有的项目，则用户将无法再看到或无法使用该过滤器：
   >
   >* 在单击过滤器图标时显示的过滤器列表中 ![](assets/filter-nwepng.png) 列表上方：
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* 在“项目”区域标题的标题中：
   >   
   >  ![](assets/disable-filter-pills.png)

1. （可选）如果要更改布局模板的默认过滤器、视图或分组，请将鼠标悬停在过滤器、视图或分组上，然后单击 **设置为默认值**.

   您选择的默认值决定了在为用户分配布局模板后，在整个Workfront的列表中，将会看到哪些过滤器、视图和分组用户。 如果不更改这些默认值，则用户将按以下方式看到所有列表：

   * **过滤器**:全部
   * **查看**:标准（如适用）；某些列表没有此视图)
   * **分组**:无

   在选择不同的默认值后，您可以隐藏选项“全部”、“标准”和“无”（请参阅步骤5），但无法删除这些选项。

   您可以删除用作默认值的任何其他选项，但必须先选择其他默认选项。

   有关删除过滤器、视图和分组的信息，请参阅 [创建、编辑和共享默认过滤器、视图和分组](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. 按如下方式隐藏和添加列表控件：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">隐藏列表控件</td> 
      <td> <p>清除或选中要隐藏或显示的列表控件旁边的复选框。</p> <p>如果复选框灰显，则无法隐藏该列表控件。 默认 <img src="assets/default-pill.png"> 每个列表控件的设置都会变暗，因为您无法隐藏当前配置为默认设置的设置。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加自定义列表控件</td> 
      <td> <p> 
        <ol> 
         <li value="1"> 单击 <strong>添加过滤器</strong>, <strong>添加视图</strong>或 <strong>添加分组</strong> “筛选器”、“查看”或“分组”列表底部的“筛选器”。 在显示的框中，开始键入之前为您的组织创建的现有自定义列表控件的名称，然后在显示该名称时单击该名称。</li> 
         <li value="2"> 如果希望将新的自定义列表控件设置为布局模板的默认过滤器、视图或分组，请单击 <strong>设置为默认值</strong>. </li> 
         <li value="3"> <p>单击 <strong>添加</strong> 完成。</p> <p><b>注释</b>: <p>用户可以将自定义列表控件添加到其自己的列表。 如果在布局模板中添加自定义列表控件，则会添加列表控件并将其移至面板底部；你的不能取代他们的。</p> <p>如果您将用户分配到具有自定义列表控件的新布局模板，则也是如此。 </p> <p>有关自定义列表控件的信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">过滤器Adobe Workfront概述</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">视图Adobe Workfront概述</a>和 <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Adobe Workfront中的分组概述</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后稍后继续修改模板。
