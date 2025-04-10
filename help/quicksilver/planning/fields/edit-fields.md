---
title: 编辑字段设置
description: 在Adobe Workfront Planning中，您可以编辑已创建字段的字段设置。 本文介绍了如何编辑Workfront Planning字段的设置。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: e49f1b3d9de3984ed798e20a0a0f03f9d4060115
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---


# 编辑字段设置

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以在Adobe Workfront规划中编辑现有字段的设置。

有关创建Adobe Workfront Planning字段的信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

本文介绍了如何编辑Workfront Planning字段的设置。 有关编辑记录的字段值的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

## 访问要求

+++ 展开以查看访问要求。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
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
   <td>   <p>管理工作区<!--<span class="preview">and record type</span>--> </a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 有关编辑字段设置的注意事项

在对字段配置进行更改之前，必须考虑以下事项：

* 您只能从记录类型表中编辑字段设置。
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

* 您可以从连接的记录中编辑现有查找字段。

<!--at production - April 10, 2025 - remove the last bullet altogether-->

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

   在表标题中突出显示的字段名称后面的![箭头菜单](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新有关该字段的信息并单击&#x200B;**保存**。<!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 保存字段后无法更新字段类型。
   >
   >* 修改字段配置（字段选项或公式表达式）时，已修改字段中包含信息的记录将实时更新其值。 字段配置更改触发的值更改没有警告和审核日志。 所有查看字段的用户将立即看到经过修改的新值。

   字段信息会针对每个有权查看工作区的用户而更新。

1. （视情况而定）对于连接的记录字段，单击&#x200B;**编辑查找字段**&#x200B;并从连接的记录类型中添加或删除任何查找字段。

   有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

   >[!TIP]
   >
   >您可以在连接的记录中添加或删除查找字段，但不能编辑查找字段的设置。


<!-- replace the TIP above with the one below at Preview, and remove this tip altogether after April 10 Prod release:-->

<!--
   >[!TIP]
   >
   >* In the Production environment, you can add or remove lookup fields from connected records, but you cannot edit the settings of lookup fields.
   >* <span class="preview">In the Preview environment, you can edit the settings of lookup fields.</span>

-->