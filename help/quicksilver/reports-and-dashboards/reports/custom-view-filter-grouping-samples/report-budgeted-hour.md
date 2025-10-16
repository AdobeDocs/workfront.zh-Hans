---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 报告：预算小时数
description: 报告：预算小时数
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 1%

---

# 报告：预算小时数

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

当您希望与无权访问资源规划者的其他用户共享预算小时数信息时，可以通过构建预算小时数报表来实现这一点。 然后，您可以与他们共享该报表。

>[!IMPORTANT]
>
>预算小时数通常每小时在Adobe Workfront数据库中更新一次（在不常见情况下，最多可能需要三个小时）。 刷新报告不一定刷新其中的小时信息。 您可以在每个预算小时报表的右上角查看自上次更新以来经过的时间。 仅当自上次更新以来已超过一小时时，刷新报告才会刷新其中的信息。
>
>![预算小时报告时间同步警告](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 生成预算小时报告

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)或左上角的&#x200B;**主菜单**&#x200B;图标![主菜单行](assets/lines-main-menu.png)（如果可用），然后单击&#x200B;**报表**。

1. 单击&#x200B;**新报告** > **更多** > **预算小时数**。

   默认视图应用于报表。

1. （可选）若要使报表更易于阅读，请单击&#x200B;**Bud。 小时**&#x200B;列，然后&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 将`valuefield`行更改为`valueexpreesion`并输入舍入表达式。

   这会将预算小时数舍入到您指定的小数位数。

   有关如何在Workfront中舍入数字的信息，请参阅文章[计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**完成**。
1. （可选）单击&#x200B;**添加列**&#x200B;以添加其他列。
1. （可选）为了使报表更易于阅读，我们建议您向报表中添加分组。 我们建议进行以下分组：

   单击&#x200B;**分组**&#x200B;选项卡，然后执行以下一项或多项操作：

   * 单击&#x200B;**添加分组**&#x200B;并开始键入“项目名称”，然后当它出现在列表中时将其选定。
   * 单击&#x200B;**添加分组**&#x200B;并开始键入“工作角色名称”，然后当它出现在列表中时将其选定。
   * 单击&#x200B;**添加分组**&#x200B;并开始键入“分配日期”，当它出现在列表中时将其选中，然后从&#x200B;**日期分组依据**&#x200B;字段中选择要作为分组依据的时间范围。

1. （可选）单击&#x200B;**筛选器**&#x200B;以将筛选器添加到报表。
1. （可选）单击&#x200B;**图表**&#x200B;以向报表中添加图表。
1. 单击&#x200B;**保存+关闭**。

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
