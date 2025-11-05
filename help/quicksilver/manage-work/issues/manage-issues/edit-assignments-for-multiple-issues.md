---
product-area: projects
navigation-topic: manage-issues
title: 修改列表中多个问题的用户分配
description: 修改列表中多个问题的用户分配
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 1%

---

# 修改列表中多个问题的用户分配

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<div class="preview">

此页面上高亮显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 从“预览”版本开始的一周后，生产环境中所有客户也可以使用相同的功能。

有关详细信息，请参阅[接口现代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

</div>

您可以同时将用户分配修改为多个问题。 有关编辑问题或一次分配一个问题的信息，另请参阅以下文章：

* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [分配问题](../../../manage-work/issues/manage-issues/assign-issues.md)

有关分配问题的一般信息，请参阅[修改问题分配的概述](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)。

>[!NOTE]
>
>您必须至少具有问题的Contribute权限，才能为该问题分配工作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务以分配一个问题</p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>管理问题的权限</p> <p>分配多个问题时，向问题所在的项目或任务分配Contribute权限或更高。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多个问题的分配

1. 转到问题列表，其中包含要修改其分配的问题。
1. （可选）创建一个过滤器，以仅显示分配给要修改的被分派人的问题。

   例如，您可以创建一个过滤器，以仅显示具有作为被分配人的特定角色的问题。  然后，您可以使用特定用户替换角色。 执行以下操作：

   1. 单击&#x200B;**筛选器**&#x200B;下拉列表，然后单击&#x200B;**新建筛选器**。

   1. 在第一个字段中，开始键入&#x200B;**任务角色**，然后从列表中选择&#x200B;**任务角色：名称**。
   1. 从修饰符下拉菜单中选择&#x200B;**是**&#x200B;的任一项，然后开始键入角色的名称，并在角色显示在列表中时将其选定。 您可以键入多个角色。

      >[!TIP]
      >
      >不要使用&#x200B;**分配给**，因为此字段仅引用问题所有者，而不引用所有被分配人。

      问题列表会自动根据您的筛选条件进行筛选。
   1. （可选）单击&#x200B;**另存为新项**，然后单击&#x200B;**保存**。

1. 选择要修改分配的问题，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/qs-edit-icon.png)。

   此时将显示&#x200B;**编辑问题**。 所选的项目数显示在页面的左上角。

1. （视情况而定）在生产环境中，执行以下操作：

   1. 转到&#x200B;**工作**&#x200B;部分，然后选择&#x200B;**代理人**。

      ![工作区域](assets/classic-assignmens-area-on-edit-box-350x119.png)

   1. 执行下列操作之一：

      1. 要添加新的被分派人，请执行以下操作：

         1. 开始键入用户、角色或团队的名称，然后在该名称显示在列表中时将其选定。 分配已添加，并且不会替换所选问题中的当前分配。

         >[!TIP]
         >
         >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
         >
         >如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
         >
         >* 将工作项重新分配给活动资源。
         >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

         将显示所有选定问题中通用的信息。 例如，如果将同一用户分配到所有问题，则该用户会显示在&#x200B;**被分派人**&#x200B;列中。 如果所选问题中的信息不常见，则不会显示任何信息。

      1. 要移除单个被分配人，请执行以下操作：

         1. 如果被分派人显示在“工作总揽”列表中，则单击要删除的被分派人名称旁边的&#x200B;**X图标**。

            或

            如果要删除的被分配人由于仅分配给您选择的某些问题而未显示在“工作总揽”部分中，请单击“删除被分配人”**&#x200B;**，然后开始键入要删除的被分配人的名称，然后在该名称出现在下拉列表中时单击该名称。

         1. 再次单击&#x200B;**移除被分派人**&#x200B;以添加另一个要移除的被分派人。

      1. 要删除所有现有被分配人，请执行以下操作：

         1. 单击&#x200B;**删除所有现有被分配人**，然后单击&#x200B;**是，删除所有被分配人**。

            这不仅会删除常见的被分配人（显示在“编辑”对话框中的被分配人），还会删除所有已选问题中的所有被分配人。

         1. （可选）为您选定要与问题关联的被分配人修改以下任意选项：

            * **问题所有者：**&#x200B;选择单选按钮以指示哪个被分配者被指定为问题所有者。 如果不选中此项，Adobe Workfront会将第一个被分配人指定为问题所有者。 这不适用于团队分配。
            * **被分派人的角色**：从下拉列表中选择一个角色。 如果保持未选中状态，Workfront将自动选择用户的主要角色。

      1. 单击&#x200B;**保存更改**。

1. <span class="preview">在“预览”环境中，执行以下操作：</span>

   1. <span class="preview">单击左侧面板中的&#x200B;**工作**，然后单击要删除的工作负责人旁边的&#x200B;**x**&#x200B;图标。</span>

      >[!TIP]
      >
      ><span class="preview">只有分配到所有选定问题的被分配者才会显示在&#x200B;**工作总揽**&#x200B;区域。</span>

      ![批量编辑问题中的分配区域](assets/assignments-area-on-bulk-edit-issues.png)

   1. <span class="preview">开始键入用户、角色或团队的名称，以将受分配人添加到所有已选问题。</span>

      >[!TIP]
      >
      >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
      >
      >如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
      >
      >* 将工作项重新分配给活动资源。
      >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

      <span class="preview">添加的被分配人已添加到现有被分配人。 它们不会替换每个选定问题的现有问题。</span>
   1. <span class="preview">（可选）单击&#x200B;**分配给我**&#x200B;以将所有问题分配给您自己。</span>
   1. <span class="preview">单击&#x200B;**保存**。</span>




