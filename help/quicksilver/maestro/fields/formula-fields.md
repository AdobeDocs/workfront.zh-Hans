---
title: 公式字段概述
description: 在Adobe Workfront Planning中，您可以创建公式字段，这些字段使用函数和现有字段计算新的自定义值。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# 公式字段概述

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中创建自定义字段，方法是引用现有字段并通过公式连接它们。 您可以通过创建自定义公式类型字段来实现这一点。

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

有关信息，请参阅 [创建字段](../fields/create-fields.md).

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
<p>贵组织必须注册Adobe Workfront Planning测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>Workfornt计划没有访问控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## 有关公式字段的注意事项

* 公式字段引用属于同一记录类型的字段。 创建公式字段时，不能引用其他记录类型的字段。 <!--is this still accurate??-->
* 保存公式字段后，无法更改其字段类型。
* 保存公式字段后，您可以更新公式字段的计算，计算结果将自动更新相同类型的所有记录。
* 您必须添加您在公式中引用的字段，这些字段在Workfront Planning界面中显示。
* 在公式中使用链接记录类型中的查找字段将在以后可用。

## 支持的公式

Adobe Workfront Planning公式字段支持Workfront计算字段中的所有表达式。 有关更多信息，请参阅 [计算数据表达式概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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
   <td><strong>数组唯一</strong> </td> 
   <td> <p>返回具有唯一值的数组。</p> <p>表达式的格式如下所示：

<code>ARRAYUNIQUE(array)</code>
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
   <td> <p>返回一年中的周数。（可选）您可以指定星期的开始日期（使用1表示星期日，使用2表示星期一）。 如果忽略，默认情况下，周从星期日开始。</p> <p>表达式的格式如下所示：

<code>WEEKOFYEAR（日期，2）</code>
或
<code>WEEKOFYEAR（日期）</code>
</p>
   </td></tr>

</table>
