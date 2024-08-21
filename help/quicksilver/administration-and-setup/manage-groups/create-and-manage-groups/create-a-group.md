---
user-type: administrator
product-area: system-administration;user-management
keywords: 创建，组，子组，新建
navigation-topic: create-and-manage-groups
title: 创建组
description: 作为Adobe Workfront管理员，您可以创建组以整理用户和项目并在Workfront中分配访问权限。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 3%

---

# 创建组

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

作为Adobe Workfront管理员，您可以创建组以整理用户和项目并在Workfront中分配访问权限。 有关详细信息，请参阅[组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

每个子组至少需要一个组管理员。 组管理员可以使用“组”页面在一个位置管理其组。

如果您是组管理员或Workfront管理员，则还可以在组下创建子组。 有关说明，请参阅[创建子组](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

+++

## 从头开始创建顶级组

这些步骤说明了如何从头开始创建新组。 有关通过复制现有组或子组来创建组或子组的信息，请参阅本文中的[通过复制现有组或子组来创建顶级组](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)。

您必须是Workfront管理员才能创建顶级组。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

1. 在组列表上方，单击&#x200B;**新建组**。

   >[!TIP]
   >
   >在组列表的底部，您还可以单击&#x200B;**添加更多组**&#x200B;以内联添加组，然后在添加完组信息后单击&#x200B;**Enter**。

1. 在显示的&#x200B;**新建组**&#x200B;框中，键入组的名称。
1. 指定以下信息：

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
      <td>键入组的说明。 最多可键入512个字符。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">为活动</td> 
      <td> <p>（默认启用）在Workfront实例中激活组。</p> <p>在如下所示的预输入字段中，当常规用户搜索组以将其附加到对象或与其共享对象时，列表中只会显示活动组。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>要简化用户的这项操作，您可以对当前未使用的组禁用“处于活动状态”选项。</p> <p>使用此字段，您可以轻松地根据活动或非活动状态查看、筛选和分组组列表。 有关在列表中使用视图、筛选器和分组的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报告元素：筛选器、视图和分组</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使该组和子组公开</td> 
      <td> <p>(仅在查看顶级组（而非子组）的详细信息时可用。) 启用此选项可允许组中具有编辑用户访问权限的用户（不是组的管理员）将此组及其子组添加到其他用户的用户配置文件中。</p> <p>对于公共组，任何具有编辑用户访问权限的用户（在组中或组外）都可以将该组添加到其他用户的配置文件中。 他们无法为专用组执行此操作。</p> <p>您只能在具有多个级别的组的层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。</p> <p><b>注释</b>：  
        <ul> 
         <li>不能将子组本身设为公用，但可以将其顶级父组设为公用，这样也可以使父代的所有子组设为公用。</li> 
         <li>默认情况下，属于公共组的子组是公用的，因此任何具有编辑用户访问权限的用户都可以将该子组添加到其他用户。</li> 
        </ul> </p> <p>如果您需要有关编辑用户所需访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。 有关编辑用户的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">商业领导 </td> 
      <td> <p>您可以将一个用户指定为您管理的组的业务负责人。 业务负责人是为组制定业务决策的人员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">业务负责人概述</a><span>.</span></p> <p>如果人员还不是组的成员，则向此字段添加人员的姓名也会将其添加到组中。</p> <p><b>注释</b>：  
        <ul> 
         <li>您必须先从“业务领导者”字段中移除其名称，然后才能从组中移除“业务领导者”。</li> 
         <li>如果从“业务领导者”字段中移除该名称，则该用户仍然是组的成员，除非将其从组中移除。 有关从组中删除某人的说明，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">管理组</a>一文中的<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">管理组成员资格</a>部分。</li> 
        </ul> </p> <p>有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">业务负责人概述</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组成员和组管理员</td> 
      <td>
        <p>要添加组成员，请开始键入要添加的现有用户或组的名称，然后在其出现时选择名称。</p> 
        <p>您添加的用户和组有权访问与该组共享的所有对象。</p>
        <p>顶级组必须至少有一个组管理员。 </p>
     </tr> 
     <tr> 
      <td role="rowheader">搜索列表中的人员和组</td> 
      <td> 如果您需要查找已分配给此组的用户或组，可以在此处键入其名称，并在其出现时将其选定。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**创建群组**。

## 通过复制现有组或子组创建顶层组 {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

作为Workfront管理员，您可以通过复制现有组或子组来创建新的顶级组。

执行此操作时，请牢记以下几点：

* 属于现有组的所有成员和任何子组都将复制到新的顶级组。
* 复制组的成员将保留其在原始组中的分配。 因此，原始组的组管理员也被指定为复制组中的组管理员。

要通过复制组或子组来创建新的顶层组，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 选择要复制的组，然后单击复制图标![](assets/copy-icon.png)。
1. 在出现的&#x200B;**复制组**&#x200B;框中，为复制的组键入&#x200B;**组名称**。

1. 指定以下信息：

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
      <td>键入组的说明。 最多可键入512个字符。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">为活动</td> 
      <td> <p>（默认启用）在Workfront实例中激活组。</p> <p>在如下所示的预输入字段中，当常规用户搜索组以将其附加到对象或与其共享对象时，列表中只会显示活动组。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>要简化用户的这项操作，您可以对当前未使用的组禁用“处于活动状态”选项。</p> <p>使用此字段，您可以轻松地根据活动或非活动状态查看、筛选和分组组列表。 有关在列表中使用视图、筛选器和分组的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">报告元素：筛选器、视图和分组</a>。</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使该组和子组公开</td> 
      <td> <p>(仅在查看顶级组（而非子组）的详细信息时可用。) 启用此选项可允许组中具有编辑用户访问权限的用户（不是组的管理员）将此组及其子组添加到其他用户的用户配置文件中。</p> <p>对于公共组，任何具有编辑用户访问权限的用户（在组中或组外）都可以将该组添加到其他用户的配置文件中。 他们无法为专用组执行此操作。</p> <p>您只能在具有多个级别的组的层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。</p> <p><b>注释</b>：  
        <ul> 
         <li>不能将子组本身设为公用，但可以将其顶级父组设为公用，这样还可以将父代的所有子组设为公用。</li> 
         <li>默认情况下，属于公共组的子组是公用的，因此任何具有编辑用户访问权限的用户都可以将该子组添加到其他用户。</li> 
        </ul> </p> <p>如果您需要有关编辑用户所需访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">授予用户访问权限</a>。 有关编辑用户的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">编辑用户的配置文件</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">商业领导 </td> 
      <td> <p>您可以将一个用户指定为您管理的组的业务负责人。 业务负责人是为组制定业务决策的人员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">业务负责人概述</a><span>.</span></p> <p>如果人员还不是组的成员，则向此字段添加人员的姓名也会将其添加到组中。</p> <p><b>注释</b>：  
        <ul> 
         <li>您必须先从“业务领导者”字段中移除其名称，然后才能从组中移除“业务领导者”。</li> 
         <li>如果从“业务领导者”字段中移除该名称，则该用户仍然是组的成员，除非将其从组中移除。 有关从组中删除某人的说明，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">管理组</a>一文中的<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">管理组成员资格</a>部分。</li> 
        </ul> </p> <p>有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">业务负责人概述</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组成员和组管理员</td> 
      <td> 
       <ul> 
        <li> <p>组成员：要将用户和组添加到组，请开始键入要添加的现有用户或组的名称，然后在出现时选择该名称。</p> <p>您添加的用户和组可以访问与该组共享的所有对象。</p> </li> 
        <li> <p>组管理员：原始组的任何组管理员也将被指定为复制组中的组管理员。 您可以使用用户名右侧的下拉菜单将组成员指定为组的管理员。</p> <p>顶级组必须至少有一个组管理员。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">搜索列表中的人员和组</td> 
      <td> 如果您需要查找已分配给此组的用户或组，可以在此处键入其名称，并在其出现时将其选定。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* 如果原始组具有子组，则子组将添加到新组中，并且其名称默认为“原始子组名称（复制）”。
   >* 通过单击用户或子组名称右侧的X ，可以将任何用户或子组从原始组中删除。

1. 单击&#x200B;**创建群组**。
