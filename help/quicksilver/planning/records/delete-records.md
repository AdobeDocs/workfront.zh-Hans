---
title: 删除记录
description: 您可以删除您或其他用户创建的记录。 无法恢复已删除的记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 删除记录

{{planning-important-intro}}

您可以删除Adobe Workfront Planning中不再相关的记录。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td role="rowheader"><p>Adobe Workfront许可证</p>
   </td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>为工作区提供或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 有关删除记录的注意事项

* 您可以删除您或其他用户创建的记录。
* 无法恢复已删除的记录。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 如果删除的记录链接到其他记录，则不会删除链接的记录，但也会删除来自已删除记录的信息。
* 不能批量删除记录。 <!--this will probably change-->
* 您无法从时间线视图中删除记录。

## 删除记录

您可以从以下区域删除记录：

* [从记录的页面](#delete-a-record-from-the-records-page)
* [从记录类型的表格视图中](#delete-a-record-from-the-record-type-table-view)

### 从记录的页面中删除记录

{{step1-to-planning}}

1. 单击要删除其记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. 执行下列操作之一：

   * 在“表”视图中，单击记录的名称。
   * 在“表”视图中，将鼠标悬停在记录名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **视图**

     ![](assets/contextual-menu-for-record-row.png)
   * 在“时间轴”视图中，单击记录栏。

   此时将打开记录页面。

1. 单击 **更多** 菜单 ![](assets/more-menu.png) 记录名称的右侧，然后单击 **删除**，则 **删除** 再次确认。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
该记录已删除，无法恢复。

### 从记录类型表格视图中删除记录

{{step1-to-planning}}

1. 单击要删除其记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. （视情况而定）从 **视图** 在表左上角的下拉菜单中，选择一个“表”视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 执行下列操作之一：

   * 右键单击记录行，然后单击 **删除**.
   * 单击 **更多** 菜单 ![](assets/more-menu.png) 记录名称的右侧，然后单击 **删除**

     ![](assets/contextual-menu-for-record-row.png)

   * 单击 **打开详细信息** 图标 ![](assets/open-details-icon-in-table-name-field.png) 打开包含记录详细信息的框，然后单击 **更多** ![](assets/more-menu.png) 记录名称的右侧，然后 **删除**.

   该记录已删除，无法恢复。

1. （可选）使用以下键盘快捷键撤消或重做删除记录：

   * CTRL + Z(Mac为⌘ + Z)可撤消更改
   * 按CTRL + Shift + Z(对于Mac，按⌘ + Shift + Z)可重做更改
