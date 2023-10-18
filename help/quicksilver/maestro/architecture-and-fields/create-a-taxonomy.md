---
title: 创建分类记录类型
description: 分类是一种可重用的记录类型，可捕获Adobe Workfront Maestro中某个运营记录类型的相关属性。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 创建分类记录类型

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe公司推出的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

分类是记录类型，用于捕获AdobeMaestro中有关操作记录类型的属性。

例如，Campaign可以是操作记录类型。 以下是捕获有关Campaign记录类型的属性的分类：地区、受众、国家/地区。

有关Maestro记录类型的详细信息，请参阅 [记录类型和分类概述](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## 有关创建分类的注意事项

* 必须先创建工作区，然后才能在该工作区中创建分类。

  有关工作区的信息，请参见 [创建工作区](../architecture-and-fields/create-workspaces.md).
* 通过执行以下操作之一，可以创建分类记录类型：
   * 在使用模板创建工作区时自动创建它们。 有关信息，请参阅 [创建工作区](../architecture-and-fields/create-workspaces.md).
   * 从头开始手动创建它们。
   * 通过从外部列表中粘贴信息，手动创建它们。

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* 所有新创建的分类都包含以下字段：

   * 名称 <!--if there won't be any more fields, consider rephrasing this-->

  此外，您还可以将自定义字段添加到分类。 有关更多信息，请参阅 [创建字段](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    使用工作区模板时创建的分类具有其他字段。

## 创建分类

创建分类与从头开始或从工作区模板创建操作记录类型类似。

有关信息，请参阅文章中的“从头开始创建记录类型”部分 [创建记录类型](../architecture-and-fields/create-record-types.md).

有关在从模板创建工作区时自动创建分类的信息，请参阅 [创建工作区](../architecture-and-fields/create-workspaces.md).
