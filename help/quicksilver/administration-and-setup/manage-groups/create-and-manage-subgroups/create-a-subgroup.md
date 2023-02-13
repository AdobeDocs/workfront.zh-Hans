---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: 创建子组
description: 您可以在您管理的组下创建子组，以组织用户和项目并在Adobe Workfront中分配访问权限。 通常，组管理员会管理组和子组。 他们可以使用“组”页面在一个位置管理其组和子组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 3%

---

# 创建子组

您可以在您管理的组下创建子组，以组织用户和项目并在Adobe Workfront中分配访问权限。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

但是，组管理员通常会管理组和子组。 他们可以使用“组”页面在一个位置管理其组和子组。 有关组和子组在Workfront中的工作方式的信息，请参阅 [群组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md) 和 [子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 添加子组

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 选择要添加新子组的现有组或子组。
1. 单击 **新子群**.
1. 在 **新子群** 框，键入 **群组名称** 分组。
1. （可选）指定以下任一信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">组名称</td> 
      <td>更改组的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入子组的说明。 最多可键入512个字符。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">活动</td> 
      <td> <p>（默认启用）使组在您的Workfront实例中处于活动状态。</p> <p>在如下所示的“提前键入”字段中，当常规用户搜索组以将其附加到对象或与其共享对象时，列表中只显示活动组。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>要为用户简化此过程，您可以对当前未使用的组禁用“处于活动状态”选项。</p> <p>使用此字段，您可以轻松地根据活动或非活动状态查看、过滤和分组群组列表。 有关在列表中使用视图、过滤器和分组的信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">报表元素：过滤器、视图和分组</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使该组和子组公开</td> 
      <td> <p>(仅当您查看顶级组（而非子组）的详细信息时才可用。) 启用此选项，以允许具有编辑用户访问权限的子组（非组管理员）中的用户将此组及其子组添加到其他用户的用户配置文件中。</p> <p>对于公共群组，任何具有编辑用户访问权限的用户（群组内或群组外）都可以将群组添加到其他用户的配置文件中。 他们不能为私人组执行此操作。</p> <p>您只能在具有多个级别的组层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。</p> <p><b>注释</b>:  
        <ul> 
         <li>不能单独将子组设为公用，但可以将其设为顶级父组公用，这也会将父组的所有子组设为公用。</li> 
         <li>默认情况下，属于公共组的子组是公共的，因此具有编辑用户访问权限的任何用户也可以将该子组添加到其他用户。</li> 
        </ul> </p> <p>如果您需要有关编辑用户所需访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">授予用户访问权限</a>. 有关编辑用户的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">编辑用户的配置文件</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">商业领导 </td> 
      <td> <p>您可以将一个用户指定为您管理的子组的业务领导者。 业务领导者是负责子组业务决策的人。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">业务领先者概述</a><span>.</span></p> <p>如果人员尚未是子组的成员，则将其名称添加到此字段中也会将其添加到组中。</p> <p><b>注释</b>:  
        <ul> 
         <li>在从子组中删除“业务领导者”之前，必须从“业务领导者”字段中删除其名称。</li> 
         <li>如果从“业务领导者”(Business Leader)字段中删除该名称，则该用户将保持为子组的成员，除非从中删除它们。 有关从组中删除某人的说明，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">管理群组成员关系</a> 在文章中 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">管理群组</a>.</li> 
        </ul> </p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">业务领先者概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组成员和组管理员</td> 
      <td> 
       <ul> 
        <li> <p>组成员：要将用户和组添加到子组，请开始键入要添加的现有用户或组的名称，然后在显示时选择该名称。</p> <p>您添加的用户和组有权访问与该组共享的所有对象。</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">组管理员：子组会继承其上方组的组管理员，因此可以选择将用户指定为子组的组管理员。 您可以使用用户名右侧的下拉菜单，将群组成员分配为群组的管理员。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">搜索列表中的人员和组</td> 
      <td> 如果需要查找已分配给此子组的用户或组，可以在此处键入其名称，并在出现时将其选中。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存。**
