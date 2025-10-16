---
title: 删除记录类型
description: 当记录类型不再相关时，您可以将其删除。 删除记录类型也会删除与记录类型关联的所有信息，如其记录、字段和视图。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# 删除记录类型

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

当记录类型不再相关时，您可以将其删除。

但是，删除记录类型也会删除与记录类型关联的所有信息。 有关详细信息，请参阅本文中的[删除记录类型时的注意事项](#considerations-when-deleting-record-types)部分。

有关记录类型的信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning包</p></li>
<p>或</p>
<li><p>任何工作流和任何计划包</p></li></ul>
<div class="preview">
<p>要删除全局记录类型，请执行以下操作：</p>
<ul><li><p>任何Workfront包和Planning Plus包</p></li>
<p>或</p>
<li><p>任何工作流和计划Prime或Ultimate包</p></li></ul>
</div>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## 删除记录类型时的注意事项

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 您只能从具有“管理”权限的工作区中删除记录类型。
* 删除记录类型将删除与其关联的以下信息：

   * 该类型的所有记录。
   * 与记录类型关联的所有字段。
   * 记录类型的所有视图（包括筛选器、分组和排序标准）。
* 记录类型将从所有访问工作区的用户中删除。
* 无法恢复已删除的记录类型或其信息。
* 我们建议在删除字段和记录之前，在其他记录类型上重新创建与要删除的记录类型关联的它们。

<div class="preview">

* 您无法删除已添加到其他工作区的全局记录类型。

  有关详细信息，请参阅本文中的[删除全局记录类型](#delete-global-record-types)部分。

</div>

## 删除记录类型

{{step1-to-planning}}

1. 单击要删除其记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。

   此时会打开工作区，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型卡片上，单击&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**删除**。
   * 单击要删除的记录类型的卡片，然后在记录类型页面中，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**删除**。

   ![永久删除记录类型确认](assets/permanently-delete-record-type-confirmation.png)


1. 在确认框中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。 不区分大小写。

   所选的记录类型及其字段、关联的记录和视图将被删除并且无法恢复。

<div class="preview">

## 删除全局记录类型

删除全局记录类型时存在以下情况：

* 如果配置为全局的记录类型尚未添加到另一个工作区，则可以从其原始工作区中删除它。

* 如果配置为全局记录类型的记录类型已添加到至少一个其他工作区，则不能将其从原始工作区中删除。 首先，必须从添加全局记录类型的辅助工作区中删除（通过删除）全局记录类型，然后才能从其原始工作区中永久删除全局记录类型。

### 从原始工作区中删除全局记录类型

如果记录类型不再相关，您可以将其从原始工作区中删除。

1. 转到其原始工作区中的全局记录类型。

1. （视情况而定）根据是否将全局记录类型添加到辅助工作区，执行以下操作之一：

   * 如果记录类型未添加到辅助工作区，请单击记录类型卡片上的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或该记录类型在其页面上的名称右侧，然后单击&#x200B;**删除**。
   * 如果记录类型已添加到至少一个其他辅助工作区，请先转到辅助工作区并从该工作区中删除全局记录。

     有关信息，请参阅本文中的[从辅助工作区中删除全局记录类型](#delete-a-global-record-type-from-a-secondary-workspace)部分。

1. （视情况而定）继续删除记录类型，如本文中的[删除记录类型](#delete-record-types-1)部分所述。

   出现以下情况：

   * 全局记录类型将从原始工作区中删除，并且无法恢复该记录类型、其记录和字段。
   * 辅助工作区中的所有全局记录类型及其记录也将被删除。

### 从辅助工作区中删除全局记录类型

如果不再需要某个记录类型，您可以将其从另一个工作区中删除。

请考虑以下事项：

* 从辅助工作区中删除全局记录类型只会将其从辅助工作区中删除。 记录类型仍保留在原始工作区中。

* 从辅助工作区中删除全局记录类型时，也会删除以下内容：

   * 从辅助工作区添加的记录。

  <!--Coming later: * The fields added from the secondary workspace.-->

* 无法恢复从其辅助工作区中删除的全局记录类型。

* 原始记录类型会保留在其原始工作区中，以及已添加该记录的其他工作区中。

要从辅助工作区中删除全局记录类型，请执行以下操作：

1. 转到辅助工作区中的全局记录类型。

1. （可选）单击记录类型卡片上的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或记录类型名称页面右侧，然后单击&#x200B;**删除**。
1. （视情况而定）在提供的字段中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。

   ![删除辅助全局记录类型确认框](assets/delete-secondary-global-record-type.png)

   出现以下情况：

   * 从所选工作区中删除从全局记录类型创建的记录类型。
   * 原始记录类型及其字段保留在其原始工作区中。
   * 记录类型将保留在添加该记录的所有其他工作区中。
   * 删除从当前工作区添加到记录类型的记录<!--and fields-->。 从添加全局记录类型的附加工作区中添加的所有其他记录将保留在各自的工作区和原始工作区中。 &lt;！ — 字段保留在添加它们的工作区中。

</div>
