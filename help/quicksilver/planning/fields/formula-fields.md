---
title: 公式字段概述
description: 在Adobe Workfront Planning中，您可以创建公式字段，这些字段使用函数和现有字段计算新的自定义值。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 8%

---

# 公式字段概述

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--this article is linked to the UI in the formula box, "Learn more..."-->

<!---
title: Formula fields overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中创建自定义字段，方法是引用现有字段并在公式类型字段中连接它们。

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

有关信息，请参阅文章[创建字段](/help/quicksilver/planning/fields/create-fields.md)中的“公式”部分。

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
   <td> <p>Workfornt计划没有访问控制</p>  
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

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## 有关公式字段的注意事项

* 公式字段引用属于同一记录类型的字段。 创建公式字段时，不能引用其他记录类型的字段。<!--is this still accurate??-->
* 保存公式字段后，无法更改其字段类型。
* 保存公式字段后，您可以更新公式字段的计算，计算结果将自动更新相同类型的所有记录。
* 您必须添加您在公式中引用的字段，这些字段在Workfront Planning界面中显示。
<!--* You can format the result of a formula calculation by choosing from the following options:

   * Text
   * Number
   * Percent
   * Currency
   * Tags
   * Date

   For more information, see the "Formula" section in the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). -->


## 支持的公式

Adobe Workfront Planning公式字段支持Workfront计算字段中的所有表达式。 有关详细信息，请参阅[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

此外，我们为Workfront Planning公式字段支持以下表达式：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>表达式</th> 
   <th>说明和示例</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>按分隔符返回连接字符串。</p> <p>表达式的格式如下所示：

<code>ARRAYJOIN（分隔符，数组）</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>返回具有唯一值的数组。</p> <p>表达式的格式如下所示：

<code>ARRAYUNIQUE（数组）</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>返回记录的ID。 每个记录都有一个唯一的ID。</p> <p>表达式的格式如下所示：

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>将日期和时间的时区设置为特定时区。</p> <p>表达式的格式如下所示：

<code>SETTIMEZONE（日期，&#39;美洲/洛杉矶&#39;）</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>返回一年中的周数。（可选）您可以指定一周从哪一天开始（使用 1 表示星期日，或使用 2 表示星期一）。如果省略，则默认为一周从星期日开始。</p> <p>表达式的格式如下所示：

<code>WEEKOFYEAR（日期，2）</code>
或
<code>WEEKOFYEAR（日期）</code>
</p>
   </td></tr>

</table>
