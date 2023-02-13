---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 计算示例 — 从任务中计算EAC作为汇总
description: PIM =基于小时
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# 计算示例 — 从任务中计算EAC作为汇总

## EAC方法：从任务或子任务汇总

* [PIM=基于小时](#pim-hour-based)
* [PIM=基于成本](#pim-cost-based)

### PIM=基于小时 {#pim-hour-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目包含子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks}

PIM =基于小时

EAC方法=从任务/子任务汇总

1. 创建项目A，其中包含三项任务（无子任务），所有任务均分配给成本/小时为$100.00的用户1。
1. 根据下表，将计划/实际工时添加到每个任务，并完成%:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任务</strong> </p> </th> 
   <th> <br> <p><strong>计划小时</strong> </p> </th> 
   <th> <br> <p><strong>实际小时数</strong> </p> </th> 
   <th> <p><strong>% 完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 重新计算财务
1. **任务1的CPI** = .04，计算如下：\
   **任务1的CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任务1的CPI** = 1 / 25\
   **任务1的CPI** = .04

1. **任务1的EAC** = 125小时计算如下：\
   **任务1的EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **任务1的EAC** = 5 / .04\
   **任务1的EAC** = 125小时

1. 任务2和3的CPI/EAC包括：\
   任务2 = .12 / 83.33小时\
   任务3 = .24 / 62.5小时

1. **项目CPI** = .13，计算如下：\
   **项目CPI** = *如果* 实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **项目CPI** = 10 / 75\
   **项目CPI** = .13

1. **项目EAC** = 270.83小时，计算如下\
   **项目EAC** = EAC任务1 + EAC任务2 + EAC任务3\
   **项目EAC** = 125 + 83.33 + 62.5\
   **项目EAC** = 270.83小时

#### 复杂的示例：项目包含子任务 {#complicated-example-project-has-children-tasks}

PIM =基于小时

EAC方法=从任务/子任务汇总

1. 创建项目A，其中任务3是任务4和5的父项，任务1是任务2和3的父项，如下所示：\
   任务1\
      任务2\
      任务3\
         任务4\
         任务5\
   任务6

1. 将任务2、4、5和6分配给成本/小时费率为$100.00的用户1。
1. 根据下表，添加每个任务的计划/实际小时数和完成百分比。

   >[!NOTE]
   >
   >对于任务1和3，您只添加实际小时数。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任务</strong> </p> </th> 
   <th> <br> <p><strong>计划小时</strong> </p> </th> 
   <th> <br> <p><strong>实际小时数</strong> </p> </th> 
   <th> <p><strong>% 完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>20小时</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 将50小时直接添加到项目（“更多”>“小时”>“日志小时数”），这样实际人工成本就有$5,000.00直接记录到项目中。
1. 运行重新计算财务
1. **任务2的CPI** = .1，计算如下：\
   **任务2的CPI** = *如果* 实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任务2的CPI** = 1 / 10\
   **任务2的CPI** = .1

1. **任务2的EAC** = 50小时计算如下：\
   **任务2的EAC** = *如果* CPI &lt;> 0 *然后*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC =计划小时数+实际小时数\
   **任务2的EAC** = 5 / .1\
   **任务2的EAC** = 50小时

1. 任务4、任务5和任务6的CPI/EAC :\
   任务4 = .4 / 25小时\
   任务5 = .75 / 20小时\
   任务6 = 1.2 / 16.67小时

1. **任务3的CPI** = .38\
   **任务3的CPI** = *如果* 实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任务3的CPI** = 11.5 / 30\
   **任务3的CPI** = .38

1. **任务3的EAC** = EAC任务4 + EAC任务5\
   **任务3的EAC** = 25 + 20\
   **任务3的EAC** = 45小时

1. **任务1的CPI** = .25，计算如下：\
   **任务1的CPI** = *如果* 实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任务1的CPI** = 12.5 / 50\
   **任务1的CPI** = .25

1. **任务1的EAC** = EAC任务2 + EAC任务3\
   **任务1的EAC** = 50 + 45\
   **任务1的EAC** = 95小时

1. 项目的CPI = .22，计算如下：\
   **项目CPI** = *如果* 实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **项目CPI** = 24.5 / 110\
   **项目CPI** = .22272\
   **项目CPI** = .22

1. **项目的EAC** = EAC任务1 + EAC任务6\
   **项目的EAC** = 95 + 16.67\
   **项目的EAC** = 111.67小时

### PIM=基于成本 {#pim-cost-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks-1}

PIM =基于成本

EAC方法=从任务/子任务汇总

1. 创建项目A，其中包含三项任务（无子任务），所有任务均分配给成本/小时为$100.00的用户1。
1. 根据下表，将计划/实际工时添加到每个任务，并完成%:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任务</strong> </p> </th> 
   <th> <br> <p><strong>计划小时</strong> </p> </th> 
   <th> <br> <p><strong>Pln Lbr成本</strong> </p> </th> 
   <th> <br> <p><strong>实际小时数</strong> </p> </th> 
   <th> <br> <p><strong>Act Lbr成本</strong> </p> </th> 
   <th> <p><strong>% 完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根据下表，向每项任务添加费用：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务</strong> </p> </th> 
   <th> <p><strong>费用</strong> </p> </th> 
   <th> <p><strong>计划数量</strong> </p> </th> 
   <th> <p><strong>实际数量</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2扩展</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>任务3扩展</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目中添加两项费用（即未与任务绑定），如下所示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>费用</strong> </p> </th> 
   <th> <p><strong>计划数量</strong> </p> </th> 
   <th> <p><strong>实际数量</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>项目扩展1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根据上述价值，已产生/未产生成本厘定如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务</strong> </p> </th> 
   <th> <p><strong>未产生计划费用</strong> </p> </th> 
   <th> <p><strong>已发生的计划费用</strong> </p> </th> 
   <th> <p><strong>已发生实际费用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目活动中，运行重新计算财务
1. **任务1的CPI****** = .14，计算如下：\
   **任务1的CPI******  = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **任务1的CPI******  =(100+300)/(2500+400)\
   **任务1的CPI******  = 400 / 2900\
   **任务1的CPI******  = .14

1. **任务1的EAC****** = 13,400.00美元\
   **任务1的CPI Labor****** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **任务1的CPI Labor****** = 100/2500\
   **任务1的CPI Labor****** = .04

   **任务1的EAC人工****** = *如果* CPI_Labor &lt;> 0 *然后*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **任务1的EAC人工****** = 500.00/.04\
   **任务1的EAC人工****** = 12,500.00美元

   **任务1的EAC费用****** = ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **任务1的EAC费用****** = $400.00 + $500.00\
   **任务1的EAC费用****** = $900.00

   **任务1的EAC****** = EAC人工+ EAC费用\
   **任务1的EAC******  = $12,500.00 + $900.00\
   **任务1的EAC******  = 13,400.00美元

1. 以下是任务2和任务3的CPI/EAC值：\
   任务2 = .19 / $8,433.33\
   任务3 = .44 / $6,950.00****

1. 项目的CPI = .32\
   **项目的CPI****** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **项目的CPI****** =(1000 + 2300)/(7500 + 2700)\
   **项目的CPI****** = 3300 / 10200\
   **项目的CPI****** = .32

1. 该项目的EAC为28,783.33美元\
   **项目EAC****** = EAC任务1 + EAC任务2 + EAC任务3\
   **项目EAC****** = $13,400.00 + $8,433.33 + $6,950.00\
   **项目EAC****** = $28,783.33
