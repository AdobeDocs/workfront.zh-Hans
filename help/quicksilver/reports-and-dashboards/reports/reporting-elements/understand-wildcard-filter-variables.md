---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: 通配符筛选器变量
description: 通过在过滤器中使用通配符，您可以引用通用用户或日期，而不是特定用户或日期。 通过这种方式，您构建的元素是动态的，并且结果会根据使用它们的上下文而变化。
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 1%

---

# 通配符筛选器变量概述

<!-- Audited: 12/2023 -->

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

使用通配符，您可以引用通用用户或日期，而不是特定用户或日期。 这样，您构建的元素是动态的；结果会根据使用它们的上下文而变化。

例如，在项目报告中筛选$$USER.homeGroupID将仅检索与登录用户的主组关联的项目。

在构建以下元素时，可以使用筛选器变量（也称为通配符）：

<table>
    <tr>
        <td>列表、报告和资源规划者中的过滤器</td>
        <td>有关Workfront过滤器的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">过滤器概述</a>.
</td>
    </tr>
    <tr>
        <td>高级搜索</td>
        <td>有关高级搜索的信息，请参阅部分 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">使用高级搜索</a> 在文章中 <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">搜索Adobe Workfront</a>.
    </tr>
    <tr>
        <td>视图中的计算列</td>
        <td></td>
    </tr>
    <tr>
        <td>视图中的条件格式</td>
        <td>有关条件格式的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">在视图中使用条件格式</a>.
    </tr>
    <tr>
        <td>计算的自定义字段</td>
        <td>在计算列中引用嵌套集合时，不支持通配符筛选器变量。

有关计算的自定义字段和列的信息，请参阅文章 <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">计算的自定义字段与计算的列</a>.
</td>
    </tr>
</table>

## 基于日期的通配符筛选器变量

基于日期的通配符选项可与任何日期筛选器属性结合使用。 有关向报表中添加基于日期的通配符的信息，请参阅文章 [使用基于日期的通配符对报表进行泛化](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>如果创建的日期和时间计算不包括时间部分，或者使用日期通配符$$TODAY或$$NOW，则系统将根据协调世界时(UTC)区域使用日期，而不是根据您的本地时区。 这可能会导致意外的日期结果。

您可以从以下基于日期的通配符中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$今天</strong> </p> </td> 
   <td> <p>我们建议您使用此通配符构建日期敏感型过滤器，以避免在明天、下周或下个月再次构建过滤器。</p> <p>例如，如果要显示今天之前到期的所有任务，可以在任务筛选器中使用以下规则： <em>计划开始日期小于$$TODAY</em>.</p> <p>$$TODAY始终等于当天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>这与$$TODAY通配符类似，但包含当前日期和时间。 $$NOW等于当前日期和时间。</p> <p>例如，如果要显示截至当前时间提供的所有小时条目，则可以在小时过滤器中使用以下规则执行此操作： <em>计划开始日期小于$$NOW</em>.</p> <p>注意：资源规划者不支持此通配符。</p> </td> 
  </tr> 
 </tbody> 
</table>

要指示不同的时间段和不同的时间点（将来或过去），您可以将上面的通配符与以下内容结合使用：

| 属性 |   |
|---|---|
| **q** | 日历季度 |
| **h** | 小时 |
| **d** | 天 |
| **w** | 周 |
| **m** | 月 |
| **y** | 年 |

{style="table-layout:auto"}

| **限定符** | |
|---|---|
| **b** | 一周开始（星期日） |
| **e** | 一周结束（星期六） |

{style="table-layout:auto"}

| **运算符** | |
|---|---|
| **+** | 向通配符值添加值 |
| **-** | 从通配符值中减去值 |

{style="table-layout:auto"}

例如，通配符 `$$TODAYb+2w` 是指“本周开始后的2周”。 通配符*`$$NOW+2h` 是指“2小时之后”。

## 基于用户的通配符筛选器变量

>[!IMPORTANT]
>
>如果过滤器或报表包含基于用户的通配符过滤器变量，则结果始终显示按当前登录的用户过滤的信息。 当您与其他用户共享此类过滤器或报告时，通配符将检索查看报告的用户的信息。 这两个用户会看到不同的结果。
>
>有关向报表中添加基于用户的通配符的信息，请参阅文章 [使用基于用户的通配符对报告进行归纳](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

您可以从以下基于用户的变量中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最常见的基于用户的变量为$$USER.ID。 此操作将始终返回登录用户的ID。 此ID用于标识创建每个对象的用户及其工作分配。</p> <p>在报表中使用时，此通配符会减少需要在系统中创建的报表数量。 您可以创建一个报告并与多个用户共享，并且结果会根据登录并查看该报告的用户而发生更改。</p> <p>例如，要针对分配给登录用户的所有问题构建报告，您可以在问题过滤器中使用以下规则： <em>分配至的ID等于$$USER.ID</em>.</p> <p>Workfront在以下内置筛选器中使用此变量：</p> 
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
   <td> <p>$$USER.categoryID变量是指与登录用户关联的特定自定义表单。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$$USER.accessLevelID变量是指与登录用户关联的访问级别的ID。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$$USER.accessLevelRank变量是指与登录用户关联的访问级别排名。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>$$USER.companyID变量是指与登录用户关联的公司。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID变量是指与您的环境关联的客户帐户ID。 对于您的环境，此变量只有一个可能的值，通常仅在通过API构建集成时使用。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName变量是指登录用户的名字。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName变量是指登录用户的姓氏。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name变量是指登录用户的全名。</p> <p>注意：   <p>仅当在文本模式下修改过滤器时，此通配符变量才起作用。 您无法在不支持文本模式的筛选器中使用此通配符。 例如，您无法在以下区域的筛选条件中使用此通配符：</p> 
     <ul> 
      <li> <p>资源规划程序</p> </li> 
      <li> <p>工作负载均衡器</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID变量是指登录用户的主组的ID。 作为组管理员，您可以使用此变量仅过滤属于主组中的用户的项目。</p> <p>例如，要查看财务组中项目的所有未完成任务，请在任务筛选器中使用以下筛选规则：<br><em>项目：组ID等于$$USER.homeGroupID </em><br><em>完成百分比小于100</em></p> <p>要查看分配给登录用户主组这一特定组中个人的所有未完成任务，请在任务筛选器中使用以下筛选规则：</p> <p><em>分配对象：组ID等于$$USER.homeGroupID<br>完成百分比小于100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs变量是指与登录用户配置文件关联的所有组（包括主组）。</p> <p>此变量的功能与$$USER.homeGroupID变量的功能类似，不同之处在于结果会显示有关属于与登录用户相关联的任何组的用户的信息。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID变量是指登录用户的主团队ID。 作为团队经理，您可以使用此变量仅筛选属于主团队中的用户的项目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs变量返回与登录用户关联的所有团队的列表。</p> <p>此变量的功能与$$USER.homeTeamID变量的功能类似，不同之处在于结果会显示有关属于该筛选条件中确定的任何团队的用户的信息。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID变量是指登录用户的主要角色。 使用此变量，您可以报告分配给特定工作角色的任务或问题。</p> <p>例如，要查看分配给登录用户的主要角色的所有任务，您可以在任务过滤器中使用以下过滤器规则：</p> <p><em>任务：角色ID等于$$USER.roleID。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>$$USER.roleIDs变量是指与登录用户关联的所有工作角色。 使用此变量，您可以报告分配给与登录用户关联的任何工作角色的任务或问题。 </p> <p>例如，要查看分配给与登录用户相关联的任何角色的所有任务，您可以在任务过滤器中使用以下过滤器规则：</p> <p><i>任务：角色ID等于$$USERID.roleIDs<br></i> </p> <p>提示： <i>任务：角色ID等于$$USERID.roleIDs</i> 过滤器规则存在于内置过滤器中：“我的角色中的未分配任务”和“我的角色中的未分配问题”。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 基于对象的通配符筛选器变量

您可以从以下基于对象的通配符中进行选择：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE变量是指对象的类型。 </p> 
     <p>在自定义表单中，如果表单的选定对象类型与计算自定义字段中引用的字段不兼容，则可以使用此通配符避免为这些对象类型创建重复表单的解决方法。</p> 
     <p>在计算自定义字段中，通过在IF表达式中包含通配符来实现这一点，以便计算可以为表单的每个对象类型输出不同的值。 </p> 
     <p>有关更多信息和示例，请参阅部分 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">多对象自定义表单中计算的自定义字段</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">将计算的数据添加到自定义表单</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
