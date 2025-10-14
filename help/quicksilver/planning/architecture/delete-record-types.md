---
title: 删除记录类型
description: 当记录类型不再相关时，您可以将其删除。 删除记录类型也会删除与记录类型关联的所有信息，如其记录、字段和视图。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---


<!--keep the global record type reference in yellow till January 2026-->

# 删除记录类型

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

当记录类型不再相关时，您可以将其删除。

但是，删除记录类型也会删除与记录类型关联的所有信息。 有关详细信息，请参阅本文中的[删除记录类型时的注意事项](#considerations-when-deleting-record-types)部分。

有关记录类型的信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## 访问要求

+++ 展开以查看访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区和记录类型的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p></td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


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

<!--

<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 
   
   You must first delete it from the secondary workspaces where it's been added, before you can delete it from its original workspace. 

   Deleting a global record type from their secondary workspaces only remove them, their records, and that workspace's fields from the secondary workspace. It does not delete the global record type from its original workspace.

   For information, see the section "Delete a global record type from a secondary workspace" in the article [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

</div>
-->

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

   <!--[!TIP]
   >
   ><span class="preview">You cannot delete global record types added to other workspaces. First, delete the global record types form their secondary workspaces before deleting them from the original workspace.</span>-->


1. 在确认框中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。 不区分大小写。

   所选的记录类型及其字段、关联的记录和视图将被删除并且无法恢复。


