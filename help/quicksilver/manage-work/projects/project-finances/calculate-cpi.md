---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算成本绩效指数(CPI)
description: 成本绩效指数(CPI)描述项目或任务层计划成本与实际成本之间的关系。 项目经理会审核此量度，以确定在给定时间点当前在成本或成本过高下跟踪的任务或项目。
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# 计算成本绩效指数(CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

成本绩效指数(CPI)描述项目或任务层计划成本与实际成本之间的关系。 项目经理会审核此量度，以确定在给定时间点当前在成本或成本过高下跟踪的任务或项目。 成本可以以小时或美元计量，具体取决于您的性能指数方法(PIM)。 有关设置性能索引方法的详细信息，请参阅 [设置性能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

只有需要时间录入的组织才能使用CPI。 此外，基于成本的PIM值仅在具有为任务分配者（职务角色或用户）定义成本费率的组织中是准确的。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对项目和财务数据的访问权限</p> <p> 如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限，并具有查看财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 成本绩效指数(CPI)概述

* [CPI值](#the-cpi-value)
* [如何计算CPI](#how-cpi-is-calculated)

### CPI值 {#the-cpi-value}

项目经理们明白，CPI值为1，意味着项目正处于预算状态。 大于1的值表示项目处于预算之下（记录的小时数或费用少于最初计划），小于1的值表示项目超出预算（记录的小时数或费用多于最初计划）。 距1越远，与计划的偏差越大。

| **CPI值** | **预算指示** |
|---|---|
| 1 | 关于计划或预算 |
| > 1（大于1） | 预算不足 |
| &lt; 1（小于1） | 超出预算 |


### 如何计算CPI {#how-cpi-is-calculated}

在Adobe Workfront,CPI的计算取决于为项目选择的绩效指数方法。 有关设置性能索引方法的详细信息，请参阅 [设置性能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [使用基于小时的PIM时的CPI计算](#cpi-calculations-when-using-hour-based-pim)
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

* **对于非父任务：**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **对于父任务：**
已执行的预算成本工作合计=所有直接子任务的预算成本工作合计字段的总和。

* **对于项目：**
执行的预算成本工作合计=所有顶层任务（父任务和独立任务）的“执行的预算成本工作合计”字段的总和。

有关已执行预算成本工作(BCWP)的信息，请参阅 [计算已执行的预算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

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

此计算中的字段如下所述：

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

已发生费用是实际成本> 0的费用

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* “执行的工作的计划成本”按以下公式计算：

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

已执行的预算成本工作总额计算如下：

* **对于非父任务：**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **对于父任务：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **对于项目：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## 在项目或任务中查找CPI

您可以在项目或任务列表或报表中显示项目或任务的CPI。 此外，您还可以在项目或任务级别查看。

1. 转到要查看CPI的项目或任务。
1. 展开 **项目详细信息** 或 **任务详细信息** 在左侧面板中，取决于您查看的是项目还是任务的CPI。

1. 单击 **金融**.

   CPI显示在 **CPI/SPI/CSI** 字段。

   ![](assets/cpi-on-project-nwe.png)
