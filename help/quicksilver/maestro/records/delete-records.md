---
title: 删除记录
description: 您可以删除您或其他用户创建的记录。 无法恢复已删除的记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 删除记录

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

您可以删除Adobe大师中不再相关的记录。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关删除记录的注意事项

* 您可以删除您或其他用户创建的记录。
* 无法恢复已删除的记录。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 如果删除的记录链接到其他记录，则不会删除链接的记录，但也会删除来自已删除记录的信息。
* 不能批量删除记录。 <!--this will probably change-->
* 您无法从时间线视图中删除记录。

## 删除记录

您可以从以下区域删除记录：

* [从记录的详细信息页面](#delete-a-record-from-the-records-details-page)
* [从记录类型的表格视图中](#delete-a-record-from-the-record-type-table-view)

### 从记录的“详细信息”页面中删除记录

1. 单击 **主菜单** ![](assets/main-menu-workfront.png) 位于右上角，或 **主菜单** ![](assets/main-menu-shell.png) 如果左上角可用，请单击Maestro。

   您上次访问的工作区将打开。
1. 单击记录类型。

   此时将打开记录类型页面。
1. 执行下列操作之一：

   * 在“表”视图中，单击记录的名称。
   * 在“表”视图中，将鼠标悬停在记录名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **视图**

     ![](assets/contextual-menu-for-record-row.png)
   * 在“时间轴”视图中，单击记录栏。

   记录 **详细信息** 页面将打开。

1. 单击 **更多** 菜单 ![](assets/more-menu.png) 记录名称的右侧，然后单击 **删除**，则 **删除** 再次确认。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
该记录已删除，无法恢复。

### 从记录类型表格视图中删除记录

1. 单击 **主菜单** ![](assets/main-menu-workfront.png) 位于右上角，或 **主菜单** ![](assets/main-menu-shell.png) （如果可用），然后单击 **大师**.

   您上次访问的工作区随即打开。
1. 单击记录类型。

   此时将打开记录类型页面。
1. （视情况而定）从 **视图** 在表右上角的下拉菜单中，选择一个“表”视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 右键单击记录行，然后单击 **删除**.

   ![](assets/contextual-menu-for-record-row.png)

   该记录已删除，无法恢复。
