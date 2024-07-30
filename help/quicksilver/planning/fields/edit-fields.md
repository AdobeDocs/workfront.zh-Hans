---
title: 编辑字段设置
description: 在Adobe Workfront Planning中，您可以编辑已创建字段的字段设置。 本文介绍了如何编辑Workfront Planning字段的设置。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 编辑字段设置

{{planning-important-intro}}

您可以编辑已在Adobe Workfront Planning中创建的字段的字段设置。

有关创建Adobe Workfront Planning字段的信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

本文介绍了如何编辑Workfront Planning字段的设置。 有关编辑记录的字段值的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

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
   <td> <p>Workfront Planning没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 有关编辑字段设置的注意事项

在对字段配置进行更改之前，必须考虑以下事项：

* 如果您对字段所属的工作区具有管理权限，则可以编辑您创建的字段或其他用户创建的字段。
* 您可以在记录类型表中编辑字段。
* 不能在记录页面或表格视图之外的任何其他视图中编辑字段。
* 保存字段后，您无法编辑字段类型。
* 如果附加到“数字”、“百分比”或“货币”字段的记录中已经存储了负值，则不能取消选择以前选择的“允许负数”设置。
* 保存字段后，可以编辑以下字段元素的配置：

   * 任何字段的名称或描述
   * 单选或多选字段的选项。
   * “公式”字段的表达式。

  >[!WARNING]
  >
  >当公式表达式发生更改，或者在select-type字段中添加或删除选项时，如果记录中已存储信息且这些信息的字段修改了配置，则这些记录的数据将会丢失。
  >
  >在更改字段配置时，没有警告或指示可能发生此数据丢失。
  >
  >不会通知其他用户字段配置已更改。

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## 编辑字段设置

{{step1-to-planning}}

1. 单击要编辑其记录字段的工作区。

   工作区将打开，工作区中的所有记录类型都显示在信息卡上。

1. 单击记录类型的卡。

   这将打开记录类型的页面。

1. （视情况而定）单击&#x200B;**表视图**&#x200B;的选项卡。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。
1. 将鼠标悬停在要编辑的字段的列标题上，单击字段名称后面的向下箭头，然后单击“**编辑字段**”

   或

   双击该字段的列标题。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新有关该字段的信息并单击&#x200B;**保存**。<!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 保存字段后无法更新字段类型。
   >
   >* 修改字段配置（字段选项或公式表达式）时，已修改字段中包含信息的记录将实时更新其值。 字段配置更改触发的值更改没有警告和审核日志。 所有查看字段的用户将立即看到经过修改的新值。

   字段信息会针对每个有权查看工作区的用户而更新。

1. （视情况而定）对于链接的记录字段，单击&#x200B;**编辑查找字段**&#x200B;并从链接的记录类型中添加或删除任何字段。

   有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

