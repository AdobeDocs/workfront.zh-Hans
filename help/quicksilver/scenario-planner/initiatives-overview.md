---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Scenario Planner中的计划概述
description: Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅Scenario Planner概述。
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# [!DNL Scenario Planner]中的计划概述

作为业务经理，您可以在[!DNL Adobe Workfront Scenario Planner]中创建计划的计划。 有关创建计划的信息，请参阅文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

## 计划概述

使用[!DNL Workfront Scenario Planner]，您可以估计和查看每个计划的以下信息：

* 估计完成计划可能需要的工作角色的类型和数量。 这将添加到计划的“必需”工作角色计数，并计算可为计划复查的人员成本。
* 估算与完成计划所需的工作相关的固定成本。
* 估算计划完成时贵公司可能获得的计划收益。

要查看有关计划的信息，您可以访问计划中的各个计划。 有关创建和访问计划的信息，请参阅文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

## 关于计划的注意事项

创建计划时，请考虑以下事项：

* 在创建计划之前，必须先创建计划。
* 您可以从头开始创建计划，也可以将项目导入计划。 这些项目将成为计划内的计划。

  有关从头开始创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

  有关将项目导入计划以从项目创建计划的信息，请参阅[将项目导入计划中的 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)。

* 计划是比计划小的规划单元，它们仅作为计划的一部分创建。
* 最短的主动行动可以持续1个月。 最长倡议的期限可为5年。
* 您不能对计划执行实际工作。 在方案层，您可以定义需要哪些资源以及这些资源将产生哪些成本，以便开始执行计划的某个需求。 例如，如果贵公司计划在新位置扩展并收购新办公室，则您的部门可能会主动为该新位置安装网络基础架构。
* 您可以在一个计划中创建多个计划。 对于每个计划，您都可以概述一个高级战略来完成您所在部门的工作。
* 您可以优先处理计划内的计划，以确保最重要的计划获得最多的预算和最多的资源。
* 在计划中创建计划时，查看该计划的所有人也可以查看该计划中的所有计划。
* 您可以发布计划以创建项目或更新链接到它们的项目。 有关发布计划的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

## 关于计划的财务信息

您可以查看有关各个计划的财务信息，以了解计划如何适应计划。 有关访问计划的信息，请参阅文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

通过访问计划中的方案，可以查看有关方案的以下财务指标：

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 成本总额]</td> 
   <td> <p style="font-weight: normal;">这是对计划总成本的计算。 </p> <p style="font-weight: normal;">[!DNL Workfront] 使用此公式计算方案的总成本值：</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 固定成本]</td> 
   <td> <p><span style="font-weight: normal;">这是一个手动输入项，您可以估计计划每个月的固定成本金额<span>。</span>这不包括与添加到计划的角色相关的成本，这些角色在[!UICONTROL 人员成本]字段中捕获。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 人员成本]</td> 
   <td> <p style="font-weight: normal;">这是计划持续时间中与计划工作角色相关的成本的总计算。 此数字取决于您为计划每月的工作角色估计的FTE或小时数。 </p> 
     <p><b>提示</b>  
     <ul> 
      <li> <p>同一工作角色的每月FTE数量可能因月而异。</p> </li> 
      <li> <p>[!DNL Workfront] 认为一个月有160个工作时间。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] 使用以下公式计算计划的[!UICONTROL 人员成本]：</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront]使用以下公式计算计划持续期间每个月的每月人员成本：</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>示例</b></p>
      <p>如果您有一个为期6个月的计划，其中要求1个Designer按每月1个FTE的小时费率为50美元，而一个Web Designer按计划2个月的小时费率为100美元，则计划的人员成本计算如下：</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划收益]</td> 
   <td>这是一个手动输入项，您可以在其中估计部门完成此计划将获得的总体收益。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 净值金额]</td> 
   <td> <p style="font-weight: normal;">这代表在考虑总体成本和计划预计的福利时，计划的价值。 [!DNL Workfront]使用以下公式计算方案的净值：</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## 报告中的计划信息

您可以在报表中显示方案信息，如下表所述。 仅当您的公司购买了Workfront Scenario Planner许可证时，此信息才会在您的Workfront实例中可用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>报告类型</b></td> 
   <td><b>计划信息</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 计划] </td> 
   <td>名称、持续时间、开始和结束日期、输入者、ID、上次发布日期*、所有项目字段，包括自定义字段*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 计划工作角色]</td> 
   <td>上面列出的所有计划信息、（工作角色） ID、项目*、项目分配计划小时数*、计划工作角色小时数、（工作角色）计数、所有项目字段，包括自定义字段*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL 项目]*</p></td> 
   <td> <p>以上列出的所有计划信息*</p> </td> 
  </tr> 
 </tbody> 
</table>

*仅当从项目创建计划或至少将计划发布到项目一次时，这些字段才会填充链接到计划的项目中的信息。 有关发布计划的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。
