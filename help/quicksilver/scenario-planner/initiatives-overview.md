---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 方案规划器中的方案概述
description: 方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案计划员的信息，请参阅：方案计划员概览
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# 中的计划概述 [!DNL Scenario Planner]

的 [!DNL Scenario Planner] 只能在新 [!DNL Adobe Workfront] 体验，并且需要其他许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 [的 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).
作为业务经理，您可以在 [!DNL Adobe Workfront Scenario Planner]. 有关创建计划的信息，请参阅文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## 计划概述

使用 [!DNL Workfront Scenario Planner]，您可以评估和查看每个计划的以下信息：

* 估计完成计划可能需要的工作角色的类型和数量。 这会将计划的“必需职务”职责计数添加到该计划，并计算您可以为方案复查的人员成本。
* 估计与完成方案所需工作相关的固定成本。
* 估算计划完成后贵公司可能获得的计划福利。

要查看有关您的计划的信息，您可以访问计划中的各个计划。 有关创建和访问计划的信息，请参阅文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## 有关计划的考虑事项

创建计划时请考虑以下事项：

* 必须先创建计划，然后才能创建方案。
* 您可以从头开始创建方案，也可以将项目导入计划。 这些项目成为计划内的倡议。

   有关从头开始创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   有关将项目导入计划以从项目创建方案的信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 计划是比计划小的规划单位，只作为计划的一部分创建。
* 最短计划的期限为1个月。 最长的倡议可以有5年的期限。
* 不能对方案进行实际工作。 在方案层，您可以定义需要哪些资源以及这些资源将产生的成本，以便您开始执行计划的其中一项需求。 例如，如果贵公司计划在新位置扩展并购买新办公室，则您的部门可能会主动为该新位置安装网络基础架构。
* 您可以在一个计划中创建多个方案。 通过每项计划，您可以概述完成部门工作的高级战略。
* 您可以在计划中对计划进行优先排序，以确保最重要的计划获得最多的预算和资源。
* 在计划内创建计划时，每个查看该计划的人也可以查看计划内的所有计划。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* 您可以发布各种方案以创建项目或更新与其关联的项目。 有关发布计划的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## 有关计划的财务信息

您可以查看有关单个计划的财务信息，以了解计划中计划的适合程度。 有关访问计划的信息，请参阅文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

您可以通过在计划中访问某个方案来查看有关该方案的以下财务指标：

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本总额]</td> 
   <td> <p style="font-weight: normal;">这是计算一项计划的总费用。 </p> <p style="font-weight: normal;">[!DNL Workfront] 使用此公式计算方案的“成本”总值：</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL固定成本]</td> 
   <td> <p><span style="font-weight: normal;">这是一个手动录入项，您可以在其中进行估算 <span>每月计划的固定成本金额。</span> 这不包括与添加到方案中的角色（在[!UICONTROL人员成本]字段中捕获）关联的成本。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL人员成本]</td> 
   <td> <p style="font-weight: normal;">这是该倡议期间与该倡议的工作角色有关的费用的总计。 此数字取决于您为计划每个月的工作角色估计的FTE或小时数。 </p> 
     <p><b>提示</b>  
     <ul> 
      <li> <p>同一工作角色的月FTE数量可能不同于月。</p> </li> 
      <li> <p>[!DNL Workfront] 认为一个月内有160个工作小时。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] 使用以下公式计算方案的[!UICONTROL人员成本]:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] 使用以下公式计算计划期间每月的每月人员成本：</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>示例</b></p>
      <p>如果您的计划持续时间为6个月，要求1个设计人员每月为1个FTE提供$50的每小时费率，而Web设计人员在计划的2个月内每小时费率为$100，则计划的人员成本计算如下：</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL计划收益]</td> 
   <td>这是一个手动输入项，您可以在此输入项中，通过完成此计划来估算部门将获得的总体好处。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL净值金额]</td> 
   <td> <p style="font-weight: normal;">这表示您的计划在考虑到计划的总体成本和计划福利时的价值。 [!DNL Workfront] 使用以下公式计算方案的净值：</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## 报告中的主动性信息

您可以在报表中显示方案信息，如下表所述。 此信息仅在您的公司购买了Workfront方案计划员许可证后，才可在Workfront实例中使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>报表类型</b></td> 
   <td><b>主动信息</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>名称、持续时间、开始和结束日期、输入者、ID、上次发布日期*、包括自定义字段在内的所有项目字段*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>上面列出的所有方案信息、（作业角色）ID、项目*、项目分配计划小时数*、方案作业角色小时数、（作业角色）计数、包括自定义字段的所有项目字段*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL项目]*</p></td> 
   <td> <p>上面列出的所有计划信息*</p> </td> 
  </tr> 
 </tbody> 
</table>

*只有在从项目创建或至少将方案发布到项目一次时，这些字段才会填充来自链接到方案的项目的信息。 有关发布计划的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
