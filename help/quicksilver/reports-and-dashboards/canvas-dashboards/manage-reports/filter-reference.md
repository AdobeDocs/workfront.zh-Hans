---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 画布功能板的报表过滤器引用
description: 引用在画布功能板中过滤报表时可以使用的字段、运算符、通配符和特殊规则。
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 85ae49708acf2c472816ac848ce15429577b934e
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 9%
---
# 画布功能板的报表过滤器引用

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

本文介绍了过滤报表时可用的字段、运算符、通配符和特殊规则。 有关构建或编辑过滤器的步骤，请参阅[在画布功能板中过滤报表](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-a-report.md)。

## 按字段类型划分的字段运算符

+++ 展开以查看按字段类型划分的字段运算符列表。 

<table>
    <tr>
        <td><b>字段类型</b></td>
        <td><b>示例</b></td>
       <td><b>操作员</b></td>
        <td><b>通配符</b></td>
    </tr>
    <tr>
        <td>对象/引用名称</td>
        <td>任何本机名称属性或自定义查找</td>
              <td><ul>
        <li>等于</li>
        <li>不等于</li>
        <li>包含</li>
          <li>不包含</li>
            <li>为空</li>
              <li>不为空</li>
        </ul></td>
        <td>用户：名称
        <ul>
        <li>我（已登录的用户）</li>
        </ul>
        组：名称
        <ul>
          <li>我的家庭组（登录用户组）</li>
            <li>我的其他群组（已登录用户群组）</li>
          </ul>
          团队：名称
                  <ul>
          <li>我的默认团队（登录用户的团队）</li>
            <li>我的其他团队（登录用户的团队）</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>字符串/文本输入 </td>
                <td>项目：描述</td>
                      <td><ul>
             <li>等于</li>
        <li>不等于</li>
        <li>包含</li>
          <li>不包含</li>
            <li>为空</li>
              <li>不为空</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>整数/双精度</td>
             <td>项目：计划小时数
        <br>任务：完成百分比</td>
              <td><ul>
        <li>等于</li>
        <li>不等于</li>
        <li>大于</li>
          <li>大于或等于</li>
          <li>小于</li>
          <li>小于或等于</li>
            <li>为空</li>
              <li>不为空</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> 日期/日期时间 </td>
                    <td>项目：计划开始日期
        <br>小时：输入日期</td>
              <td><ul>
        <li>等于</li>
        <li>不等于</li>
        </ul></td>
        <td>通过切换<b>设置相对日期</b>选项，您可以应用相对日期通配符，使报表更动态，并根据常见的日期时段进行自我调整。 
         <ul><li>$$今天</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>布尔值 </td>
                  <td>项目：具有文档
        <br>任务：关键
        <br>用户：处于活动状态</td>
        <td><ul>
        <li>等于</li>
        <li>不等于</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++

## 基于日期的通配符筛选器变量

基于日期的通配符选项可与任何日期筛选器属性结合使用。 有关向报表中添加基于日期的通配符的信息，请参阅[使用基于日期的通配符来泛化报表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

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
   <td> <p>我们建议您使用此通配符构建日期敏感型过滤器，以避免在明天、下周或下个月再次构建过滤器。</p> <p>例如，如果要显示今天之前到期的所有任务，可以在任务筛选器中使用以下规则： <em>计划开始日期小于$$TODAY</em>。</p> <p>$$TODAY始终等于当天的午夜。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>这与$$TODAY通配符类似，但包含当前日期和时间。 $$NOW等于当前日期和时间。</p> <p>例如，如果您希望显示截至当前时间提供的所有小时条目，则可以在小时过滤器中使用以下规则执行此操作：<em>计划开始日期小于$$NOW</em>。</p> <p>注意：资源规划者不支持此通配符。</p> </td> 
  </tr> 
 </tbody> 
</table>

要指示不同的时间段和不同的时间点（将来或过去），您可以将上面的通配符与以下内容结合使用：

| 属性 |   |
|---|---|
| **q** | 日历季度 |
| **小时** | 小时 |
| **天** | 天 |
| **w** | 周 |
| **分钟** | 月 |
| **y** | 年 |

{style="table-layout:auto"}

| **限定符** |   |
|---|---|
| **b** | 期间开始（没有指定属性，默认为一周的开始：星期日） |
| **e** | 期间结束（没有指定属性，默认为一周的结束：星期六） |

{style="table-layout:auto"}

| **操作员** |   |
|---|---|
| **+** | 向通配符值添加值 |
| **-** | 从通配符值中减去值 |

{style="table-layout:auto"}

例如，通配符`$$TODAYb+2w`引用“从本周开始的2周”。 通配符`$$NOW+2h`引用“从现在起的2小时”。

## 登录用户通配符筛选器变量

* 筛选用户`name`属性时，您将查看&#x200B;**我（已登录的用户）**&#x200B;选项。

  ![用户名属性](assets/user-name-attribute.png)

* 在筛选组`name`属性时，您将查看要在筛选条件中使用的&#x200B;**我的主组（已登录的用户组）**&#x200B;和&#x200B;**我的其他组（已登录的用户组）**&#x200B;选项。

  ![组名属性](assets/group-name-attribute.png)

* 在筛选团队`name`属性时，您将查看可在筛选条件中选择的&#x200B;**我的默认团队（已登录的用户团队）**&#x200B;和&#x200B;**我的其他团队（已登录的用户团队）**&#x200B;选项。

  ![团队名称属性](assets/team-name-attribute.png)

## 引用子对象

其他列、筛选器选项和分组属性的可用关系通常仅限于Workfront对象层次结构中较高的对象，或者在报表的基本实体对象上具有单个选择。 这种情况有一些例外，其中包括：

* 项目>任务
* 文档审批>文档审批阶段
* 文档审批阶段>文档审批阶段参与者

使用上面列出的任何父子关系时，您将在表中看到连接到父对象的每个子记录的一行。

<!--
<div class="preview">

## Filter on collection relationships in Preview

A collection is a field that links to a group of related records rather than to a single record. For example, the participants on a project's approval stages are a collection. When you build a filter, you can filter on collections directly, without switching to text mode.

To filter on a collection, open the Select a field panel, then select Collections. This section lists only collection relationships. Single-record relationships stay under Relationships.

![collection relationships](assets/collections.png)

After you select a collection, you can do two things:

* Filter on the collection's own fields. For example, from a portfolio's projects, you can filter on a project's status.
* Follow one single-record relationship out of the collection. For example, from a portfolio's projects, you can reach the project owner.

Collections don't support deeper navigation. You can't open a collection nested inside another collection, follow more than one relationship, or select the relationship that leads back to where you started.

The Collections section appears only when you build a filter. It doesn't appear in other field choosers, such as those for table columns, groupings, or chart fields.

</div>

-->

## 排除个人项目、任务和机器人用户

>[!NOTE]
>
>如果与类似的经典报表相比，画布功能板报表返回的结果多于您的预期，则默认情况下可能包含个人项目、个人任务或机器人用户。 添加筛选条件以排除它们。

在画布功能板项目和任务报告中，不会自动应用`isPersonal`筛选器，因此默认情况下结果中包含个人项目和个人任务。 要排除它们，请添加筛选条件，如`isPersonal=false`。

同样，默认情况下，画布功能板用户报表包含所有用户，包括AI协作者（机器人用户）。 要排除机器人用户，请添加筛选条件，如`isBot=false`。

传统项目和任务报表自动排除个人项目和个人任务，而传统用户报表自动排除机器人用户。 要将其包含在传统报表中，请添加筛选条件，如`isPersonal=true`（仅个人项目）或`isPersonal_Mod=notnull`（个人和非个人项目）。
