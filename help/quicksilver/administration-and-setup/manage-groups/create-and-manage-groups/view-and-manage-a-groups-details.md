---
title: 查看和管理群组的详细信息
description: 您可以查看和编辑您管理的组或子组的“组详细信息”页。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# 查看和管理群组的详细信息

您可以查看和编辑您管理的组或子组的“组详细信息”页。 此页面包括：

* 群组描述
* 业务领导和组管理员的姓名
* 允许您将组及其子组设为公用或专用的选项

   <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

有关可以管理群组的其他方式的信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

有关如何停用或重新激活群组的信息，请参阅 [停用或重新激活群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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

## 查看和管理群组的详细信息

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **群组**.

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击要编辑的顶级群组的名称。
1. 如果要停用或重新激活群组，请
1. 在左侧菜单中，单击 **组详细信息**，然后执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td> <p>最多可键入512个字符。</p> <p>如果字段为空，请单击 <strong>添加</strong> 键入描述。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">活动</td> 
      <td> <p>（默认启用）使组在您的Workfront实例中处于活动状态。</p> <p>在如下所示的“提前键入”字段中，当常规用户搜索组以将其附加到对象或与其共享对象时，列表中只显示活动组。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>要为用户简化此过程，您可以对当前未使用的组禁用“处于活动状态”选项。</p> <p>使用此字段，您可以轻松地根据活动或非活动状态查看、过滤和分组群组列表。 有关在列表中使用视图、过滤器和分组的信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报表元素：过滤器、视图和分组</a>.</p> <p>有关不活动群组的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">非活动组的注意事项</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">删除或停用自定义表单</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组辅助</td> 
      <td> <p>(仅当您查看群组（而非子群组）的详细信息时才可用。) 启用或禁用选项 <strong>将此组和子组设为私有</strong>.</p> <p>对于公共群组，任何具有编辑用户访问权限的用户（群组内或群组外）都可以将群组添加到其他用户的配置文件中。 他们不能为私人组执行此操作。</p> <p>您只能在具有多个级别的组层次结构中的顶层父组上编辑此选项。 父组的所有子组将继承其设置。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组利益相关者</td> 
      <td> 
       <ul> 
        <li><strong>组管理员</strong>:添加或删除具有计划员许可证的用户作为群组的群组管理员。 开始键入用户的名称，然后在下拉菜单中显示该名称时单击该名称。</li> 
        <li><strong>业务领袖</strong>:执行以下操作之一：
         <ul>
          <li>如果尚未为组分配业务领导，请单击 <strong>添加</strong>，开始键入要分配的用户名，然后在显示时单击该人员的姓名。</li>
          <li>如果组已经有业务领导者，并且您想要更改它，请双击现有业务领导者的名称。 删除该名称，开始键入要分配的用户名称，然后在显示时单击该人的名称。</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加自定义表单</td> 
      <td>如果您的访问级别允许您管理自定义表单，请向群组添加自定义表单。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">自定义表单</a>.</td> 
     </tr> 
    </tbody> 
   </table>
