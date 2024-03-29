---
product-area: projects
navigation-topic: manage-issues
title: 修改列表中多个问题的用户分配
description: 修改列表中多个问题的用户分配
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 修改列表中多个问题的用户分配

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

您可以同时将用户分配修改为多个问题。 有关编辑问题或一次分配一个问题的信息，另请参阅以下文章：

* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [分配问题](../../../manage-work/issues/manage-issues/assign-issues.md)

有关分配问题的一般信息，请参阅 [修改问题分配的概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>您必须至少具有问题的Contribute权限，才能为该问题分配工作。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多个问题的分配

1. 转到问题列表，其中包含要修改其分配的问题。
1. （可选）创建一个过滤器，以仅显示分配给要修改的被分派人的问题。

   例如，您可以创建一个过滤器，以仅显示具有作为被分配人的特定角色的问题。 然后，您可以使用特定用户替换角色。 执行以下操作：

   1. 单击 **筛选** 下拉列表，然后单击 **新建筛选器**.

      此时将显示“新建过滤器”对话框。

   1. 单击 **添加筛选器规则。**
   1. 要筛选特定角色，请展开 **任务角色，** 然后单击 **标识。**

      或

      要筛选特定用户，请展开 **任务用户，** 然后单击 **标识。**

      >[!TIP]
      >
      >不使用 **分派给** 因为此字段仅引用问题所有者，而不引用所有被分配人。

   1. 在下拉列表中，选择 **等于** 作为过滤器限定符。
   1. 开始键入要筛选的用户或角色的名称，然后在名称出现在下拉列表中时单击该名称。
   1. 单击 **保存筛选器。**

1. 选择要修改分配的问题，然后单击 **编辑** 图标 ![](assets/qs-edit-icon.png).

   此 **编辑问题** 显示。 已编辑的项目显示在页面的左上角。

1. 转到 **指定任务** 部分，然后选择 **被分派人**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 执行下列操作之一：

   1. 要添加新的被分派人，请执行以下操作：

      1. 开始键入用户、角色或团队的名称，然后在该名称显示在列表中时将其选定。 分配已添加，并且不会替换所选问题中的当前分配。

         >[!TIP]
         >
         您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
         >
         如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
         >
         * 将工作项重新分配给活动资源。
         * 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

         将显示所有选定问题中通用的信息。 例如，如果将同一用户分配到所有问题，则该用户将显示在 **被分派人** 列。 如果所选问题中的信息不常见，则不会显示任何信息。

   1. 要移除单个被分配人，请执行以下操作：

      1. 单击 **X图标** 如果被分配人显示在“工作总揽”列表中，则位于要移除的被分配人名称旁。

         或

         （视情况而定）如果要删除的被分配人由于仅分配给您选择的某些问题而未显示在“工作总揽”部分中，请单击 **移除被分派人** 开始键入要删除的被分配人的名称，然后在名称出现在下拉列表中时单击该名称。

      1. 单击 **移除被分派人** 再次添加另一个被分派人以将其删除。

   1. 要删除所有现有被分配人，请执行以下操作：

      1. 单击 **移除所有现有被分配人**，然后单击 **是，删除所有被分配人**.

         这不仅会删除常见的被分配人（显示在“编辑”对话框中的被分配人），还会删除所有已选问题中的所有被分配人。

1. （可选）为您选定要与问题关联的被分配人修改以下任意选项：

   * **问题所有者：** 选择单选按钮以指明哪个被分配人被指定为“问题责任人”。 如果不选中此项，Adobe Workfront会将第一个被分配人指定为问题所有者。 这不适用于团队分配。
   * **被分派人的角色**：从下拉列表中选择一个角色。 如果保持未选中状态，Workfront将自动选择用户的主要角色。

1. 单击 **保存更改**.
