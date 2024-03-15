---
product-area: reporting
navigation-topic: reporting-elements
title: 过滤器和条件修饰符
description: 利用过滤器和条件修饰符，可构建过滤器并建立用于格式化报表结果的条件。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 0%

---

# 过滤器和条件修饰符

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

利用过滤器和条件修饰符，可构建过滤器并建立用于格式化报表结果的条件。

有关构建过滤器的更多信息，请参阅文章 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

有关在视图中使用条件格式的详细信息，请参阅文章 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 过滤器和条件修饰符

某些修饰符是内置的，您可以从筛选器或条件格式语句中的下拉菜单中选择它们。 其他修饰符只能在文本模式过滤器中使用。

有关了解文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

有关内置时间范围修饰符的列表，请参阅文章 [按时间范围筛选报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p><strong>为空</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>对象存在该字段，但该字段当前没有值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不为空</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>您正在筛选的字段已存在并已获得一个值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>该字段为空或不存在。 例如，您要查找没有父任务ID的项目。 这意味着您只想查看独立任务。 “父任务ID”的限定符将为 <strong>null</strong>，因为没有ID的任务（在本例中是父任务）不存在。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>您正在筛选的字段存在，并包含非空值。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p><strong>菊花</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 版本 <strong>包含</strong>. 例如： <code>cicontains inf</code> 捕获包含以下任意值的任何值： <code>Inf</code> 或 <code>inf</code>.</p> <p> <p>注意：Adobe Workfront将搜索您为每个过滤语句指定的确切单词或短语。 例如，如果要搜索包含短语的任何项目 <code>new project</code> 在名称中，Workfront不显示仅具有 <code>new</code> 或只是 <code>project</code>，或 <code>new main project</code> 在名称中。 该过滤器仅查找包含精确短语的项目 <code>new project</code> 在名称中。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不包含</strong> </p> </td> 
   <td> <p><strong>肉桂含有</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 版本 <strong>notcontains</strong>.</p><p>此修饰符用于筛选缺少指定值的项目。</p> <p>例如， <code>does not contain inf</code> 捕获任何内容，而不是 <code>Inf</code> 或 <code>inf</code> 在名称中。</p> <p>注意： <span>如果要过滤的字段有多个选项，则过滤掉包含指定选项、指定选项和任何其他选项的结果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p> 搜索指定的 <i>区分大小写</i> 整个文本字符串中的文本。</p> <p>例如，使用 <code>contains Inf</code> 通过以下方式捕获任何内容 <code>Inf</code> 其中，例如单词 <code>Infinity.</code></p> <p>此修饰符只能在文本模式筛选器中使用。有关筛选器中文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>它会筛选缺少以下内容的项目： <i>区分大小写</i> 指定值。</p> <p>例如， <code>notcontains inf</code> 捕获任何内容，而不是 <code>inf</code>，但显示的值包含 <code>Inf</code>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 选项 <strong>eq</strong>. 它仅返回与搜索值完全匹配的值。</p> <p>例如，当搜索具有特定名称的任务时， <code>task name cieq test</code> 查找名称为的任务 <code>Test</code>， <code>TEST</code>，或 <code>Test</code>，但未找到名为的任务 <code>test 123.</code></p> <p>搜索状态时， <strong>cieq</strong> 不支持修饰符。 您应使用区分大小写的修饰符， <strong>eq</strong>，以搜索状态。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>电影</strong> </td> 
   <td> <p>这是 <i>区分大小写</i> 选项 <strong>ne</strong>，并且它与 <b>cieq</b> 修饰符。 它只返回与搜索的值不完全匹配的结果，不考虑值的大小写。</p> <p>例如， <b>电影</b> 返回不等于“current”或“Current”的任何值。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>此修饰符仅返回一个精确值， <i>区分大小写</i> 搜索值的匹配项。</p> <p>例如，在搜索完整项目时， <code>eq CPL</code> 返回所有处于完成状态的项目。 <code>eq CPL, CUR</code> 不返回结果，因为某个项目不能同时完整且为当前项目。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>这是 <i>区分大小写</i> 反向 <strong>eq</strong>. 它仅返回与搜索的值不完全匹配的结果，并且与值的大小写也匹配。</p> <p>例如， <b>ne</b> 返回不等于“Current”的任何值，但不会返回不等于“current”的任何值。 </p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> 这是 <i>区分大小写</i> 版本 <strong>在</strong>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>香茅素</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 版本 <strong>notin</strong>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等于</strong> </p> </td> 
   <td> <p><strong>在</strong> </p> </td> 
   <td> <p>此修饰符允许您创建以逗号分隔的 <i>区分大小写</i> 变量进行比较，以与在筛选器中计算的单个属性进行比较。 整个列表将被视为OR语句，并返回符合一个或多个变量标准的任何结果。</p> <p>例如，在搜索项目时，使用 <code>in CUR, PLN, CPL</code> 返回所有处于“当前”、“OR计划”或“完成”状态的项目。</p> <p>内置修饰符 <strong>等于</strong> 与的文本模式修饰符相对应 <strong>在</strong>. 这意味着可以为字段选择等于多个值。</p> <p>例如，您可以在项目报表中选择“状态等于当前、计划、终止”，并且您可以查看处于其中任一状态的项目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不等于</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 反向 <strong>在</strong>. 它只返回不在指定列表中的结果。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> <p>注意： <span>如果要过滤的字段有多个选项，则过滤掉包含指定选项、指定选项和任何其他选项的结果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>这是 <i>区分大小写</i> 版本 <strong>点赞</strong>. 例如： <code>cilike %Current% %Dead%</code> 返回包含的任何注释 <code>Current to Dead</code> 或 <code>current to dead</code>.</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>点赞</strong> </p> </td> 
   <td> <p>此修饰符搜索 <i>区分大小写</i> 与类似的文本字符串 <strong>包含</strong>. 但是， <strong>点赞</strong> 提供插入通配符以分解文本的功能。</p> <p>例如，在搜索注释时，使用 <code>like %Current% %Dead%</code> 返回包含短语“Current to Dead”的任何注释。 它不包括任何包含“Dead to Current”的注释。 每个值都将按其列出的顺序进行搜索。 %表示用于替换文本字符或区段的通配符。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>不存在</strong> </td> 
   <td><strong>无文本主义者</strong> </td> 
   <td> <p>此修饰符仅用于EXISTS语句中的复杂过滤器。 这些过滤器仅引用以下对象： </p> 
    <ul> 
     <li>对象层次结构中跨多个级别的对象 </li> 
     <li>缺少的对象 </li> 
    </ul> <p>有关使用EXISTS语句创建复杂过滤器的信息，请参阅本文 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">使用EXISTS语句创建复杂的文本模式筛选器</a>. 这是EXISTS语句中使用的唯一修饰符。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大于</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>这将搜索其值大于输入值（不包括输入值）的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小于</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>这将搜索其值小于输入值的所有结果，不包括输入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大于或等于</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>这将搜索其值大于或等于输入值的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小于或等于</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>这将搜索其值小于或等于输入值的所有结果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>介于</strong> </p> </td> 
   <td> <p><strong>介于</strong> </p> </td> 
   <td> <p>提供两个必填字段值，并搜索两个字段范围内的所有结果，包括输入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>这与 <strong>介于</strong>. 它提供两个必填值字段，并搜索两个字段（包括输入的值）范围以外的所有结果。</p> <p>此修饰符只能在文本模式过滤器中使用。 有关过滤器中的文本模式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文本模式编辑筛选器</a>.</p> </td> 
  </tr>

</tbody> 
</table>
