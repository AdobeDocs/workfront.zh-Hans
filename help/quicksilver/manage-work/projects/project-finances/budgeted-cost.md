---
content-type: reference
product-area: projects
navigation-topic: financials
title: 计算预算成本
description: 计算预算成本跟踪项目进度（含利用率报表）”
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# 计算预算成本

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

项目的预算成本是与计划项目时估计的项目关联的总成本。

## 项目预算成本概览

您不能人工更改项目的预算成本。 Adobe Workfront使用以下公式计算预算成本：

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 的 **资源计划员预算人工成本** 在上述计算中，是与项目中的任务角色关联的成本。

   您可以在“业务案例”或“资源计划员”的“资源预算”区域中跟踪项目的预算人工成本。

   >[!TIP]
   >
   >  “业务案例”中项目的预算人工成本在报表和列表中显示为“资源计划员预算人工成本”。

   有关预算人工成本的信息，请参阅文章 [了解项目的预算人工成本和预算工时](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* 的 **预算费用成本** 在以上计算中，与项目费用关联的计划成本，它们是在“业务案例”的“费用”区域或项目的“费用”标签中计算的。\
   有关项目费用的详细信息，请参阅文章 [管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* 的 **固定成本** 在上述计算中，与项目成本关联的固定金额，在项目“详细信息”部分的“财务”区域中定义。\
   有关项目“财务”子选项卡的详细信息，请参阅文章 [在项目财务区管理信息](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront使用项目的货币计算所有成本信息。 如果在资源计划器中为资源指定预算小时数，则更改项目币种的选项将被禁用。
>
>有关更改项目货币的更多信息，请参阅文章 [更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md).

## 查找项目的预算成本

“业务案例”或“资源计划员”的“资源预算”区域中反映的预算成本将以下名称显示在Workfront的以下区域：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>预算成本显示名称</strong></td> 
     <td><strong>Workfront地区</strong></td> 
    </tr> 
    <tr> 
     <td>预算成本</td> 
     <td> <p>商业论证摘要</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>成本</td> 
     <td> <p>Portfolio优化程序</p> <p>提示：所有项目预算成本值的合计为项目组合的预算成本。</p> </td> 
    </tr> 
    <tr> 
     <td>项目预算成本</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>项目报告</p> <p>项目（财务数据）报表</p> <p>任务报告</p> <p>问题报告</p> <p>预算小时报表</p> <p>有关创建报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
