---
title: 删除记录类型
description: 如果操作记录类型或分类记录类型不再相关，您可以将其删除。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# 删除记录类型

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

如果操作记录类型或分类记录类型不再相关，您可以将其删除。

有关记录类型和分类的信息，请参阅 [记录类型和分类概述](../architecture/overview-of-record-types-and-taxonomies.md).

我们建议在删除字段和记录之前，在其他记录类型上重新创建与您要删除的记录类型或分类关联的它们。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <p> Adobe Workfront</p> <p>要将Maestro记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console。</p> </td>
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
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
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

## 删除记录类型时的注意事项

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 您只能从您拥有管理权限的工作区中删除记录类型或分类。
* 删除记录类型会删除与其关联的所有信息，包括该类型的字段和记录。 记录类型将从所有访问工作区的用户中删除。
* 无法恢复已删除的记录类型或其信息。

## 删除记录类型

删除分类记录类型与删除操作记录类型相同。

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其删除记录类型的工作区。

   工作区将打开，并显示与其关联的记录类型和分类。
1. 单击要删除的记录类型或分类卡。

   这将打开记录类型的页面。
1. 单击 **更多** 菜单 ![](assets/more-menu.png) 记录类型名称的右侧，然后单击 **删除**.
1. 单击 **删除** 以确认。

   所选的记录类型或分类及其字段和关联的记录将被删除。
