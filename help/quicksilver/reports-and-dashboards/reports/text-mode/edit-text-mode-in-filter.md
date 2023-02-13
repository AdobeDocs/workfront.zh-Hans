---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式编辑过滤器
description: ‘注意：在本文中添加一节：/内容/报表和功能板/报表/报表Elements/create-customize-fitlers.html;***此外，在文本模式概述文章中起草此区域)`
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# 使用文本模式编辑过滤器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

您可以在列表或报表中使用文本模式编辑过滤器，以访问标准界面中不可用的字段，并创建更复杂的过滤器。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的报表元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的过滤器</p> <p>管理过滤器的权限以对其进行编辑</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

开始在报表或列表中使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、过滤器和分组示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在过滤器中编辑文本模式

对于报表和列表，使用文本模式编辑过滤器的方式相同。 从报表或列表访问视图的方式有所不同。

>[!TIP]
>
>我们建议您在标准模式下尽可能多地构建过滤器，然后将过滤器转换为文本模式以对其进行编辑。

有关构建过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

有关创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 执行下列操作之一：

   1. 要从报表访问过滤器，请转到报表，然后单击 **报表操作** > **编辑** > **过滤器** 选项卡。
   1. 要从列表访问过滤器，请转到列表，然后从 **过滤器** 下拉菜单中，将鼠标悬停在要修改的过滤器上，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

      此时会打开过滤器生成器。

1. 单击 **添加过滤器规则** 要开始添加过滤器的条件，请单击 **切换到文本模式** 中。
1. 使用文本模式添加filter语句。 每个filter语句可以包含以下行和其他信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>过滤行/信息</td> 
      <td>示例</td> 
     </tr> 
     <tr> 
      <td> <p>字段名称及其等于在Workfront数据库中显示的值。</p> <p>此行是必填行。</p> <p> 有关对象和字段在数据库中的显示方式的详细信息，请参阅 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>要筛选状态为“进行中”的任务，请使用以下行：</p> <p><code>status=INP</code> </p> <p>提示：筛选状态时，必须使用状态的三字母代码，而不是名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>字段名称修饰符以及修饰符等于的内容。 这表示您要筛选的字段必须满足的条件。</p> <p>此行是必填行。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>要指示您筛选的任务的状态必须等于“正在进行”，请除以上行外，使用以下行：</p> <p><code>status_Mod=in</code> </p> <p>如果修改量是一个范围，则有两行可指示该修改量。</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>示例: </b></span></span> 
        <p>这是一种文本模式筛选器，用于查找正在进行的任务，这些任务在当月具有计划完成日期，并且已分配给具有特定GUID的用户：</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>有关文本模式下的过滤器修饰符的完整列表，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>语句运算符。 默认情况下，每个filter语句都使用“AND”运算符连接。 这不会在文本模式界面中显示。 您还可以在两个语句之间添加“OR”运算符，以指示您希望筛选满足两个条件之一或另一个条件的对象。</p> <p>仅对于具有多个语句的过滤器，需要使用过滤器运算符。</p> <p>提示：   
        <ul> 
         <li> <p>“或”区分大小写，且必须始终大写。</p> </li> 
         <li> <p>将运算符从AND更改为OR时，列表项的数量可能会增加。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>示例: </b></span></span> 
        <p>要筛选状态为“进行中”或“计划完成日期为今天”的任务，请使用以下方法： </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>通配符，用于对过滤器中的信息进行归纳并引用当前时间或登录用户。</p> <p>通配符是可选的。</p> <p>提示：   <p>我们建议尽可能使用通配符来增强过滤器的动态性，并且不要为每个用户或类似的时间范围重复相同的过滤器。</p> <p>有关筛选通配符的信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">通配符过滤器变量</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>示例: </b></span></span> 
        <p>要筛选分配给当前已登录用户的任务，请使用以下代码：</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 要添加由“OR”运算符连接的filter语句，请执行以下操作：

   1. 添加新的代码行并键入OR:1: 后跟要筛选的对象或属性以及要与之进行比较的值。 要引用除“新建”之外处于任何状态的任务，请使用以下行：

      ```
      OR:1:status=NEW
      ```

   1. 添加第二行并键入OR:1: 后跟对象、修饰符和修饰符代码。 要为引用除“新建”之外的所有任务状态的代码行定义修改量，请使用以下修改量行：

      ```
      OR:1:status_Mod=notin
      ```

      新语句的每一行都必须在“OR:`<number>`：“”。

      有关在过滤器中创建“OR”语句的信息，请参阅 [在文本模式筛选器中创建“OR”语句](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>您可以在同一过滤器中使用多个“OR”语句。 每次您有新的“OR”语句时，“OR：”后面的数字都会增加。
要筛选状态为“进行中”或已分配给登录用户或具有计划完成日期（今天）的任务，请使用以下方法：
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. 单击 **完成** 如果要保存更改并继续编辑报表或过滤器，请执行以下操作：
1. 单击 **保存并关闭** 保存报表或 **保存过滤器** 以在列表中保存过滤器。
