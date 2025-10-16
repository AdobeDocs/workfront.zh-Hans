---
title: 公式字段概述
description: 在Adobe Workfront Planning中，您可以创建公式字段，这些字段使用函数和现有字段计算新的自定义值。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 5%

---

# 公式字段概述

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中创建自定义字段，方法是引用现有字段并在公式类型字段中连接它们。

公式字段使用记录类型中其他字段的现有值以及指示应如何计算现有值的函数来生成新值。

有关信息，请参阅文章[创建字段](/help/quicksilver/planning/fields/create-fields.md)中的“公式”部分。

<!--do we need these for an overview article?

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and any Planning package</p>
<p>Any Workflow and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

-->

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## 有关公式字段的注意事项

* 公式字段引用属于同一记录类型的字段。
* 仅当将其他记录类型连接到要为其创建公式字段的记录类型时，才能引用其他记录类型的字段。
* 在公式中引用连接的记录类型或其查找字段取决于您对连接的记录类型的权限。 如果您无权查看记录类型，则无法在公式中引用其字段。
* 保存公式字段后，无法更改其字段类型。
* 保存公式字段后，您可以更新公式字段的计算，计算结果将自动更新相同类型的所有记录。
* 您必须添加您在公式中引用的字段，这些字段在Workfront Planning界面中显示。
* 您只能引用在记录类型的表视图或记录详细信息页面中显示的字段。
* 通过从以下格式选项中进行选择，可以定义公式计算值的格式：

   * 文本
   * 数值
   * 百分比
   * 货币
   * 标记
   * 日期

  有关详细信息，请参阅文章[创建字段](/help/quicksilver/planning/fields/create-fields.md)中的“公式”部分。
* 您可以在新的公式中引用公式字段。 一旦在公式字段中引用的字段中更新了值，引用该字段的所有后续字段或包含该字段的公式字段将自动更新。

* 当您更新公式字段或可能影响该字段的字段时，警报会通知您更改的影响。 警报在以下情况下显示：

   * 当更新公式字段（不包括名称和说明更改）时，如果该字段具有从属公式或查找字段。 警报会列出这些依赖字段，并询问您是否要继续。

   * 删除在公式表达式中或用作查找字段的字段时。 警报会列出相关公式和查找字段，并询问您是否要继续删除。

## 公式字段的限制

* 您最多可以为一个记录类型添加20个公式字段。

  从连接的记录类型添加的公式查找字段不计入此限制。

* 公式表达式不能超过50,000个字符。

* 在以下情况下，公式字段可能显示为`#ERROR!`：
   * 删除公式中使用的字段时。
   * 当聚合查找字段中使用的字段显示为`#ERROR!`时。

     例如，如果您显示的查找字段包含汇总查找公式字段，并且其中一个引用的公式字段显示为`#ERROR!`。
   * 当公式值无法以所选格式显示时。

     例如，如果我为公式字段的格式选择数字，并且公式中使用的字段是只显示非数字文本值的文本字段，则公式结果将显示为`#ERROR!`，因为它无法将文本解析为数字。


## 支持的公式

Adobe Workfront Planning公式字段支持Workfront计算字段中的大多数表达式。

>[!NOTE]
>
>Workfront Planning公式字段不支持以下Workfront表达式：
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* 格式

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

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
