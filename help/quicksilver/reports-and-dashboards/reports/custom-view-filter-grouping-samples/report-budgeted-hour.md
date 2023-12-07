---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '报告：预算小时数'
description: '报告：预算小时数'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---

# 报告：预算小时数

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

当您希望与无权访问资源规划者的其他用户共享预算小时数信息时，可以通过构建预算小时数报表来实现这一点。 然后，您可以与他们共享该报表。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>预算小时数每小时在Adobe Workfront数据库中更新一次。 刷新报告不一定刷新其中的小时信息。 您可以在每个预算小时报表的右上角查看自上次更新以来经过的时间。 仅当自上次更新以来已超过一小时时，刷新报告才会刷新其中的信息。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 生成预算小时报告

1. 单击 **主菜单** ![](assets/main-menu-icon.png) 图标，然后单击 **报表**.

1. 单击 **新报表>预算小时数**.

   默认视图应用于报表。

1. （可选）要使报表更易于阅读，请单击 **预算小时数** 列，然后 **切换到文本模式**，然后更改

   ```
   valuefield
   ```

   行至

   ```
   valueexpreesion
   ```

   并输入舍入表达式。

   这会将预算小时数舍入到您指定的小数位数。

   有关如何在Workfront中舍入数字的信息，请参阅文章 [计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. （可选）单击 **添加列** 以添加其他列。
1. （可选）为了使报表更易于阅读，我们建议您向报表中添加分组。 我们建议进行以下分组：

   单击 **分组** 选项卡，然后执行以下一项或多项操作：

   1. 单击 **添加分组** 并开始键入“项目名称”，然后当它出现在列表中时将其选中。
   1. 单击 **添加分组** 并开始键入“工作角色名称”，然后当它出现在列表中时将其选中。
   1. 单击 **添加分组** 并开始键入 **分配日期**，选择显示在列表中的时间范围，然后从中选择要作为分组依据的时间范围 **日期分组条件** 字段。

1. （可选）单击 **过滤器** 以向报表中添加过滤器。
1. （可选）单击 **图表** 以向报表中添加图表。
1. 单击 **保存+关闭**.

## 查看预算小时数报告

默认情况下，预算小时数报表中提供了以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">项目 </td> 
   <td>这是与预算小时数关联的项目的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>工作角色</p> </td> 
   <td>这是与预算小时数关联的工作角色的名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户</td> 
   <td>这是与预算小时数关联的用户的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>这是分配日期。 这是您为其预算小时数的每周第一天（星期日）。</p> <p>提示：  <p>如果一周持续两个月，这会在报表中生成两行：一行对应于一周的第一天（一周的周日，位于第一个月），另一行对应于第二个月的第一天（可以是一周中的任何一天）。</p> <p>例如，如果您为用户分配6月30日（星期日）至7月6日（星期六）这周的8小时的预算，则两行显示分配日期为6月30日和7月1日。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">预算小时</td> 
   <td>这些是资源规划者中分配给用户的预算小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划 预算小时</td> 
   <td>这些是分配给资源规划者中的工作角色或项目的预算小时数。</td> 
  </tr> 
 </tbody> 
</table>
