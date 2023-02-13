---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: ‘报告：预算小时数
description: ‘报告：预算小时数
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# 报表：预算小时数

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

如果要与无权访问资源计划员的其他用户共享预算小时信息，则可以通过构建预算小时报表来执行此操作。 然后，您可以与他们共享该报表。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>预算小时数在Adobe Workfront数据库中每小时更新一次。 刷新报表不一定会刷新报表中的小时信息。 您可以在每个预算小时报表的右上角查看自上次更新以来已经过的时间。 刷新报表时，仅当距上次更新已超过一小时时，才会刷新报表中的信息。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 生成预算小时报表

1. 单击 **主菜单** ![](assets/main-menu-icon.png) ，然后单击 **报表**.

1. 单击 **新建报表>预算小时数**.

   默认视图将应用于报表。

1. （可选）为了更便于阅读，请单击 **预算小时数** 列，然后 **切换到文本模式**，然后更改

   ```
   valuefield
   ```

   行到

   ```
   valueexpreesion
   ```

   并输入舍入表达式。

   这会将预算小时数舍入为您指定的小数位数。

   有关如何在Workfront中对数字进行四舍五入的信息，请参阅文章 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. （可选）单击 **添加列** 添加其他列。
1. （可选）为了更便于阅读，我们建议您为报表添加分组。 我们建议进行以下分组：

   单击 **分组** 选项卡，然后执行以下一个或多个操作：

   1. 单击 **添加分组** 然后开始键入“项目名称”，然后在列表中显示时将其选中。
   1. 单击 **添加分组** 然后开始键入“作业角色名称”，然后在列表中显示时将其选中。
   1. 单击 **添加分组** 开始键入 **分配日期**，选择该时间范围（当该时间范围显示在列表中时），然后从 **分组日期依据** 字段。

1. （可选）单击 **过滤器** 向报表添加过滤器。
1. （可选）单击 **图表** 向报表中添加图表。
1. 单击 **保存并关闭**.

## 复查预算小时报表

默认情况下，“预算小时”报表中提供以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">项目 </td> 
   <td>这是与预算小时关联的项目名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>作业角色</p> </td> 
   <td>这是与预算小时关联的职务角色的名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户</td> 
   <td>这是与预算小时关联的用户名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>这是分配日期。 这是您预算小时数的一周中的第一天（星期日）。</p> <p>提示：  <p>如果一周跨越两个月，则会在报表中生成两行：一个对应于一周的第一天（一周的星期日，即第一个月），另一个对应于第二个月的第一天（可能是一周的任何一天）。</p> <p>例如，如果您为6月30日（星期日） — 7月6日（星期六）这一周的用户预算8小时，则这两行会显示分配日期：6月30日和7月1日。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">预算小时</td> 
   <td>这些是分配给资源计划员中用户的预算小时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">兹罗提。 预算小时</td> 
   <td>这些是分配给资源计划员中任务职责或项目的预算小时数。</td> 
  </tr> 
 </tbody> 
</table>
