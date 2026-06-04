---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 计算示例 — 以任务汇总的形式计算EAC
description: 本文提供了一个计算项目完工估算(EAC)的示例，此示例是从Adobe Workfront中项目的所有任务汇总而来。
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
TQID: https://experienceleague.adobe.com/O-A-9mMVMuqsnHXpph-J5Qwh6Qj5r46zxj7VG85rX04
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1155
ht-degree: 4%

---

# 计算示例 — 以任务汇总的形式计算EAC

## EAC方法：从任务或子任务汇总

* [PIM=基于小时](#pim-hour-based)
* [PIM=基于成本](#pim-cost-based)

### PIM=基于小时 {#pim-hour-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)
* [复杂的示例：项目具有子任务](#complicated-example-project-has-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks}

pim =基于小时

EAC方法=从任务/子任务汇总

1. 创建项目A，其中三个任务（无子任务）均分配给成本/小时为$100.00的用户1。
1. 根据下表将计划/实际小时数添加到每个任务中，并添加完成百分比：

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
1. 任务1 **的** CPI = .04计算如下：\
   任务1 **的** CPI = *IF*&#x200B;实际小时数> 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/实际小时数\
   *ELSE* CPI = 1\
   任务1的&#x200B;**CPI** = 1 / 25\
   任务1 **的** CPI = .04

1. 任务1 **的** EAC = 125小时，计算方式如下：\
   任务1的&#x200B;**EAC** = *IF* CPI &lt;> 0 *则* EAC =计划小时数/ CPI\
   *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   任务1 **的** EAC = 5 / .04\
   任务1 **的** EAC = 125小时

1. 任务2和3的CPI / EAC包括：\
   任务2 = .12 / 83.33小时\
   任务3 = .24 / 62.5小时

1. 项目&#x200B;**的** CPI = .13计算如下：\
   项目&#x200B;**CPI** = *IF*&#x200B;实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   项目&#x200B;**的** CPI = 10 / 75\
   项目&#x200B;**的** CPI = .13

1. **项目**&#x200B;的EAC = 270.83小时，计算如下\
   **项目的EAC** = EAC任务1 + EAC任务2 + EAC任务3\
   项目&#x200B;**EAC** = 125 + 83.33 + 62.5\
   项目&#x200B;**的** EAC = 270.83小时

#### 复杂的示例：项目具有子任务 {#complicated-example-project-has-children-tasks}

pim =基于小时

EAC方法=从任务/子任务汇总

1. 创建项目A，其中任务3是任务4和5的父级任务，任务1是任务2和3的父级任务，如下所示：

   ```
   Task 1  
      Task 2  
      Task 3  
         Task 4  
         Task 5  
   Task 6
   ```

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
      <td> </td> 
      <td> <p>10小时</p> </td> 
      <td> </td> 
   </tr> 
   <tr> 
      <td> <p>任务2</p> </td> 
      <td> <p>5小时</p> </td> 
      <td> <p>10小时</p> </td> 
      <td> <p>20%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>任务3</p> </td> 
      <td> </td> 
      <td> <p>10小时</p> </td> 
      <td> </td> 
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

1. 直接将50小时添加到项目（“更多”>“小时”>“记录小时”），以便将$5,000.00的实际人工成本直接记录到项目中。
1. 运行重新计算财务
1. 任务2 **的** CPI = .1计算如下：\
   任务2 **的** CPI = *IF*&#x200B;实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   任务2 **的** CPI = 1 / 10\
   任务2 **的** CPI = .1

1. 任务2 **的** EAC = 50小时，计算方式如下：\
   任务2 **的** EAC = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

   *ELSE* EAC =计划小时数+实际小时数\
   任务2 **的** EAC = 5 / .1\
   任务2 **的** EAC = 50小时

1. 任务4 、任务5和任务6的CPI / EAC ：\
   任务4 = .4 / 25小时\
   任务5 = .75 / 20小时\
   任务6 = 1.2 / 16.67小时

1. 任务3 **的** CPI = .38\
   任务3 **的** CPI = *IF*&#x200B;实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   任务3 **的** CPI = 11.5 / 30\
   任务3 **的** CPI = .38

1. 任务3 **的** EAC = EAC任务4 + EAC任务5\
   任务3 **的** EAC = 25 + 20\
   任务3 **的** EAC = 45小时

1. 任务1 **的** CPI = .25计算如下：\
   任务1 **的** CPI = *IF*&#x200B;实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   任务1的&#x200B;**CPI** = 12.5 / 50\
   任务1 **的** CPI = .25

1. 任务1的&#x200B;**EAC** = EAC任务2 + EAC任务3\
   任务1 **的** EAC = 50 + 45\
   任务1 **的** EAC = 95小时

1. 项目的CPI = .22，计算方法如下：\
   项目&#x200B;**CPI** = *IF*&#x200B;实际小时数> 0 *然后*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   项目&#x200B;**的** CPI = 24.5 / 110\
   项目&#x200B;**的** CPI = .22272\
   项目&#x200B;**的** CPI = .22

1. **项目**&#x200B;的EAC = EAC任务1 + EAC任务6\
   项目&#x200B;**的** EAC = 95 + 16.67\
   项目&#x200B;**的** EAC = 111.67小时

### PIM=基于成本 {#pim-cost-based}

* [简单示例：项目没有子任务](#simple-example-project-has-no-children-tasks)

#### 简单示例：项目没有子任务 {#simple-example-project-has-no-children-tasks-1}

PIM =基于成本

EAC方法=从任务/子任务汇总

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
      <td> <p>$300.00</p> </td> 
      <td> <p>$400.00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>任务1</p> </td> 
      <td> <p>任务1费用2</p> </td> 
      <td> <p>$500.00</p> </td> 
      <td> <p>$0.00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>任务2</p> </td> 
      <td> <p>任务2费用</p> </td> 
      <td> <p>$200.00</p> </td> 
      <td> <p>$100.00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>任务3</p> </td> 
      <td> <p>任务3费用</p> </td> 
      <td> <p>$800.00</p> </td> 
      <td> <p>$700.00</p> </td> 
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
      <td> <p>$1,000.00</p> </td> 
      <td> <p>$1,500.00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>任务1费用2</p> </td> 
      <td> <p>$2,500.00</p> </td> 
      <td> <p>$0.00</p> </td> 
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

1. 在项目操作中，运行重新计算财务
1. 任务1 **的** CPI**** = .14计算如下：\
   任务1 **的** CPI **** = *IF*实际劳力成本+ GeneratedActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     任务1 **** 1}的**CPI= (100+300) / (2500+400)**\
     任务1 **** 1}的**CPI= 400 / 2900**\
     任务1 **** 1}的**CPI = .14**

1. 任务1 **的** EAC**** = $13,400.00\
   任务1 **的** CPI人工****=如果实际人工成本&lt;> 0，则

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   否则CPI_Labor = 1\
   任务1 **** 1}的**CPI人工= 100/2500**\
   任务1 **** 1}的**CPI人工= .04**

   任务1 ****1}的&#x200B;**EAC人工= *IF* CPI_Labor &lt;> 0 *THEN***

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* EAC人力=计划人工成本+实际人工成本\
     **任务1****EAC人工= 500.00/.04**\
     **任务1**&#x200B;的EAC人工**** = $12,500.00

   任务1 **的** EAC费用**** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **任务1**&#x200B;的EAC费用**** = $400.00 + $500.00\
   任务1 **的** EAC费用**** = $900.00

   任务1 **的** EAC**** = EAC人工+ EAC费用\
   任务1 **的** EAC**** = $12,500.00 + $900.00\
   任务1 **的** EAC**** = $13,400.00

1. 以下是任务2和任务3的CPI / EAC值：\
   任务2 = .19 / $8,433.33\
   任务3 = .44 / $6,950.00****

1. 项目的CPI = .32\
   项目&#x200B;**CPI ****1} = *IF*实际劳力成本+ GeneratedActualExpenseCost &lt;> 0 *THEN***

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     项目&#x200B;**** 0}CPI** = (1000 + 2300) / (7500 + 2700)**\
     项目&#x200B;**** 1}的**CPI= 3300 / 10200**\
     项目&#x200B;********CPI = .32

1. 该项目的EAC为28,783.33美元\
   **项目EAC****** = EAC任务1 + EAC任务2 + EAC任务3\
   **项目****EAC** = $13,400.00 + $8,433.33 + $6,950.00\
   **项目****EAC** = $28,783.33
