---
title: 使用布局模板自定义筛选器、视图和分组
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Workfront管理员，您可以使用布局模板来指定在筛选器、视图和分组下拉菜单中显示的列表控件。 这些菜单出现在整个Workfront的上方列表中，例如项目的任务列表。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# 使用布局模板自定义筛选器、视图和分组

作为Adobe Workfront管理员，您可以使用布局模板来指定在筛选器、视图和分组下拉菜单中显示的列表控件。 这些菜单出现在整个Workfront的上方列表中，例如项目的任务列表：

![筛选器视图分组布局模板](assets/filter-view-grouping-layout-templates.png)

有关布局模板的更多信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
        <p>要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义筛选器、视图和分组列表控件

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 单击![自定义用户看到的内容](assets/down-arrow-blue.png)下的向下箭头&#x200B;**向下箭头**，然后在显示的下拉菜单中单击&#x200B;**列表**。

   ![自定义用户看到的内容](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. 单击![下的向下箭头](assets/down-arrow-blue.png)向下箭头&#x200B;**选择要自定义的列表**，然后选择要为其自定义筛选器、视图和分组列表控件的Workfront对象的类型。

   ![选择要自定义的列表](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >如果您选择项目作为要自定义的列表，然后在筛选部分禁用我所在的项目或我拥有的项目，则用户将无法再看到或无法使用该筛选器：
   >
   >* 在单击列表上方的过滤器图标![过滤器图标](assets/filter-nwepng.png)时显示的过滤器列表中：
   >   
   >  ![禁用筛选器](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* 在项目区域标题的标题中：
   >   
   >  ![禁用筛选器按钮](assets/disable-filter-pills.png)

1. （可选）如果要更改布局模板的默认筛选器、视图或分组，请将鼠标悬停在筛选器、视图或分组上，然后单击“**设置为默认值**”。

   您选择的默认值决定了将布局模板分配给用户后，用户在整个Workfront的列表中看到的筛选器、视图和分组。 如果不更改这些默认值，用户将按如下方式查看所有列表：

   * **筛选器**：全部
   * **视图**：标准（如果适用；某些列表没有此视图）
   * **分组**：无

   选择不同的缺省值后，您可以隐藏“全部”、“标准”和“无”选项（请参阅步骤5），但无法删除这些选项。

   您可以删除用作默认值的任何其他选项，但必须先选择其他默认选项。

   有关删除筛选器、视图和分组的信息，请参阅[创建、编辑和共享默认筛选器、视图和分组](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md)。

1. 按如下方式隐藏和添加列表控件：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">隐藏列表控件</td> 
      <td> <p>清除或选中要隐藏或显示的列表控件旁边的复选框。</p> <p>如果复选框灰显，则无法隐藏该列表控件。 每个列表控件的默认<img src="assets/default-pill.png">设置都呈灰显状态，因为您不能隐藏当前配置为默认设置的设置。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加自定义列表控件</td> 
      <td> <p> 
        <ol> 
         <li value="1"> 单击筛选器、视图或分组列表底部的<strong>添加筛选器</strong>、<strong>添加视图</strong>或<strong>添加分组</strong>。 在显示的框中，开始键入先前为您的组织创建的现有自定义列表控件的名称，然后在出现时单击该名称。</li> 
         <li value="2"> 如果要将新的自定义列表控件设置为布局模板的默认筛选器、视图或分组，请单击<strong>设置为默认值</strong>。 </li> 
         <li value="3"> <p>完成后，单击<strong>添加</strong>。</p> <p><b>注释</b>： <p>用户可以将自定义列表控件添加到自己的列表。 如果在布局模板中添加自定义列表控件，则会添加列表控件并将其移动到面板底部；不会替换列表控件。</p> <p>如果将用户分配到具有自定义列表控件的新布局模板，也是如此。 </p> <p>有关自定义列表控件的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">筛选器概述</a>、<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Adobe Workfront中的视图概述</a>和<a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Adobe Workfront中的分组概述</a>。</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**保存**。

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后继续修改模板。
