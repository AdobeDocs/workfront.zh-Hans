---
product-area: reporting
navigation-topic: reporting-elements
title: 过滤器和条件修饰符
description: 过滤器和条件修饰符允许您构建过滤器并建立条件以格式化报表结果。
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# 过滤器和条件修饰符

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

过滤器和条件修饰符允许您构建过滤器并建立条件以格式化报表结果。

有关构建过滤器的更多信息，请参阅文章 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

有关在视图中使用条件格式的更多信息，请参阅文章 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 过滤器和条件修饰符

有关内置时间范围修饰符的列表，请参阅文章 [按时间范围过滤报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

某些修饰符是内置的，您可以从过滤器或条件格式语句内的下拉菜单中选择它们。 其他修饰符只能在文本模式筛选器中使用。 有关了解文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

您可以在过滤器和条件格式语句中使用以下条件修饰符：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>内置修饰符</strong> </p> </th> 
   <th> <p><strong>文本模式修饰符</strong> </p> </th> 
   <th> <p><strong>描述</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>该字段存在于对象中，但尚未为该字段赋值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不为空白</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>要筛选的字段存在，且已赋值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>字段为空或不存在。 例如，您希望查找没有父任务ID的项目。 这意味着您只想查看独立任务。 “父任务ID”的限定符将为 <strong>null</strong>，因为没有ID的任务（在本例中为父项）不存在。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>要筛选的字段存在，且包含除null之外的其他值。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p><strong>环带</strong> </p> </td> 
   <td> <p>（不区分大小写）这是 <strong>包含</strong>. 例如：“cicontains inf”可捕获包含“Inf”或“inf”的任何值。</p> <p> <p>注意：Adobe Workfront会搜索您为每个filter语句指定的确切字词或短语。 例如，如果您正在搜索名称中包含短语“new project”的任何项目，则Workfront不会显示名称中只包含“new”或“project”或“new main project”的项目。 过滤器仅会查找名称中具有确切短语“new project”的项目。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>（不区分大小写）这是 <strong>eq</strong>. 它只返回与搜索值的完全匹配项。</p> <p>例如，在搜索具有特定名称的任务时，“任务名称cieq test”会查找名称为“Test”、“TEST”或“Test”的任务，但找不到名称为“test 123”的任务。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p>（不区分大小写）这是 <strong>in</strong>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>奇利克</strong> </p> </td> 
   <td> <p>这是不区分大小写的版本 <strong>点赞</strong>. 例如："cilike %Current% %Dead%"返回包含"Current to Dead"或"current to dead"的任何注释。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>灰黄素</strong> </p> </td> 
   <td> <p>（不区分大小写）这是 <strong>诺丁</strong>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关使用文本模式创建过滤器的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p>（区分大小写）在整个文本字符串中搜索指定的文本。</p> <p>例如，使用“包含Inf”可捕获其中包含“Inf”的任何内容，如“Infinity”一词。</p> <p>此修饰符只能在文本模式筛选器中使用。有关筛选器中文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不包含</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>（不区分大小写）用于筛选缺少指定值的项目。</p> <p>例如，“不包含inf”会捕获名称中没有“Inf”或“inf”的任何内容。</p> <p>注意： <span>如果要筛选的字段具有多个选项，则此选项会筛选出包含您指定的选项以及您指定的选项和任何其他选项的结果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>不存在</strong> </td> 
   <td><strong>笔记本</strong> </td> 
   <td> <p>此修饰符仅用于EXISTS语句中的复杂过滤器。 这些过滤器仅引用以下对象： </p> 
    <ul> 
     <li>对象层次结构中跨多个级别的对象 </li> 
     <li>缺少的对象 </li> 
    </ul> <p>有关使用EXISTS语句创建复杂过滤器的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">使用EXISTS语句创建复杂的文本模式过滤器</a>. 这是EXISTS语句中使用的唯一修饰符。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等于 (区分大小写)</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>（区分大小写）此修饰符允许您创建以逗号分隔的变量列表，以与过滤器中评估的单个属性进行比较。 整个列表将被视为OR语句，并返回符合一个或多个变量条件的任何结果。</p> <p>例如，在搜索项目时，使用“在CUR、PLN、CPL中”将返回所有处于“当前”、“或计划”或“完成”状态的项目。</p> <p>内置修饰符 <strong>等于</strong> 对应于 <strong>in</strong>. 这表示您可以为字段选择等于多个值。</p> <p>例如，您可以在项目报表中选择“状态等于当前、计划、停用”，并且可以查看处于其中任何状态的项目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>（区分大小写）这仅返回与搜索值的完全匹配项。</p> <p>例如，在搜索完整项目时，“eq CPL”会返回处于完整状态的所有项目。 “eq CPL， CUR”不会返回结果，因为项目不能同时完成且为最新项目。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关使用文本模式创建过滤器的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大于</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>这会搜索值大于输入值（不包括输入值）的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>点赞</strong> </p> </td> 
   <td> <p>（区分大小写）以与 <strong>包含</strong>. 但是， <strong>点赞</strong> 提供插入通配符以划分文本的功能。</p> <p>例如，在搜索注释时，使用“类似%Current% %Dead%”会返回任何包含“当前到无效”短语的注释。 它不包括任何包含“死到当前”的注释。 每个值会按其列出顺序进行搜索。 %表示用于替换字符或文本段的通配符。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小于</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>这会搜索值小于输入内容的所有结果，不包括输入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大于或等于</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>这会搜索值大于或等于输入值的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小于和等于</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>这会搜索值小于或等于输入值的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>介于</strong> </p> </td> 
   <td> <p><strong>介于</strong> </p> </td> 
   <td> <p>提供两个必填字段值，并搜索两个字段范围（包括输入的值）内的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>（区分大小写）用于筛选缺少指定值的项目。</p> <p>例如，“notcontains inf”会捕获任何不带“inf”的内容，但会显示包含“Inf”的值。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>这与 <strong>介于</strong>. 它提供两个必填值字段，并搜索两个字段范围外的所有结果（包括输入的值）。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不等于</strong> </p> </td> 
   <td> <p><strong>诺丁</strong> </p> </td> 
   <td> <p>（区分大小写）这与 <strong>in</strong>. 它只返回不在指定列表中的结果。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> <p>注意： <span>如果要筛选的字段具有多个选项，则此选项会筛选出包含您指定的选项以及您指定的选项和任何其他选项的结果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>（区分大小写）这与 <strong>eq</strong>. 它只返回与搜索值不完全匹配的结果，并且它也与值的大小写匹配。</p> <p>例如， <b>ne</b> 返回不等于“Current”的任何值，但不返回不等于“current”的任何值。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>（不区分大小写）这是 <strong>ne</strong> 而它与 <b>cieq</b> 修饰符。 它只返回与搜索值不完全匹配的结果，而不考虑值的大小写。</p> <p>例如， <b>cine</b> 返回不等于“current”或“Current”的任何值。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑过滤器</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
