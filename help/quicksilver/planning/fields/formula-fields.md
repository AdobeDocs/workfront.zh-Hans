---
title: 公式字段概述
description: 在Adobe Workfront Planning中，您可以创建公式字段，这些字段使用函数和现有字段计算新的自定义值。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 7%

---

# 公式字段概述

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中创建自定义字段，方法是引用现有字段并在公式类型字段中连接它们。

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

有关信息，请参阅文章[创建字段](/help/quicksilver/planning/fields/create-fields.md)中的“公式”部分。

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
   <td><p> 标准</p>
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
   <td>   <p>管理工作区<span class="preview">和记录类型</span> </a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning的布局模板。</p>
<p><span class="preview">在“预览”环境中，标准用户和系统管理员默认启用Planning。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关公式字段的注意事项

* 公式字段引用属于同一记录类型的字段。
* 仅当将其他记录类型连接到要为其创建公式字段的记录类型时，才能引用其他记录类型的字段。
* 保存公式字段后，无法更改其字段类型。
* 保存公式字段后，您可以更新公式字段的计算，计算结果将自动更新相同类型的所有记录。
* 您必须添加您在公式中引用的字段，这些字段在Workfront Planning界面中显示。
* 您只能引用在记录类型的表视图或记录详细信息页面中显示的字段。
* 通过从以下格式选项中进行选择，可以定义公式计算值的格式：

   * 文本
   * 数字
   * 百分比
   * 货币
   * 标记
   * 日期

  有关详细信息，请参阅文章[创建字段](/help/quicksilver/planning/fields/create-fields.md)中的“公式”部分。

## 支持的公式

Adobe Workfront Planning公式字段支持Workfront计算字段中的大多数表达式。

>[!NOTE]
>
>Workfront Planning公式字段不支持以下Workfront表达式：
>
>* SORTASCARRAY
>* SORTDESCARRAY
>* ADDHOUR
>* SWITCH
>* 格式


有关Workfront表达式的完整列表，请参阅[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

此外，我们为Workfront Planning公式字段支持以下表达式。 Workfront表达式不支持以下表达式：

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

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
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>通过提供的JSONPath从JSON返回数据。 如果JSON中不存在JSONPath，则将返回空结果。 </p> <p>表达式的格式如下所示：
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
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
