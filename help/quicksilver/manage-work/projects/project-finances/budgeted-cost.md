---
content-type: reference
product-area: projects
navigation-topic: financials
title: 计算预算成本
description: 使用利用率报告计算预算成本跟踪项目进度”
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
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

项目的预算成本是在计划项目时与项目关联的总成本（按估计值）。

## 项目中的预算成本概览

您无法手动更改项目的预算成本。 Adobe Workfront使用以下公式计算预算成本：

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 以上计算中的&#x200B;**资源规划者预算劳力成本**&#x200B;是与项目中的工作角色关联的成本。

  您可以在业务案例或资源规划者的资源预算区域中跟踪项目的预算劳力成本。

  >[!TIP]
  >
  >  业务案例中项目的预算劳力成本在报告和列表中显示为资源规划者预算劳力成本。

  有关预算劳力成本的信息，请参阅文章[了解项目的预算劳力成本和预算小时数](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)。

* 以上计算中的&#x200B;**预算费用成本**&#x200B;是与项目费用关联的计划成本，因为这些费用是在业务案例的费用区域或项目的“费用”选项卡中计算的。\
  有关项目费用的详细信息，请参阅文章[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* 上述计算中的&#x200B;**固定成本**&#x200B;是与项目成本关联的固定金额，如项目详细信息部分的“财务”区域中定义。\
  有关项目的“财务”子选项卡的详细信息，请参阅文章[管理项目财务区域的信息](../../../manage-work/projects/project-finances/manage-project-finance-area.md)。

>[!NOTE]
>
>Workfront使用项目的货币计算所有成本信息。 如果您在资源规划者中为资源指定预算小时数，则将禁用更改项目币种的选项。
>
>有关更改项目货币的详细信息，请参阅文章[更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 查找项目的预算成本

业务案例或资源规划者的资源预算区域中反映的预算成本显示在Workfront的以下区域中，并以下列名称命名：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>预算成本显示名称</strong></td> 
     <td><strong>Workfront区域</strong></td> 
    </tr> 
    <tr> 
     <td>预算成本</td> 
     <td> <p>商业论证摘要</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>成本</td> 
     <td> <p>Portfolio优化器</p> <p>提示：所有项目预算成本值的总计是项目组合的预算成本。</p> </td> 
    </tr> 
    <tr> 
     <td>项目预算成本</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>项目报告</p> <p>项目（财务数据）报表</p> <p>任务报告</p> <p>问题报告</p> <p>预算小时数报告</p> <p>有关创建报告的详细信息，请参阅文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报告</a>。</p> </td> 
    </tr> 
   </tbody> 
  </table>
