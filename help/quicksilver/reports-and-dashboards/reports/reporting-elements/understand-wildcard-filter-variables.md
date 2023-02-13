---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: 通配符过滤器变量
description: 通过在过滤器中使用通配符，您可以引用通用用户或日期，而不是特定用户或日期。 这样，您构建的元素就会是动态的，结果会根据使用这些元素的上下文而发生更改。
author: Lisa
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 2%

---

# 通配符过滤器变量

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Adobe Workfront在生成以下元素时支持筛选变量或通配符：

* 列表、报表和资源计划员中的过滤器

   有关Workfront过滤器的信息，请参阅文章 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 高级搜索

   有关高级搜索的信息，请参阅部分 [使用高级搜索](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) 在文章中 [搜索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* 视图中的计算列
* 视图中的条件格式

   有关条件格式的信息，请参阅文章 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* 计算的自定义字段

   >[!NOTE]
   >
   >在计算列中引用嵌套集合时，不支持通配符过滤器变量。

   有关计算的自定义字段和列的信息，请参阅文章 [计算自定义字段与计算列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

通过使用通配符，您可以引用通用用户或日期，而不是特定用户或日期。 这样，您构建的元素就会是动态的，结果会根据使用这些元素的上下文而发生更改。

例如，在项目报表中筛选$USER.homeGroupID时，只检索与登录用户的“主页组”关联的项目。

您可以在Workfront中使用基于日期或基于用户的过滤器变量。

## 基于日期的通配符过滤器变量

Workfront基于日期的通配符选项可以与任何日期过滤器属性结合使用。

有关向报表添加基于日期的通配符的信息，请参阅文章 [使用基于日期的通配符对报表进行归纳](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>如果您创建的日期和时间计算不包含时间部分，或者使用日期通配符$$TODAY或$NOW，则系统会根据协调通用时间(UTC)区域来使用日期，而不是根据您的本地时区。 这可能会导致意外的日期结果。

从以下基于日期的通配符中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>今天$</strong> </p> </td> 
   <td> <p>我们建议您使用此通配符生成对日期敏感的过滤器，这样您就无需在明天、下周或下月再次构建过滤器。</p> <p>例如，如果要显示今天之前到期的所有任务，您可以在任务筛选器中使用以下规则： <em>计划开始日期少于$TODAY</em>.</p> <p>$TODAY始终等于当天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$NOW</strong> </p> </td> 
   <td> <p>这类似于$$TODAY通配符，但包括当前日期和时间。 $$NOW等于当前日期和时间。</p> <p>例如，如果要显示截至当前时间提供的所有小时条目，则可以在小时过滤器中使用以下规则来执行此操作： <em>计划开始日期少于$NOW</em>.</p> <p>注意：资源规划器不支持此通配符。</p> </td> 
  </tr> 
 </tbody> 
</table>

要指示不同时间段和不同时间点（将来或过去），可将通配符与以下内容组合：

| 属性 |   |
|---|---|
| **q** | 日历季度 |
| **h** | 小时 |
| **d** | 天 |
| **w** | 周 |
| **m** | 月 |
| **y** | 年 |

{style=&quot;table-layout:auto&quot;}

| **限定符** |  |
|---|---|
| **b** | 星期初（星期日） |
| **e** | 周末（星期六） |

{style=&quot;table-layout:auto&quot;}

| **运算符** |  |
|---|---|
| **+** | 将值添加到通配符值 |
| **-** | 从通配符值中减去值 |

{style=&quot;table-layout:auto&quot;}

例如，通配符 `$$TODAYb+2w` 是指“从本周开始算起2周”。 通配符*`$$NOW+2h` 是指“2小时后”。

## 基于用户的通配符过滤器变量

>[!IMPORTANT]
>
>如果过滤器或报表包含基于用户的通配符过滤器变量，则结果始终显示按当前登录用户过滤的信息。 当您与其他用户共享此类过滤器或报表时，通配符会为查看报表的用户检索信息。 两个用户会看到不同的结果。

有关向报表添加基于用户的通配符的信息，请参阅文章 [使用基于用户的通配符对报表进行归纳](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront提供了以下基于用户的变量：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最常见的基于用户的变量是$USER.ID。 这将始终返回已登录用户的ID。 这是用于标识创建每个对象的用户及其工作分配的ID。</p> <p>在报表中使用此通配符会减少您需要在系统中创建的报表数量。 您可以创建一个报表并将其与多个用户共享，并且结果会根据登录用户和查看报表的用户而发生更改。</p> <p>例如，要为分配给登录用户的所有问题构建报表，您可以在问题过滤器中使用以下规则： <em>分配给ID等于$USER.ID</em>.</p> <p>Workfront在以下内置过滤器中使用此变量：</p> 
    <ul> 
     <li>我的报告</li> 
     <li>我的项目</li> 
     <li>我的任务</li> 
     <li>我的问题</li> 
     <li>我的小时</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>$USER.categoryID变量引用与登录用户关联的特定自定义表单。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$USER.accessLevelID变量引用与登录用户关联的访问级别的ID。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$USER.accessLevelRank变量引用与登录用户关联的访问级别排名。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.companyID</strong> </p> </td> 
   <td> <p>$USER.companyID变量引用与登录用户关联的公司。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.customerID</strong> </p> </td> 
   <td> <p>$USER.customerID变量引用与您的环境关联的客户帐户的ID。 对于您的环境，此变量只有一个可能的值，通常仅在通过API构建集成时才使用。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName变量引用登录用户的名字。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$USER.lastName变量引用登录用户的姓氏。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$USER.name变量引用登录用户的全名。</p> <p>注释:   <p>此通配符变量仅在文本模式下修改过滤器时有效。 不能在不支持文本模式的过滤器中使用此通配符。 例如，您不能在以下区域的过滤器中使用此通配符：</p> 
     <ul> 
      <li> <p>资源规划程序</p> </li> 
      <li> <p>工作负载均衡器</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$USER.homeGroupID变量引用登录用户的主组ID。 作为群组管理员，您可以使用此变量仅过滤属于您的“主页”群组中用户的项目。</p> <p>例如，要查看财务组中项目上所有未完成的任务，请在任务筛选器中使用以下筛选规则：<br><em>项目：组ID等于$USER.homeGroupID </em><br><em>完成百分比小于100</em></p> <p>要查看分配给特定组（即已登录用户的主组）中个人的所有未完成任务，请在任务筛选器中使用以下筛选器规则：</p> <p><em>分配给：组ID等于$USER.homeGroupID<br>完成百分比小于100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$USER.otherGroupIDs变量引用与登录用户的配置文件关联的所有组（包括主组）。</p> <p>此变量的功能与$$USER.homeGroupID变量的功能类似，不同之处在于，结果显示了属于与登录用户关联的任何组的用户的信息。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$USER.homeTeamID变量引用已登录用户的主团队的ID。 作为团队经理，您可以使用此变量仅过滤属于您主团队中用户的项目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.teamIDs</strong> </p> </td> 
   <td> <p>$USER.teamIDs变量会返回与已登录用户关联的所有团队的列表。</p> <p>此变量的功能与$USER.homeTeamID变量的功能类似，不同之处在于，结果会显示有关属于过滤器中已识别任何团队的用户的信息。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$USER.roleID</strong> </p> </td> 
   <td> <p>$USER.roleID变量引用登录用户的主要角色。 使用此变量，您可以报告分配给特定作业角色的任务或问题。</p> <p>例如，要查看分配给已登录用户的“主角色”的所有任务，您可以在任务筛选器中使用以下筛选规则：</p> <p><em>任务：角色ID等于$USER.roleID。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$USER.roleIDs</td> 
   <td> <p>$USER.roleIDs变量引用与登录用户关联的所有作业角色。 使用此变量，您可以报告分配给与登录用户关联的任何作业角色的任务或问题。 </p> <p>例如，要查看分配给与登录用户关联的任何角色的所有任务，您可以在任务筛选器中使用以下筛选规则：</p> <p><i>任务：角色ID等于$USERID.roleIDs<br></i> </p> <p>提示：的 <i>任务：角色ID等于$USERID.roleIDs</i> 过滤器规则存在于“我的角色”的“未分配任务”和“我的角色”的“未分配问题”中。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 基于对象的通配符过滤器变量

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$OBJCODE变量引用对象的类型。 </p> 
     <p>在自定义表单中，当表单的选定对象类型与计算的自定义字段中引用的字段不兼容时，您可以使用此通配符避免为这些对象类型创建重复表单的解决方法。</p> 
     <p>在计算的自定义字段中，您可以通过在IF表达式中包含通配符来实现此目的，以便计算可以针对表单的每种对象类型输出不同的值。 </p> 
     <p>有关更多信息和示例，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">多对象自定义表单中的计算自定义字段</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">将计算数据添加到自定义表单</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
