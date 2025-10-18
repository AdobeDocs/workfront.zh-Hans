---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子组，编辑
navigation-topic: create-and-manage-subgroups
title: 管理子组
description: 作为子组的组管理员，您可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。 您还可以通过从子组的父组中将其删除来将该子组设置为顶级组。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# 管理子组

作为子组的组管理员，您可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。

您还可以通过从子组的父组中将其删除来将该子组设置为顶级组。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

有关子组的详细信息，请参阅[子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

>[!TIP]
>
>在管理包含子组的组时，能够识别和过滤有关整个组及其所有子组的数据会很有帮助。 您可以使用报表或列表中的顶级父项ID字段完成此操作。
>
>例如，假设您管理一个庞大的营销部门，并且想要一个包含整个部门正在处理的所有项目的列表。
>
>在Workfront中，该营销部门由一个称为营销的组表示，该组包含3个称为现场营销、产品营销和数字营销的子组。 要列出属于整个营销部门（全部4个组）的项目，您可以使用以下筛选规则为项目区域创建筛选器：
>
>`Group: Top Parent ID > Equal > Marketing`
>
>您还可以使用“顶级父代名称”字段来标识与顶级组关联的数据，但仅限于视图，而不能用于筛选器或组。

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
  <tr> 
   <td>访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建子组

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击要添加子组的组的组的名称。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. 若要从您正在查看的组创建下一级的新子组，请单击&#x200B;**添加子组**。

   或者，如果要在列表中的另一个子组下创建新子组，请选择该子组，然后单击&#x200B;**添加子组**。

   有关可用于配置子组的选项的信息，请参阅[创建子组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

   组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。

## 移动子组

您可以将现有子组移动到您管理的另一个组下。

组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击目标组的名称（您将在后续步骤中指定要移动的子组）。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. （可选）选择一个子组以使其成为目标组。

   如果跳过此步骤，则在步骤3中选择的组就是目标组。

1. 单击&#x200B;**添加子组>现有组**。
1. 在出现的&#x200B;**现有组**&#x200B;框中，开始键入要移动的子组的名称。

   显示的结果不包含目标组上方的组。

   您可以确保选择正确的组，方法是将鼠标悬停在该组上，然后单击该组旁边显示的信息图标![信息图标](assets/info-icon.png)。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。

1. 在列表中找到要移动的子组时，请选择要移动的子组的名称。
1. 对要移动到目标组的任何其他子组重复步骤7 - 8。
1. 单击&#x200B;**保存**。

## 编辑子组

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要编辑的子组的组的名称。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. 选择要编辑的子组，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

   有关可用于配置子组的选项的信息，请参阅[创建子组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 复制子组

>[!NOTE]
>
>只有系统管理员才能复制子组。

复制子组时，它将变为父组。 所有组成员及子组都会随该模板一起复制。 该组成员保留其在原始组中的任何分配。

复制子组时，请考虑以下事项：

* 如果复制的子组有自己的子组，则它们会包含在副本中，其名称的格式如下所示：

  `Original subgroup name (Copy)`

* 属于公共组的任何子组也是公共的，因此任何有权编辑用户（在组中或组外）的用户都可以将用户添加到该子组。

要复制子组，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要复制的子组的组的名称。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. 选择一个子组，然后单击&#x200B;**复制**&#x200B;图标![复制图标](assets/copy-icon.png)以根据所选组创建新的顶级组。
1. 配置新组的设置。

   有关这些设置的帮助，请参阅[创建组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)一文中的[通过复制现有组或子组来创建顶级组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

1. 单击&#x200B;**创建群组**。

## 导出子组

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要导出的子组的组的组的名称。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. 选择要导出的一个或多个子组。
1. 单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export.png)，然后选择所需的文件格式。

## 从父组中移除子组，并将其设为顶级组

通过从子组的父组中将其删除，可以将子组设置为顶级组。

>[!TIP]
>
>当您取消激活下面具有子组的组时，这些子组也会变为非活动状态。 如果您希望其中一个处于活动状态，可以使用这些说明将其从父组中移除，然后重新激活它。
>&#x200B;>有关停用和重新激活组的说明，请参阅[停用或重新激活组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。
1. 选择要成为顶级组的子组的父组，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
1. 在出现的&#x200B;**编辑组**&#x200B;框中，在&#x200B;**搜索**&#x200B;字段（**组成员和组管理员**&#x200B;下）开始键入要成为顶级组的子组的名称，然后单击该组出现时其名称右侧的X。
1. 单击&#x200B;**保存**。

## 删除子组

>[!IMPORTANT]
>
>删除组或子组时，需要保留用户、工作项以及当前分配给它的任何子组。 为了帮助您确保它们被保留，出现提示要求您将组的对象重新分配给另一个组。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要删除的子组的组的名称。
1. 在左侧菜单中，单击&#x200B;**子组**。
1. 选择子组，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

   在出现的&#x200B;**删除组**&#x200B;框中，开始键入，然后选择要移动要删除的组的成员、工作项和子组的组的组名称。

1. 单击&#x200B;**删除它**。

## 查看和管理组的子组成员

在查看您管理的组的主页时，您可以查看和管理该组子组中的所有用户。 有关说明，请参阅[查看和管理子组成员](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

