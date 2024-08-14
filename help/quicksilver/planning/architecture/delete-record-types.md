---
title: 删除记录类型
description: 当记录类型不再相关时，您可以将其删除。 删除记录类型也会删除与记录类型关联的所有信息，如其记录、字段和视图。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# 删除记录类型

{{planning-important-intro}}

当记录类型不再相关时，您可以将其删除。

但是，删除记录类型也会删除与记录类型关联的所有信息。 有关详细信息，请参阅本文中的[删除记录类型时的注意事项](#considerations-when-deleting-record-types)部分。

有关记录类型的信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>新增：标准</p>
   <p>当前：计划</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

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

## 删除记录类型

{{step1-to-planning}}

1. 单击要删除其记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。

   此时会打开工作区，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型卡片上，单击&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**删除**。
   * 单击要删除的记录类型的卡片，然后在记录类型页面中，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**删除**。

   ![](assets/permanently-delete-record-type-confirmation.png)

1. 在确认框中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。 不区分大小写。

   所选的记录类型及其字段、关联的记录和视图将被删除并且无法恢复。
