---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式编辑筛选器
description: 您可以使用文本模式在列表或报告中编辑过滤器，以访问标准界面中不可用的字段，并创建更复杂的过滤器。
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# 使用文本模式编辑筛选器

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

您可以使用文本模式在列表或报告中编辑过滤器，以访问标准界面中不可用的字段，并创建更复杂的过滤器。

有关创建筛选器时的更多文本模式示例，另请参阅文章[自定义视图、筛选器和分组示例：文章索引](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)中的[自定义筛选器的示例](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters)部分。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
    <p>或</p>
    <p>当前：计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对筛选器、视图和分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的报告元素</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以编辑报告中的筛选器</p> <p>管理筛选器权限以编辑它</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在报表或列表中开始使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在筛选器中编辑文本模式

对于报告和列表，使用文本模式编辑过滤器是相同的。 从报表或列表访问过滤器有所不同。

>[!TIP]
>
>我们建议您在标准模式下构建尽可能多的过滤器，然后将过滤器转换为文本模式以进行编辑。

有关生成筛选器的详细信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

有关创建报告的信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 执行下列操作之一：

   1. 若要从报表访问筛选器，请转到该报表，然后单击&#x200B;**报表操作** > **编辑** > **筛选器**&#x200B;选项卡。
   1. 要从列表中访问筛选器，请转到该列表，然后从&#x200B;**筛选器**&#x200B;菜单中，将鼠标悬停在要修改的筛选器上，然后单击&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。

      此时将打开过滤器生成器。

1. 单击&#x200B;**添加筛选器规则**&#x200B;开始添加筛选条件，然后单击生成器右侧的&#x200B;**文本模式**&#x200B;或&#x200B;**切换到文本模式**。
1. 使用文本模式添加过滤器语句。 每个过滤语句可以包含以下行和其他信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>过滤行/信息</b></td> 
      <td><b>示例</b></td> 
     </tr> 
     <tr> 
      <td> <p>字段名称及其在Workfront数据库中显示的值。</p> <p>此行是必填的。</p> <p> 有关对象和字段如何在数据库中显示的详细信息，请参阅<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API资源管理器</a>。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>要筛选状态为“进行中”的任务，请使用以下行：</p> <p><code>status=INP</code> </p> <p><b>提示</b>

   筛选状态时，必须使用三个字母的状态代码，而不是名称。</p> </td>
   </tr> 
     <tr> 
      <td> <p>字段名称修饰符以及修饰符所代表的内容。 这指示作为筛选依据的字段必须满足哪些条件。</p> <p>此行是必填的。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>要指示筛选的任务状态必须等于进行中，请使用上述行之外的以下行：</p> <p><code>status_Mod=in</code> </p> <p>如果修改量是一个范围，则有两个行表示该修改量。</p> 
       <div> <span class="autonumber"><span><b>示例</b></span></span> 
        <p>这是一个文本模式筛选器，用于查找正在进行的任务、计划完成日期在当前月份内的任务以及分配给具有特定GUID的用户的任务：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>有关文本模式中过滤器修饰符的完整列表，请参阅文章<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>语句运算符。 默认情况下，每个filter语句都通过“AND”运算符连接。 这不会显示在文本模式界面中。 您还可以在两个语句之间添加“OR”运算符，以指示您要筛选满足两个条件中一个或另一个的对象。</p> <p>只有包含多个语句的过滤器才需要过滤器运算符。</p> <p>提示：   
        <ul> 
         <li> <p>“或”区分大小写，且必须始终大写。</p> </li> 
         <li> <p>当您将运算符从AND更改为OR时，列表项的数量可能会增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>示例</b></span></span> 
        <p>要筛选状态为“进行中”或计划完成日期为今天的任务，请使用以下内容： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>通配符，允许您在筛选器中泛化信息并引用当前时间或登录用户。</p> <p>通配符是可选的。</p> <p>提示：   <p>我们建议尽可能使用通配符，以使筛选器更动态，并且不要对每个用户或相似的时间范围复制相同的筛选器。</p> <p>有关筛选器通配符的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">通配符筛选器变量概述</a>。</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>示例</b></span></span> 
        <p>要筛选分配给当前登录用户的任务，请使用以下内容：</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 要添加由“OR”运算符连接的过滤器语句，请执行以下操作：

   1. 添加一行新代码并键入OR:1:，后跟要过滤的对象或属性以及要与它比较的值。 要引用处于“新建”以外的任何状态的任务，请使用以下行：

      `OR:1:status=NEW`

   1. 添加第二行并键入OR:1:，后跟对象、修饰符和修饰符代码。 要为引用所有任务状态（新建除外）的代码行定义修改量，请使用以下修改量行：

      `OR:1:status_Mod=notin`

      新语句的每一行前面都必须加上“OR：`<number>`：”。

      有关在筛选器中创建“OR”语句的信息，请参阅[在文本模式筛选器中创建“OR”语句](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md)。

      >[!NOTE]
      >
      >同一过滤器可以有多个“OR”语句。 每次有新的“OR”语句时，“OR：”之后的数字都会增加。
      >
      >要筛选状态为“进行中”、已分配给登录用户或计划完成日期为今天的任务，请使用以下内容：
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. 单击&#x200B;**退出文本模式**&#x200B;或&#x200B;**完成**&#x200B;以保存文本模式更改并继续编辑报表或筛选器。
1. 单击&#x200B;**保存+关闭**&#x200B;以保存您的报告，或单击&#x200B;**保存筛选器**&#x200B;以将筛选器保存在列表中。


