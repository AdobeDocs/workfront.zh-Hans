---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 计算示例 — 在项目级别计算EAC
description: PIM =基于小时
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# 计算示例 — 在项目级别计算EAC

## EAC方法：在项目级别计算

* [PIM =基于小时](#pim-hour-based)
* [PIM=基于成本](#pim-cost-based)

### PIM =基于小时 {#pim-hour-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目包含子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks}

PIM =基于小时

EAC方法=在项目层计算****

1. 创建项目A，其中包含三项任务（无子任务），所有任务均分配给成本/小时为$100.00的用户1。
1. 将计划小时数和实际小时数添加到每个任务，并根据下表完成百分比：

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>任务</strong></p></th>
      <th><br><p><strong>计划小时</strong></p></th>
      <th><br><p><strong>实际小时数</strong></p></th>
      <th><p><strong>完成百分比</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>任务1</p></td>
      <td><p>5小时</p></td>
      <td><p>25小时</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>任务2</p></td>
      <td><p>10小时</p></td>
      <td><p>25小时</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>任务3</p></td>
      <td><p>15小时</p></td>
      <td><p>25小时</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. 对项目重新计算财务。
1. **任务1的CPI** = .04，计算如下：\
   **任务1的CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
      *ELSE* CPI = 1\
   **任务1的CPI** = 1 / 25\
   **任务1的CPI** = .04

1. **任务1的EAC** = 125小时计算如下：\
   **任务1的EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **任务1的EAC** = 5 / .04\
   **任务1的EAC** = 125小时****

1. 任务2和3的CPI/EAC包括：\
   任务2 = .12 / 83.33小时\
   任务3 = .24 / 62.5小时

1. **项目CPI** = .13，计算如下：\
   **项目CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **项目CPI** = 10 / 75\
   **项目CPI** = .13

1. **项目EAC** = 225小时计算如下：\
   **项目EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **项目EAC** = 30 / .13333\
   **项目EAC** = 225小时

#### 复杂的示例：项目包含子任务 {#complicated-example-project-has-children-tasks}

PIM =基于小时

EAC方法=在项目层计算

1. 创建项目A，其中任务3是任务4和5的父项，任务1是任务2和3的父项，如下所示：\
   任务1\
      任务2\
      任务3\
         任务4\
         任务5\
   任务6

1. 将任务2、4、5和6分配给成本/小时费率为$100.00的用户1。
1. 根据下表，添加每项任务的计划/实际小时数和完成百分比。

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

1. 将50小时直接添加到项目（更多>小时>日志小时）。
1. **任务2的CPI** = .1，计算如下：\
   **任务2的CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任务2的CPI** = 1 / 10\
   **任务2的CPI** = .1

1. **任务2的EAC** = 50小时计算如下：\
   **任务2的EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **任务2的EAC** = 5 / .1\
   **任务2的EAC** = 50小时

1. 任务4、5和6的CPI/EAC如下：\
   任务4:.4/25小时\
   任务5:.75 / 20小时\
   任务6:1.2小时/16时67分

1. **任务3的CPI** = .38的计算方式如下：\
   **任务3的CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任务3的CPI** = 11.5 / 30\
   **任务3的CPI** = .38

1. **任务3的EAC** = 65.22小时计算如下：\
   **任务3的EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **任务3的EAC** = 25 / .383333\
   **任务3的EAC** = 65.22小时

1. **任务1的CPI** = .25，计算如下：\
   **任务1的CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任务1的CPI** = 12.5 / 50\
   **任务1的CPI** = .25

1. **任务1的EAC** = 120小时计算如下：\
   **任务1的EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **任务1的EAC** = 30/.25\
   **任务1的EAC** = 120小时

1. **项目CPI** = .22，计算如下：\
   **项目CPI** = *如果* 实际小时数> 0 *然后* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **项目CPI** = 24.5 / 110\
   **项目CPI** = .22272\
   **项目CPI** = .22

1. **项目EAC** = 224.49小时计算如下：\
   **项目EAC** = *如果* CPI &lt;> 0 *然后* EAC =计划时数/CPI\
       *ELSE* EAC =计划小时数+实际小时数\
   **项目EAC** = 50 / .22272\
   **项目EAC** = 224.49小时

### PIM=基于成本 {#pim-cost-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目包含子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks-1}

PIM =基于成本

EAC方法=在项目层计算

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
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目活动中，运行重新计算财务
1. **任务1的CPI** = .14
1. **任务1的CPI****** = .14，计算如下：\
   **CPI**  **任务1** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **任务1的CPI****** =(100+300)/(2500+400)\
   **CPI**  **任务1** = 400 / 2900\
   **CPI**  **任务1**  = .14****

1. **任务1的EAC****** = 13,400.00美元\
   **CPI劳动力**  **任务1** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI劳动力**  **任务1** = 100/2500\
   **CPI劳动力**  **任务1** = .04 ****** EAC劳工&#x200B;****任务1 **=*如果&#x200B;*CPI_Labor &lt;> 0*然后&#x200B;*EAC人工=计划人工成本/CPI_人工\
   *    ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC劳工&#x200B;****对于任务1** = 500.00/.04\
   **任务1的EAC人工****** = 12,500.00美元\
   **任务1的EAC费用****** = ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **任务1的EAC费用****** = $400.00 + $500.00\
   **任务1的EAC费用****** = $900.00\
   **任务1的EAC****** = EAC人工+ EAC费用\
   **任务1的EAC******  = $12,500.00 + $900.00\
   **任务1的EAC******  = 13,400.00美元

1. 以下是任务2和任务3的CPI/EAC值：\
   任务2 = .19 / $8,433.33\
   任务3 = .44 / $6,950.00

1. **项目CPI** = .32，计算如下：\
   **项目的CPI****** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **项目的CPI****** =(1000 + 2300)/(7500 + 2700)\
   **项目的CPI****** = 3300 / 10200\
   **项目的CPI****** = .32

1. **项目EAC** = $28,200.00，计算如下：\
   **CPI Labor**** for Project** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 1000 / 7500\
   **CPI Labor**** for Project** = .13333\
   **CPI Labor**** for Project** = .13

   **EAC Labor**** for Project** = *如果* CPI_Labor &lt;> 0 *然后*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC Labor**** for Project** = 3000/.13333\
   **EAC Labor**** for Project** = $22,500.00

   **EAC费用****项目** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC费用****项目** = $3000.00 + 2,700.00\
   **EAC费用****项目** = $5,700.00

   **EAC****项目** = EAC人工+ EAC费用\
   **EAC****项目**  = $22,500.00 + $5,700.00\
   **EAC****项目**  = $28,200.00

#### 复杂的示例：项目包含子任务 {#complicated-example-project-has-children-tasks-1}

PIM =基于成本

EAC方法=在项目层计算

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
   <td> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>20小时</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 将50小时直接添加到项目（“更多”>“小时”>“日志小时数”），这样实际人工成本就有$5,000.00直接记录到项目中。 ****
1. 根据下表为每项任务添加费用（我已在每项任务之间添加一个空白行，以便更便于阅读）：

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
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2 Exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>任务3扩展</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>任务4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>任务4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4 </p> </td> 
   <td> <p>任务4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5 Exp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5 Exp 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>任务6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>任务6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <td> <p> $0.00 <strong></strong></p> </td> 
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
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目活动中，运行重新计算财务
1. **CPI** 对于任务2 = .17，计算如下：\
   **CPI任务2** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后* CPI =(TotalBudgetedCostWorkPerformed + ExceedPlanededExpenseCost)/(ActualLaborCost + ExceedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****任务2** =(100+300)/(1000+1300)\
   **CPI****任务2**  = 400 / 2300\
   **CPI****任务2**  = .17

1. **EAC** 对于任务2 = $5,900.00\
   **CPI劳工****任务2** =如果实际人工成本&lt;> 0，则CPI_人工= TotalBudgededCostWorkPerformed /实际人工成本\
      ELSE CPI_Labor = 1\
   **CPI劳工****任务2** = 100/1000\
   **CPI劳工****任务2** = .1

   **EAC劳工****任务2** = *如果* CPI_Labor &lt;> 0 *然后*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC劳工****任务2** = 500.00/.1\
   **EAC劳工****任务2** = $5,000.00 ****** EAC费用&#x200B;****任务2 **= ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **EAC费用&#x200B;****任务2** = $1,300.00 + - $400.00\
   **EAC费用****任务2** = $900.00

   **EAC****任务2** = EAC人工+ EAC费用\
   **EAC****任务2**  = $5,000.00 + $900.00\
   **EAC****任务2**  = $5,900.00

1. 任务4、5和6的CPI/EAC的确定方式相同，因此我将提供以下值：\
   任务4:.23 / 3,400.00美元\
   任务5:.64 / 3,100.00美元\
   任务6:1.06 / 2,366.67美元

1. 任务3的CPI = .31，计算如下：\
   **CPI****任务3** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任务3**  =(1,150 + 500)/(3000 + 2400)\
   **CPI****任务3**  = 1650 / 5400\
   **CPI****任务3**  = .31 ******&#x200B;任务3的EAC **= $9,521.74，计算如下：\
   **CPI劳工&#x200B;****任务3** = IF实际人工成本&lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI劳工****任务3** = 1150/3000\
   **CPI劳工****任务3** = .383333\
   **CPI劳工****任务3** = .38

   **EAC劳工****任务3** = *如果* CPI_Labor &lt;> 0 *然后*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC劳工****任务3** = $2,500.00 / .383333\
   **EAC劳工****任务3** = $6,521.74

   **EAC费用****任务3** = ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **EAC费用****任务3** = $2,400.00 + $600.00\
   **EAC费用****任务3** = $3,000.00

   **EAC****任务3** = EAC人工+ EAC费用\
   **EAC****任务3**  = $6,521.74 + $3,000.00\
   **EAC****任务3**  = $9,521.74

1. 任务1的CPI = .16，计算如下：\
   **CPI****任务1** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任务1**  =(1250 + 300)/(5000 + 4500)\
   **CPI****任务1**  = 1550 / 9500=\
   **CPI****任务1**  = .16

1. 任务1的EAC为$17,100.00，计算如下：\
   **CPI劳工****任务1** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI劳工****任务1** = 1250 / 5000\
   **CPI劳工****任务1** = .25

   **EAC Labor****任务1** = *如果* CPI_Labor &lt;> 0 *然后* EAC人工=计划人工成本/CPI_人工\
   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC Labor****任务1** = $3,000.00 / .25\
   **EAC Labor****任务1** = 12,000.00美元

   **EAC费用****任务1** = ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **EAC费用****任务1** = $4500 + 600\
   **EAC费用****任务1** = $5,100.00

   **EAC****任务1** = EAC人工+ EAC费用\
   **EAC****任务1**  = $12,000.00 + 5,100.00\
   **EAC****任务1**  = 17,100.00美元

1. 项目的CPI为。25\
   **项目的CPI****** = *如果* 实际人工成本+已发生实际费用成本&lt;> 0 *然后*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **项目的CPI****** =(2450 + 1900)/(11000 + 6700)\
   **项目的CPI****** = 4350 / 17700\
   **项目的CPI****** = .25

1. **项目EAC** = $32,248.98，计算如下：\
   **CPI Labor**** for Project** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 2450 / 11000\
   **CPI Labor**** for Project** = .22272\
   **CPI Labor**** for Project** = .22

   **EAC Labor**** for Project** = *如果* CPI_Labor &lt;> 0 *然后*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=计划人工成本+实际人工成本\
   **EAC Labor**** for Project** = $5,000.00 / .22272\
   **EAC Labor**** for Project** = $22,448.97959\
   **EAC Labor**** for Project** = $22,448.98

   **EAC费用****项目** = ExcuredActualExpenseCost + NotExcuredPlanedExpense\
   **EAC费用****项目** = $3,100.00 + $6,700.00\
   **EAC费用****项目** = $9,800.00

   **EAC****项目** = EAC人工+ EAC费用\
   **EAC****项目**  = $22,448.98 + 9,800.00\
   **EAC****项目**  = $32,248.98
