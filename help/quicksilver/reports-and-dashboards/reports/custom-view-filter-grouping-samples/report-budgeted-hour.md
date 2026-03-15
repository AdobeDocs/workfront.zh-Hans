---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 报告：预算小时数
description: 报告：预算小时数
author: Courtney
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 4%

---

# 报告：预算小时数

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

如果要与无权访问资源规划器的其他用户共享预算工时信息，可以通过构建预算工时报告来实现。 然后，您可以与他们共享报告。

>[!IMPORTANT]
>
>在Adobe Workfront数据库中，预算工时通常每小时更新一次（很少情况下，最多可能需要三小时）。 刷新报告并不一定刷新其中的小时信息。 在每个预算时数报告的右上角，可以查看自上次更新以来经过的时间。 刷新报告仅在自上次更新后超过一小时时才刷新其中的信息。
>
>![预算工时报告时间同步警告](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或请求修改筛选器 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑筛选器、视图、组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 生成预算工时报告

1. 单击右上角的&#x200B;**“主菜单”**&#x200B;图标![“主菜单”图标](assets/main-menu-icon.png)或&#x200B;**“主菜单”**&#x200B;图标![“主菜单行”](assets/lines-main-menu.png)（如果可用），然后单击&#x200B;**“报告”**。

1. 单击&#x200B;**新建报告** > **更多** > **预算工时**。

   默认视图将应用于报告。

1. （可选）若要使报告更易于阅读，请单击&#x200B;**Bud。 小时**&#x200B;列，然后&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 将`valuefield`行更改为`valueexpreesion`，然后输入舍入表达式。

   这会将预算小时数舍入到您指定的小数位数。

   有关如何在Workfront中舍入数字的信息，请参阅文章[计算数据表达式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**完成**。
1. （可选）单击&#x200B;**添加列**&#x200B;以添加其他列。
1. （可选）要使报告更易于阅读，我们建议您向其添加分组。 我们建议进行以下分组：

   单击&#x200B;**分组**&#x200B;选项卡，然后执行以下一项或多项操作：

   * 单击&#x200B;**添加分组**&#x200B;并开始键入“项目名称”，然后在列表中显示项目名称时将其选中。
   * 单击&#x200B;**添加分组**&#x200B;并开始键入“Job Role Name”，然后在列表中出现该名称时将其选中。
   * 单击&#x200B;**添加分组**&#x200B;并开始键入“分配日期”，当它出现在列表中时将其选中，然后从&#x200B;**分组日期**&#x200B;字段中选择要按其进行分组的时间范围。

1. （可选）单击&#x200B;**筛选器**&#x200B;将筛选器添加到报告中。
1. （可选）单击&#x200B;**图表**&#x200B;将图表添加到报表。
1. 单击&#x200B;**保存+关闭**。

## 复查预算工时报告

默认情况下，预算工时报告中提供以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">项目 </td> 
   <td>这是与预算工时关联的项目的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>工作角色</p> </td> 
   <td>这是与预算工时关联的作业角色的名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户</td> 
   <td>这是与预算工时关联的用户的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>这是分配日期。 这是您为其编列工时预算的周的第一天（星期日）。</p> <p>提示：  <p>如果一周跨两个月，则会在报告中生成两行：一行对应于一周的第一天（一周的星期日，即第一个月中的星期日），另一行对应于第二个月的第一天（可以是一周中的任何一天）。</p> <p>例如，如果您为6月30日（星期日） — 7月6日（星期六）这一周的用户编列了8小时的预算，则两行将显示分配日期为6月30日和7月1日。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">预算小时</td> 
   <td>这些是分配给资源规划器中的用户的预算时数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划。 预算小时</td> 
   <td>这些是分配给资源计划员中的职务角色或项目的预算时数。</td> 
  </tr> 
 </tbody> 
</table>
