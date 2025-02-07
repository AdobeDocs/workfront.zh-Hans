---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 查看和管理组最近删除的项目
description: 查看在“组”区域中管理的组时，您可以查看、筛选、还原和导出其最近删除的工作项、文档和模板。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# 查看和管理组最近删除的项目

在组区域查看您管理的组时，可通过以下方式查看和处理其最近删除的项目、任务、问题、文档和模板：

* 查看、筛选和分组最近删除项的列表
* 恢复您选择的最近删除的项目
* 导出最近删除项目的列表

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

有关已删除项目的详细信息，请参阅[管理已删除项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>已删除的项目必须与组或其任何子组相关联。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

+++

## 查看和管理组最近删除的项目

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

1. 单击组的名称。
1. 在左侧面板中，单击&#x200B;**最近删除的**。
1. 打开以下选项卡之一，您想在其中查看和管理组最近删除的项目：

   * 项目
   * 任务
   * 问题
   * 文档
   * 模板

   每个选项卡都列出了属于当前组或其子组且在过去30天内删除的相应对象类型项目。

   >[!NOTE]
   >
   >如果有人删除了项目，则该项目的所有单独任务、问题和文档都将随其一起删除。 它们不会单独显示在“任务”、“问题”、“文档”或“模板”选项卡上。 但是，恢复项目也会将所有这些子对象恢复到项目中。
   >
   >
   >如果有人单独删除了任务、问题、文档或模板，则可以在相应的选项卡上查看和管理它。

1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>还原对象</p> </td> 
      <td> <p>最多选择10个对象，然后单击<strong>还原</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>导出选项卡上的整个对象列表</p> </td> 
      <td> <p>单击<strong>导出</strong>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>更改列表中的信息显示</p> </td> 
      <td> <p>在列表右上角，使用<strong>筛选器</strong>根据您提供的条件定义显示的内容。 使用<strong>视图</strong>定义哪些字段显示为列。 使用<strong>分组</strong>将项目分组为类别。</p> </td> 
     </tr> 
    </tbody> 
   </table>
