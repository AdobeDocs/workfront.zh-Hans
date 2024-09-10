---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子组，编辑
navigation-topic: create-and-manage-subgroups
title: 管理子组
description: 作为子组的组管理员，您可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。 您还可以通过从子组的父组中将其删除来将该子组设置为顶级组。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 1%

---

# 管理子组

作为子组的组管理员，您可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。

您还可以通过从子组的父组中将其删除来将该子组设置为顶级组。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

有关子组的详细信息，请参阅[子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建、移动、查看、编辑、复制、重命名、导出或删除子组

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要处理的子组的组的组的名称。

   或

   如果要移动一个或多个子组，请单击目标组的名称（您将在后面的步骤中指定要移动的子组）。

1. 在左侧菜单中，单击&#x200B;**子组**。

1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">创建新子组</td> 
      <td> <p>如果要从正在查看的组创建下一级的新子组，请单击<strong>添加子组</strong>。</p> <p>或者，如果要在列表中的另一个子组下创建新子组，请选择该子组，然后单击<strong>添加s</strong><strong>子组</strong>。</p> <p>有关可用于配置子组的选项的信息，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">创建子组</a>中的表。</p> <p>组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移动子组 </td> 
      <td> <p>您可以将现有子组移动到您管理的另一个组下。</p> <p>组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。</p> 
       <ol> 
        <li value="1"> <p>（可选）选择一个子组以使其成为目标组。</p> <p>如果跳过此步骤，则在步骤3中选择的组就是目标组。</p> </li> 
        <li value="2">单击<strong>添加子组</strong> &gt; <strong>现有组</strong>。</li> 
        <li value="3"> <p>在出现的<strong>现有组</strong>框中，开始键入要移动的子组的名称。</p> <p>显示的结果不包含目标组上方的组。</p> <p>您可以确保选择正确的组，方法是将鼠标悬停在该组上，然后单击该组旁边显示的信息图标<img src="assets/info-icon.png">。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> </li> 
        <li value="4"> <p>当看到子组显示在列表中时，单击要移动的子组的名称。</p> </li> 
        <li value="5"> <p>对于要移动到目标组的任何其他子组，重复步骤c - d</p> </li> 
        <li value="6">单击<strong>保存</strong>。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑子组</td> 
      <td> <p>选择要编辑的子组，然后单击编辑图标<img src="assets/edit-icon.png">。</p> <p>有关可用于配置子组的选项的信息，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建组</a>中的表。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出一个或多个子组</td> 
      <td> 
       <ol> 
        <li value="1">选择要导出的一个或多个子组。</li> 
        <li value="2">单击导出图标<img src="assets/export.png">，然后选择所需的文件格式。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制子组以创建新的顶级组</td> 
      <td> <p>(仅适用于Workfront管理员。) 复制子组时，它将变为父组。 所有组成员及子组都会随该模板一起复制。 群组成员保留其在原始群组中的任何分配。</p> <p>有关复制子组的详细信息，请参阅本文中的<a href="#about-copying-a-subgroup" class="MCXref xref">关于复制子组</a>。</p> 
       <ol> 
        <li value="1">选择一个子组，然后单击“复制”图标<img src="assets/copy-icon.png">以根据所选组创建新的顶级组。</li> 
        <li value="2"> <p>配置新组的设置。</p> <p>有关这些设置的帮助，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">复制现有组或子组</a>中的项目<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">通过复制现有组或子组创建顶层组</a>部分中的表。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除子组</td> 
      <td> <p><b>重要信息</b>：删除组或子组时，需要保留用户、工作项和当前分配给它的任何子组。 为了帮助您确保它们被保留，出现提示要求您在下面的步骤中将该组的对象重新分配给另一个组。</p> 
       <ol> 
        <li value="1">选择子组，然后单击删除图标<img src="assets/delete.png">。</li> 
        <li value="2">在出现的<strong>删除组</strong>框中，开始键入，然后选择要移动要删除的组的成员、工作项和子组的组的组名。</li> 
        <li value="3">单击<strong>删除它们</strong>。</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>在管理包含子组的组时，能够识别和过滤有关整个组及其所有子组的数据会很有帮助。 您可以使用报表或列表中的顶级父项ID字段完成此操作。
>
>例如，假设您管理一个庞大的营销部门，并且想要一个包含整个部门正在处理的所有项目的列表。
>
>在Workfront中，该营销部门由一个称为营销的组表示，该组包含3个称为现场营销、产品营销和数字营销的子组。 要列出属于整个营销部门（全部4个组）的项目，您可以使用以下筛选规则为项目区域创建一个筛选器：
>
>`Group: Top Parent ID > Equal > Marketing`
>
>您还可以使用“顶级父代名称”字段来标识与顶级组关联的数据，但只能标识在视图中，而不能标识在筛选器或分组中。

## 从父组中移除子组，并将其设为顶级组

通过从子组的父组中将其删除，可以将子组设置为顶级组。

>[!TIP]
>
>当您取消激活下面具有子组的组时，这些子组也会变为非活动状态。 如果您希望其中一个处于活动状态，可以使用这些说明将其从父组中移除，然后重新激活它。
>
>有关停用和重新激活组的说明，请参阅[查看和管理组详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)文章中的[查看和管理组详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view)和[查看和管理组详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive)部分。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

1. 选择要成为顶级组的组的父组，然后单击编辑图标![](assets/edit-icon.png)。
1. 在出现的&#x200B;**编辑组**&#x200B;框中，在&#x200B;**组成员和管理员**&#x200B;下，开始键入要成为顶级组的子组的名称，然后单击该组出现时其名称右侧的X。
1. 单击&#x200B;**保存**。

## 查看和管理组的子组成员

在查看您管理的组的主页时，您可以查看和管理该组子组中的所有用户。 有关说明，请参阅[查看和管理子组成员](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

## 关于复制子组 {#about-copying-a-subgroup}

复制子组时，请考虑以下事项。

* 如果复制的子组有自己的子组，则它们会包含在副本中，其名称的格式如下所示：

  `Original subgroup name (Copy)`

* 属于公共组的任何子组也是公共的，因此任何具有编辑用户访问权限的用户（在组内或组外）都可以向该子组添加用户。
