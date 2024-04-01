---
title: 创建分类记录类型
description: 使用模板创建工作区时，会在“操作记录类型”和“分类”部分中创建记录类型。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 创建分类记录类型

{{maestro-important-intro}}

使用模板创建工作区时，会在以下部分中创建记录类型：

* 操作记录类型
* 分类标准

工作区的“分类”部分中的记录类型捕获了同一工作区的“操作记录类型”部分中有关记录类型的属性。

例如，Campaign可以是操作记录类型。 以下是捕获有关Campaign记录类型的属性的分类：地区、受众、国家/地区。

有关记录类型的详细信息，请参阅 [记录类型概览](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>要将记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区
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

* 必须先使用模板创建工作区，然后才能在工作区的“分类”部分中创建记录类型。

  有关工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).
* 通过执行以下操作之一，可在工作区的“分类”部分中创建记录类型：
   * 在使用模板创建工作区时自动创建它们。 有关信息，请参阅 [创建工作区](../architecture/create-workspaces.md).
   * 在工作区的“分类”部分中从头开始手动创建分类。

* 默认情况下，所有新创建的分类都有以下字段：

   * 名称
   * 描述
   * 开始日期
   * 结束日期
   * 状态

  此外，您还可以将自定义字段添加到分类。 有关更多信息，请参阅 [创建字段](../fields/create-fields.md).

  >[!NOTE]
  >
  >    使用工作区模板时创建的分类记录类型具有其他字段。

## 创建分类记录类型

创建分类记录类型与创建记录类型类似。

有关信息，请参阅 [创建记录类型](../architecture/create-record-types.md).
