---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算成本绩效指数(CPI)
description: 成本绩效指数(CPI)描述了项目或任务层的计划成本与实际成本之间的关系。 项目经理审查此量度，以确定当前在给定时间点跟踪成本不足或超过成本的任务或项目。
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a411c1ddf0c6d19dc7f6e181cceeebba5504530c
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 计算成本绩效指数(CPI)

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

成本绩效指数(CPI)描述了项目或任务层的计划成本与实际成本之间的关系。 项目经理审查此量度，以确定当前在给定时间点跟踪成本不足或超过成本的任务或项目。 成本可以用小时或美元来衡量，具体取决于您的绩效指数方法(PIM)。 有关设置绩效指数方法的详细信息，请参阅[设置绩效指数方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md)。

只有需要输入时间的组织才能使用CPI。 此外，基于成本的PIM值只有在为任务受分配人（职务角色或用户）定义了成本费率的组织中才准确。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：浅色或更高</p>
   <p>或</p>
   <p>当前：审阅或更高版本</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>查看对项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>具有查看财务的权限的项目的查看权限或更高权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 成本绩效指数(CPI)概览

### CPI值 {#the-cpi-value}

项目经理明白，CPI值为1意味着项目完全符合预算。 大于1的值表示项目预算不足（记录的小时数或费用比最初计划的少），而小于1的值表示项目预算超支（记录的小时数或费用比最初计划的多）。 与1越远，与计划的偏差越大。

| **CPI值** | **预算指示** |
|---|---|
| 1 | 按计划或预算 |
| > 1（大于1） | 低于预算 |
| &lt; 1（小于1） | 超出预算 |


### CPI的计算方式 {#how-cpi-is-calculated}

在Adobe Workfront中，CPI的计算取决于为项目选择的绩效指数方法。 有关设置绩效指数方法的详细信息，请参阅[设置绩效指数方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md)。

* 使用基于小时的PIM时进行[CPI计算](#cpi-calculations-when-using-hour-based-pim)
* [使用基于成本的PIM时的CPI计算](#cpi-calculations-when-using-cost-based-pim)

#### 使用基于小时的PIM时的CPI计算 {#cpi-calculations-when-using-hour-based-pim}

如果

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

否则

```
CPI = 1
```

* **对于非父级任务：**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **对于父任务：**
已执行的总预算成本工作=所有直接子任务的“已执行的总预算成本工作”字段的总和。

* 项目&#x200B;**：**
已执行的预算成本工时总计=所有顶层任务（父任务和独立任务）的已执行预算成本工时总计字段的总和。

有关已执行总预算成本工作(BCWP)的信息，请参阅[计算已执行预算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md)。

#### 使用基于成本的PIM时的CPI计算 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

如果

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



否则

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

此计算中的字段说明如下：

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

发生费用是实际成本> 0的费用

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 已执行工作的计划成本按以下公式计算：

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

已执行的总预算成本工作计算如下：

* **对于非父级任务：**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **对于父任务：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* 项目&#x200B;**：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top-level tasks)
  ```



## 在项目或任务中查找CPI

您可以在项目、任务列表或报告中显示项目或任务的CPI。 此外，您还可以在项目或任务级别查看它。

1. 转到要查看其CPI的项目或任务。
1. 在左侧面板中展开&#x200B;**项目详细信息**&#x200B;或&#x200B;**任务详细信息**，具体取决于您查看的是项目还是任务的CPI。

1. 单击&#x200B;**财务**。 CPI显示在&#x200B;**CPI/ SPI/ CSI**&#x200B;字段中。

   项目](assets/cpi-on-project-nwe.png)上的![CPI
