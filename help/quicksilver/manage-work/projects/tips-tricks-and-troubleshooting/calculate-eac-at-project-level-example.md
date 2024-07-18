---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 计算示例 — 在项目级别计算EAC
description: pim =基于小时
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# 计算示例 — 在项目级别计算EAC

## EAC方法：在项目级别计算

* [PIM =基于小时](#pim-hour-based)
* [PIM=基于成本](#pim-cost-based)

### pim =基于小时 {#pim-hour-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目具有子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks}

pim =基于小时

EAC方法=在项目级别计算****

1. 创建项目A，其中三个任务（无子任务）均分配给成本/小时为$100.00的用户1。
1. 根据下表将计划小时数和实际小时数添加到每个任务并完成百分比：

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

1. 重新计算项目财务。
1. 任务1 **的** CPI = .04计算如下：\
   任务1 **的** CPI = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
      *ELSE* CPI = 1\
   任务1的&#x200B;**CPI** = 1 / 25\
   任务1 **的** CPI = .04

1. 任务1 **的** EAC = 125小时，计算方式如下：\
   任务1的&#x200B;**EAC** = *IF* CPI &lt;> 0 *则* EAC =计划小时数/CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   任务1 **的** EAC = 5 / .04\
   任务1 **的** EAC = 125小时****

1. 任务2和3的CPI / EAC包括：\
   任务  2 = .12 / 83.33  小时\
   任务3 = .24 / 62.5小时

1. 项目&#x200B;**的** CPI = .13计算如下：\
   项目&#x200B;**CPI** = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
       *ELSE* CPI = 1\
   项目&#x200B;**的** CPI = 10 / 75\
   项目&#x200B;**的** CPI = .13

1. **项目**&#x200B;的EAC = 225小时，计算方式如下：\
   项目&#x200B;**EAC** = *IF* CPI &lt;> 0 *然后* EAC =计划小时数/CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   项目&#x200B;**的** EAC = 30 / .13333\
   项目&#x200B;**的** EAC = 225小时

#### 复杂的示例：项目具有子任务 {#complicated-example-project-has-children-tasks}

pim =基于小时

EAC方法=在项目级别计算

1. 创建项目A，其中任务3是任务4和5的父级任务，任务1是任务2和3的父级任务，如下所示：\
   任务1\
      任务2\
      任务3\
         任务4\
         任务5\
   任务6

1. 将任务2、4、5和6分配给成本/小时费率为$100.00的用户1。
1. 根据下表添加每个任务的计划/实际小时数和完成百分比。

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
   <th> <p>完成<strong>%</strong> </p> </th> 
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

1. 直接将50小时添加到项目（“更多”>“小时”>“记录小时”）。
1. 任务2 **的** CPI = .1计算如下：\
   任务2 **的** CPI = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
       *ELSE* CPI = 1\
   任务2 **的** CPI = 1 / 10\
   任务2 **的** CPI = .1

1. 任务2 **的** EAC = 50小时，计算方式如下：\
   任务2的&#x200B;**EAC** = *IF* CPI &lt;> 0 *则* EAC =计划小时数/CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   任务2 **的** EAC = 5 / .1\
   任务2 **的** EAC = 50小时

1. 任务4 、 5和6的CPI / EAC如下所示：\
   任务4：.4/25小时\
   任务5：.75/20小时\
   任务6:1.2/16.67小时

1. 任务3 **的** CPI = .38  计算如下：\
   任务3 **的** CPI = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
       *ELSE* CPI = 1\
   任务3 **的** CPI = 11.5 / 30\
   任务3 **的** CPI = .38

1. 任务3 **的** EAC = 65.22小时，计算如下：\
   任务3 **的** EAC = *IF* CPI &lt;> 0 *THEN* EAC =计划小时数/CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   任务3 **的** EAC =  25 / .383333\
   任务3 **的** EAC = 65.22小时

1. 任务1 **的** CPI = .25计算如下：\
   任务1 **的** CPI = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
       *ELSE* CPI = 1\
   任务1的&#x200B;**CPI** = 12.5 / 50\
   任务1 **的** CPI = .25

1. 任务1 **的** EAC = 120小时，计算方式如下：\
   任务1的&#x200B;**EAC** = *IF* CPI &lt;> 0 *则* EAC =计划小时数/ CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   任务1 **的** EAC =  30/ .25\
   任务1 **的** EAC = 120小时

1. 项目&#x200B;**的** CPI = .22计算如下：\
   项目&#x200B;**CPI** = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
       *ELSE* CPI = 1\
   项目&#x200B;**的** CPI = 24.5 / 110\
   项目&#x200B;**的** CPI = .22272\
   项目&#x200B;**的** CPI = .22

1. 项目&#x200B;**的** EAC = 224.49  小时数计算如下：\
   项目&#x200B;**EAC** = *IF* CPI &lt;> 0 *然后* EAC =计划小时数/CPI\
       *ELSE* EAC =计划  小时+实际  小时\
   项目&#x200B;**的** EAC =  50 / .22272\
   项目&#x200B;**的** EAC = 224.49小时

### PIM=基于成本 {#pim-cost-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目具有子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks-1}

PIM =基于成本

EAC方法=在项目级别计算

1. 创建项目A，其中三个任务（无子任务）均分配给成本/小时为$100.00的用户1。
1. 根据下表将计划/实际小时数添加到每个任务中，并添加完成百分比：

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
   <th> <br> <p><strong>计划劳力成本</strong> </p> </th> 
   <th> <br> <p><strong>实际小时数</strong> </p> </th> 
   <th> <br> <p><strong>实际劳力成本</strong> </p> </th> 
   <th> <p>完成<strong>%</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>1,500美元</p> </td> 
   <td> <p>25小时</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根据下表将费用添加到每项任务：

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
   <td> <p>任务1费用1</p> </td> 
   <td> <p>300.00</p> </td> 
   <td> <p>400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1费用2</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2费用</p> </td> 
   <td> <p>200.00</p> </td> 
   <td> <p>100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>任务3费用</p> </td> 
   <td> <p>800.00</p> </td> 
   <td> <p>700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 将两个费用添加到项目（即不绑定到任务），如下所示：

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
   <td> <p>项目费用1</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>1,500美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1费用2</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根据上述价值，已产生/未产生成本之厘定如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务</strong> </p> </th> 
   <th> <p><strong>未发生计划费用</strong> </p> </th> 
   <th> <p><strong>发生计划费用</strong> </p> </th> 
   <th> <p><strong>发生实际费用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>300.00</p> </td> 
   <td> <p>400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>200.00</p> </td> 
   <td> <p>100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>800.00</p> </td> 
   <td> <p>700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>3,000美元</p> </td> 
   <td> <p>2,300美元</p> </td> 
   <td> <p> 2,700美元 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目操作中，运行重新计算财务
1. 任务1 **的** CPI = .14
1. 任务1 **的** CPI**** = .14计算如下：\
   **CPI**  任务1 **的** = *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   任务1****1}的&#x200B;**CPI= (100+300) / (2500+400)**\
   **CPI**  任务1 **的** = 400 / 2900\
   **CPI**  任务1 **的**  = .14****

1. 任务1 **的** EAC**** = $13,400.00\
   **CPI人工**  任务1 **的** =如果实际劳力成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      否则CPI_Labor = 1\
   **CPI人工**  任务1 **的** = 100/2500\
   **CPI人工**  **对于任务1** = .04 ****** EAC人力&#x200B;****对于任务1 **=*IF *CPI_Labor &lt;> 0*THEN *EAC人力=计划人工成本/CPI_Labor\
   *    ELSE* EAC  人工=计划人工成本+实际人工成本\
   任务1的**EAC人工&#x200B;****** = 500.00/.04\
   **任务1**&#x200B;的EAC人工**** = $12,500.00\
   任务1 **的** EAC费用**** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **任务1**&#x200B;的EAC费用**** = $400.00 + $500.00\
   任务1 **的** EAC费用**** = $900.00\
   任务1 **的** EAC**** = EAC人工+ EAC费用\
   任务1 **的** EAC****  = $12,500.00 + $900.00\
   任务1 **的** EAC****  = $13,400.00

1. 以下是任务2和任务3的CPI / EAC值：\
   任务2 = .19 / $8,433.33\
   任务3 = .44 / $6,950.00

1. 项目&#x200B;**的** CPI = .32计算如下：\
   项目&#x200B;**的** CPI****= *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   项目****0}CPI **= (1000 + 2300) / (7500 + 2700)**\
   项目****1}的&#x200B;**CPI= 3300 / 10200**\
   项目&#x200B;******** CPI = .32

1. **项目**&#x200B;的EAC = $28,200.00，计算方法如下：\
   **项目****1}的CPI人工=如果实际人工成本&lt;> 0，则**

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      否则CPI_Labor = 1\
   **项目****CPI人工** = 1000 / 7500\
   **项目****CPI人工** = .13333\
   **项目****CPI人工** = .13

   **项目****1}的EAC人工= *IF* CPI_Labor &lt;> 0 *THEN***

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  人工=计划人工成本+实际人工成本\
   **项目****EAC人工** = 3000/ .13333\
   **项目****EAC人工** = $22,500.00

   **EAC费用****项目** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC费用****项目** = $3000.00 + 2,700.00\
   **EAC费用****项目** = $5,700.00

   **EAC****项目** = EAC人工+ EAC费用\
   **EAC****项目**  = $22,500.00 + $5,700.00\
   **EAC****项目**  = $28,200.00

#### 复杂的示例：项目具有子任务 {#complicated-example-project-has-children-tasks-1}

PIM =基于成本

EAC方法=在项目级别计算

1. 创建项目A，其中任务3是任务4和5的父级任务，任务1是任务2和3的父级任务，如下所示：\
   任务1\
      任务2\
      任务3\
         任务4\
         任务5\
   任务6

1. 将任务2、4、5和6分配给成本/小时费率为$100.00的用户1。
1. 根据下表添加每个任务的计划/实际小时数和完成百分比。

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
   <th> <br> <p><strong>计划劳力成本</strong> </p> </th> 
   <th> <br> <p><strong>实际小时数</strong> </p> </th> 
   <th> <br> <p><strong>实际劳力成本</strong> </p> </th> 
   <th> <p>完成<strong>%</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>5小时</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>15小时</p> </td> 
   <td> <p>1,500美元</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>20小时</p> </td> 
   <td> <p>2,000.00美元</p> </td> 
   <td> <p>10小时</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 直接将50小时添加到项目（“更多”>“小时”>“记录小时”），以便将$5,000.00的实际人工成本直接记录到项目中。 ****
1. 根据下表为每个任务添加费用（为了便于阅读，我在每个任务之间添加了一行空白）：

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
   <td> <p>任务1费用1</p> </td> 
   <td> <p>300.00</p> </td> 
   <td> <p>- 400.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1费用2</p> </td> 
   <td> <p>- 500.00美元</p> </td> 
   <td> <p>800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>任务1费用3</p> </td> 
   <td> <p>400.00</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2费用1</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2费用2</p> </td> 
   <td> <p>- 400.00美元</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2费用3</p> </td> 
   <td> <p>- 200.00美元</p> </td> 
   <td> <p>600.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>任务2费用4</p> </td> 
   <td> <p>700.00</p> </td> 
   <td> <p>- 200.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>任务3费用</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>1,000美元</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>任务4费用1</p> </td> 
   <td> <p>800.00</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>任务4费用2</p> </td> 
   <td> <p>- 100.00美元</p> </td> 
   <td> <p>300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4 </p> </td> 
   <td> <p>任务4费用3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>0.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5费用1</p> </td> 
   <td> <p>700.00</p> </td> 
   <td> <p>800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5费用2</p> </td> 
   <td> <p>- 100.00美元</p> </td> 
   <td> <p>300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>任务5费用3</p> </td> 
   <td> <p>- 400.00美元</p> </td> 
   <td> <p>- 200.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>任务6费用1</p> </td> 
   <td> <p>600.00美元</p> </td> 
   <td> <p>700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>任务6费用2</p> </td> 
   <td> <p>500.00美元</p> </td> 
   <td> <p>- 300.0美元</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 将两个费用添加到项目（即不绑定到任务），如下所示：

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
   <td> <p>项目费用1</p> </td> 
   <td> <p>1,000美元</p> </td> 
   <td> <p>1,500美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务1费用2</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p> 0.00美元 <strong></strong></p> </td> 
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
   <th> <p><strong>未发生计划费用</strong> </p> </th> 
   <th> <p><strong>发生计划费用</strong> </p> </th> 
   <th> <p><strong>发生实际费用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任务1</p> </td> 
   <td> <p>400.00</p> </td> 
   <td> <p>- 500.00美元</p> </td> 
   <td> <p>800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务2</p> </td> 
   <td> <p>- 400.00美元</p> </td> 
   <td> <p>300.00</p> </td> 
   <td> <p>1,300美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务3</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>1,000美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务4</p> </td> 
   <td> <p>600.00美元</p> </td> 
   <td> <p>- 100.00美元</p> </td> 
   <td> <p>300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务5</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>600.00美元</p> </td> 
   <td> <p>1,100.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任务6</p> </td> 
   <td> <p>0.00美元</p> </td> 
   <td> <p>600.00美元</p> </td> 
   <td> <p>700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>项目</p> </td> 
   <td> <p>2,500美元</p> </td> 
   <td> <p>1000.00</p> </td> 
   <td> <p>1,500美元</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在项目操作中，运行重新计算财务
1. 任务2的&#x200B;**CPI** = .17计算如下：\
   **CPI任务2** = *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + GeneratedPlannedExpenseCost) / (ActualLaborCost + GeneratedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****任务2** = (100+300) / (1000+1300)\
   **CPI****任务2**  = 400 / 2300\
   **CPI****任务2**  = .17

1. 任务2的&#x200B;**EAC** = $5,900.00\
   **CPI劳力****任务2** =如果实际劳力成本&lt;> 0，则CPI_劳力= TotalBudgetedCostWorkPerformed /实际劳力成本\
      否则CPI_Labor = 1\
   **CPI人工****任务2** = 100/1000\
   **CPI人工****任务2** = .1

   **EAC人工****任务2** = *IF* CPI_人工&lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  人工=计划人工成本+实际人工成本\
   **EAC人工****任务2** = 500.00/.1\
   **EAC人工****任务2** = $5,000.00 ****** EAC费用&#x200B;****任务2 **= GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC费用&#x200B;****任务2** = $1,300.00 + -$400.00\
   **EAC费用****任务2** = $900.00

   **EAC****任务2** = EAC人工+ EAC费用\
   **EAC****任务2**  = $5,000.00 + $900.00\
   **EAC****任务2**  = $5,900.00

1. 任务4、5和6的CPI/EAC采用相同的方式确定，因此我将提供以下这些值：\
   任务4： .23 / $3,400.00\
   任务5： .64 / $3,100.00\
   任务6:1.06 / $2,366.67

1. 任务3的CPI = .31，计算方法如下：\
   **CPI****任务3** = *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任务3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI****任务3**  =  1650 / 5400\
   **CPI****任务3**  = .31 ******&#x200B;任务3 **的EAC = $9,521.74计算如下：\
   **CPI人工&#x200B;****任务3** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否则CPI_Labor = 1\
   **CPI人工****任务3** = 1150/3000\
   **CPI人工****任务3** = .383333\
   **CPI人工****任务3** = .38

   **EAC人工****任务3** = *IF* CPI_人工&lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  人工=计划人工成本+实际人工成本\
   **EAC人工****任务3** = $2,500.00 / .383333\
   **EAC人工****任务3** = $6,521.74

   **EAC费用****任务3** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC费用****任务3** = $2,400.00 + $600.00\
   **EAC费用****任务3** = $3,000.00

   **EAC****任务3** = EAC人工+ EAC费用\
   **EAC****任务3**  = $6,521.74 + $3,000.00\
   **EAC****任务3**  = 9,521.74美元

1. 任务1的CPI = .16，计算方法如下：\
   **CPI****任务1** = *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任务1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****任务1**  =  1550 / 9500=\
   **CPI****任务1**  = .16

1. 任务1的EAC为$17,100.00，计算如下：\
   **CPI人工****任务1** =如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否则CPI_Labor = 1\
   **CPI人工****任务1** = 1250 / 5000\
   **CPI人工****任务1** = .25

   **EAC人工****任务1** = *IF* CPI_人工&lt;> 0 *THEN* EAC人工=计划人工成本/ CPI_人工\
   *   ELSE* EAC  人工=计划人工成本+实际人工成本\
   **EAC人工****任务1** = $3,000.00 / .25\
   **EAC人工****任务1** = $12,000.00

   **EAC费用****任务1** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC费用****任务1** = $4500 + 600\
   **EAC费用****任务1** = $5,100.00

   **EAC****任务1** = EAC人工+ EAC费用\
   **EAC****任务1**  = $12,000.00 + 5,100.00\
   **EAC****任务1**  = $17,100.00

1. 项目的CPI为0.25\
   项目&#x200B;**的** CPI****= *IF*&#x200B;实际劳力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   项目&#x200B;**CPI****1} = (2450 + 1900) / (11000 + 6700)**\
   项目****1}的&#x200B;**CPI=   4350 / 17700**\
   项目&#x200B;******** CPI = .25

1. **项目**&#x200B;的EAC = $32,248.98，计算方法如下：\
   **项目****1}的CPI人工=如果实际人工成本&lt;> 0，则**

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否则CPI_Labor = 1\
   **项目****CPI人工** = 2450 / 11000\
   **项目****CPI人工** = .22272\
   **项目****CPI人工** = .22

   **项目****1}的EAC人工= *IF* CPI_Labor &lt;> 0 *THEN***

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  人工=计划人工成本+实际人工成本\
   **项目****EAC人工** = $5,000.00 / .22272\
   **项目****EAC人工** = $22,448.97959\
   **项目****EAC人工** = $22,448.98

   **EAC费用****项目** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC费用****项目** = $3,100.00 + $6,700.00\
   **EAC费用****项目** = $9,800.00

   **EAC****项目** = EAC人工+ EAC费用\
   **EAC****项目**  = $22,448.98 + 9,800.00\
   **EAC****项目**  = 32,248.98美元
