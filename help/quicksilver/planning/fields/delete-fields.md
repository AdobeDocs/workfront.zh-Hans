---
title: 删除字段
description: 在Adobe Workfront Planning中，您可以删除不再相关的自定义字段。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 删除字段

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以创建自定义字段以存储有关记录的信息。

有关在Workfront Planning中创建自定义字段的信息，请参阅 [创建字段](/help/quicksilver/planning/fields/create-fields.md).

您可以删除不再相关的Workfront Planning字段。

## 有关删除Workfront Planning字段的注意事项：

* 只能删除记录类型表格视图中的字段。
* 您无法删除记录的主字段。
* 存储在字段中的任何信息都将被删除并且无法恢复。
* 删除链接记录字段时，所有链接的查找字段也会从链接来源的记录类型中删除。 您链接到的记录类型的链接记录字段不会被删除。

  有关更多信息，请参阅 [连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 删除字段

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 单击要删除其记录字段的工作区。

   此时会打开工作区，并显示记录类型。

1. 单击记录类型的卡。

1. （视情况而定）如果尚未选择，请单击 **表格视图** 在记录类型页面上。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。

1. 在列标题中查找要删除的字段，将鼠标悬停在列标题上，然后单击字段名称后的向下箭头。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 单击 **删除**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 单击 **删除** 以确认。

   该字段已删除，无法恢复，并且无法再与任何记录关联。
