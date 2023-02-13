---
product-area: projects
navigation-topic: manage-issues
title: 修改列表中多个问题的用户分配
description: 修改列表中多个问题的用户分配
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# 修改列表中多个问题的用户分配

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

您可以同时将用户分配修改为多个问题。 有关编辑问题或一次分配一个问题的信息，另请参阅以下文章：

* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [分配问题](../../../manage-work/issues/manage-issues/assign-issues.md)

有关分配问题的一般信息，请参阅 [修改问题分配概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>您必须至少拥有问题的Contribute权限才能对问题进行分配。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
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

1. 转到包含要修改其分配的问题的问题列表。
1. （可选）创建一个过滤器，以仅显示分配给您要修改的被分派人的问题。

   例如，您可以创建一个过滤器，以仅显示特定角色作为代理人的问题。 然后，您可以将角色替换为特定用户。 执行以下操作：

   1. 单击 **过滤器** 下拉列表，然后单击 **新建过滤器**.

      此时将显示“新建过滤器”对话框。

   1. 单击 **添加过滤器规则。**
   1. 要筛选特定角色，请展开 **分配角色、** 然后单击 **ID。**

      或

      要过滤特定用户，请展开 **分配用户、** 然后单击 **ID。**

      >[!TIP]
      >
      >请勿使用 **已分配给** 因为此字段仅指问题所有者，而不是所有受分配者。

   1. 在下拉列表中，选择 **等于** 作为过滤器限定符。
   1. 开始键入要筛选的用户或角色的名称，然后在下拉列表中显示该名称时单击。
   1. 单击 **保存过滤器。**

1. 选择要修改其分配的问题，然后单击 **编辑** 图标 ![](assets/qs-edit-icon.png).

   的 **编辑问题** 显示。 编辑的项目将显示在页面的左上角。

1. 转到 **分配** ，然后选择 **被分派人**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 执行下列操作之一：

   1. 要添加新的被分派人，请执行以下操作：

      1. 开始键入用户、角色或团队的名称，然后在列表中显示时选择该名称。 分配将被添加，并且不会替换选定问题上的当前分配。

         >[!TIP]
         您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
         如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
         * 将工作项重新分配给活动资源。
         * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


         将显示所有选定问题中通用的信息。 例如，如果将同一用户分配到所有问题，则该用户将显示在 **被分派人** 列。 如果所选问题中的信息不常见，则不会显示任何信息。
   1. 要删除单个受分配人，请执行以下操作：

      1. 单击 **X图标** 如果要删除的被分派人名称旁边(如果被分派人显示在“分配”(Assignments)列表中)。

         或

         （视情况而定）如果要删除的代理人未显示在“工作总揽”部分中，因为该代理人只被分配给您选择的某些问题，请单击 **删除被分派人** 然后开始键入要删除的被分派人的名称，然后在该名称出现在下拉列表中时单击该名称。

      1. 单击 **删除被分派人** 再次添加另一个被分派人以删除。
   1. 要删除所有现有受分配者，请执行以下操作：

      1. 单击 **删除所有现有的受分配人**，然后单击 **是，删除所有受分配人**.

         这不仅会删除常见的受分配人（在编辑对话框中显示的受分配人），还会删除所有选定问题上的所有受分配人。



1. （可选）为您选择与问题关联的受让人修改以下任意选项：

   * **问题所有者：** 选择单选按钮以指示将哪个代理人指定为问题责任人。 如果未选中，Adobe Workfront会将第一个代理人指定为问题所有者。 这不适用于团队分配。
   * **被分派人的角色**:从下拉列表中选择一个角色。 如果未选择，Workfront会自动选择用户的主要角色。

1. 单击 **保存更改**.
