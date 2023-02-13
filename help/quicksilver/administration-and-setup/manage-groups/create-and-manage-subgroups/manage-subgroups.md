---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子组，编辑
navigation-topic: create-and-manage-subgroups
title: 管理子组
description: 作为子组的组管理员，可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。 您还可以通过将子组从其父组中删除来将其设为顶级组。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# 管理子组

作为子组的组管理员，可以创建、移动、查看、编辑、复制、重命名、导出和删除子组。

您还可以通过将子组从其父组中删除来将其设为顶级组。

如果您的组上有任何组，则其管理员也可以为您的组执行这些操作。 Workfront管理员（对于任何组）也是如此。

有关子组的更多信息，请参阅 [子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## 创建、移动、查看、编辑、复制、重命名、导出或删除子组

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

   在显示的列表中，您可以看到您管理的群组，以及这些群组拥有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要处理的子组的组名称。

   或

   如果要移动一个或多个子组，请单击目标组的名称（您将指定要在稍后步骤中移动的子组）。

1. 在左侧菜单中，单击 **子组**.

1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">创建新子组</td> 
      <td> <p>如果要从正在查看的组中向下创建新子组一级，请单击 <strong>添加子组</strong>.</p> <p>或者，如果要在列表中另一个子组下创建新子组，请选择该子组，然后单击 <strong>添加</strong><strong>子组</strong>.</p> <p>有关可用于配置子组的选项的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">创建子组</a>.</p> <p>组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移动子组 </td> 
      <td> <p>您可以在您管理的另一组下移动现有子组。</p> <p>组层次结构不能超过15个级别，但单个级别可以具有无限数量的并行组。</p> 
       <ol> 
        <li value="1"> <p>（可选）选择子组以将其设为目标组。</p> <p>如果跳过此步骤，则在步骤3中选择的组是目标组。</p> </li> 
        <li value="2">单击 <strong>添加子组</strong> &gt; <strong>现有组</strong>.</li> 
        <li value="3"> <p>在 <strong>现有组</strong> 框中，开始键入要移动的子组的名称。</p> <p>显示的结果不包含目标组上方的组。</p> <p>您可以通过将鼠标悬停在正确的组上并单击信息图标来确保选择正确的组 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> </li> 
        <li value="4"> <p>在列表中显示要移动的子组名称时，单击该子组的名称。</p> </li> 
        <li value="5"> <p>对要移动到目标组的任何其他子组重复步骤c-d</p> </li> 
        <li value="6">单击<strong>保存</strong>。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑子组</td> 
      <td> <p>选择要编辑的子组，然后单击“编辑”图标 <img src="assets/edit-icon.png">.</p> <p>有关可用于配置子组的选项的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建群组</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出一个或多个子组</td> 
      <td> 
       <ol> 
        <li value="1">选择要导出的子组。</li> 
        <li value="2">单击导出图标 <img src="assets/export.png">，然后选择所需的文件格式。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">复制子组以创建新的顶级组</td> 
      <td> <p>(仅适用于Workfront管理员。) 复制子组时，它会成为父组。 所有群组成员和子组都随其复制。 组成员保留其在原始组中拥有的任何分配。</p> <p>有关复制子组的详细信息，请参阅 <a href="#about-copying-a-subgroup" class="MCXref xref">关于复制子组</a> 在本文中。</p> 
       <ol> 
        <li value="1">选择子组，然后单击复制图标 <img src="assets/copy-icon.png"> 创建基于所选群组的新顶级群组。</li> 
        <li value="2"> <p>配置新组的设置。</p> <p>有关这些设置的帮助，请参阅部分中的表 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">通过复制现有组或子组创建顶级组</a> 在文章中 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">通过复制现有组或子组创建顶级组</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除子组</td> 
      <td> <p><b>重要信息</b>:删除组或子组时，需要保留当前分配给该组或子组的用户、工作项和任何子组。 为帮助您确保保留这些对象，系统会提示您在以下步骤中将组的对象重新分配给其他组。</p> 
       <ol> 
        <li value="1">选择子组，然后单击删除图标 <img src="assets/delete.png">.</li> 
        <li value="2">在 <strong>删除组</strong> 框中，开始键入内容，然后选择要移动所删除群组的成员、工作项和子组的群组名称。</li> 
        <li value="3">单击 <strong>删除它们</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>管理包含子组的组时，能够识别和筛选有关整个组及其所有子组的数据将非常有用。 为此，您可以使用报表或列表中的顶级父ID字段。
>
>例如，假设您管理一个大型营销部门，并且希望列出整个部门正在处理的所有项目。
>
>在Workfront中，此营销部门由一个名为“营销”的组来代表，其中包含3个名为“字段营销”、“产品营销”和“数字营销”的子组。 要列出属于整个营销部门（所有4个组）的项目，您可以使用以下过滤器规则为“项目”区域创建过滤器：
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>您还可以使用“顶级父项名称”字段来标识与顶级组关联的数据，但仅在“视图”中，而不能在“过滤器”或“分组”中。

## 从其父组中删除子组，并将其设为顶级组

通过将子组从其父组中删除，可以将其设为顶级组。

>[!TIP]
>
>当您停用下面有子组的组时，这些子组也会变为不活动。 如果希望其中一个组处于活动状态，则可以按照以下说明将其从其父组中删除，然后将其重新激活。
>
>有关停用和重新激活群组的说明，请参阅 [查看和管理群组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) 和 [查看和管理群组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) 在文章中 [查看和管理群组的详细信息](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 选择要创建顶级群组的群组的父群组，然后单击编辑图标 ![](assets/edit-icon.png).
1. 在 **编辑群组** 框，位于 **组成员和组管理员**，开始键入要创建顶级群组的子群组名称，然后在出现该子组名称右侧单击X。
1. 单击&#x200B;**保存**。

## 查看和管理组的子组成员

在查看您管理的组的主页时，可以查看和管理该组的子组中的所有用户。 有关说明，请参阅 [查看和管理子组成员](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 关于复制子组 {#about-copying-a-subgroup}

复制子组时，请考虑以下事项。

* 如果复制的子组具有其自己的子组，则它们将包含在副本中，并且其名称的格式如下：

   ```
   Original subgroup name (Copy)
   ```

* 属于公共组的任何子组也是公共的，因此具有编辑用户访问权限的任何用户，无论是进入还是退出该组，都可以将用户添加到该子组。
