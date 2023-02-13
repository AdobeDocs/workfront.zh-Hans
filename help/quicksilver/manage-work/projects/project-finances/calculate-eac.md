---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 完成时计算估计(EAC)
description: 作为绩效量度，完成时估计(EAC)表示项目或任务完成时的预计总成本。
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 完成时计算估计(EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

作为绩效量度，完成时估计(EAC)表示项目或任务完成时的预计总成本。

作为设置，它允许您定义应如何计算EAC值。 

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
   <td> <p>查看对项目和财务数据的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限，并具有查看财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 定义如何计算EAC

作为项目系统首选项的一部分，Adobe Workfront管理员可以定义如何计算EAC。 EAC可通过以下两种方式之一进行计算：

* [在项目级别计算](#calculate-at-the-project-level)
* [从任务和子任务汇总](#roll-up-from-tasks-and-subtasks)

有关在Workfront中设置项目首选项（包括如何在完成时计算估计）的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

作为项目经理，您还可以在项目级别的项目的“财务”子选项卡中更改此首选项。 有关编辑项目的“财务”子选项卡的更多信息，请参阅 [在项目财务区管理信息](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### 在项目级别计算 {#calculate-at-the-project-level}

父任务和项目的EAC通过在EAC公式中输入实际工时/实际人工成本来确定。 此计算包括直接添加到父任务或项目的实际小时数/成本和费用。

### 从任务和子任务汇总 {#roll-up-from-tasks-and-subtasks}

父任务和项目的EAC通过汇总每个子任务的EAC来确定。 此计算不包括直接添加到父任务或项目的实际小时数/成本和费用。

## 如何根据性能指数方法(PIM)计算EAC

在Workfront中，EAC的计算取决于项目的所选性能索引方法(PIM)。 有关为系统或项目设置PIM的更多信息，请参阅 [设置性能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [使用基于小时的PIM计算EAC](#calculate-eac-using-hour-based-pim)
* [使用基于成本的PIM计算EAC](#calculate-eac-using-cost-based-pim)

### 使用基于小时的PIM计算EAC {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;如果成本绩效指数 [计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0,EAC =总计划小时数+实际小时数。 捕获了小时，但项目/任务完成率为0%时，会发生这种情况。

有关计算CPI的详细信息，请参见 [计算成本绩效指数(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### 使用基于成本的PIM计算EAC {#calculate-eac-using-cost-based-pim}

项目的EAC使用以下公式计算：

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC人工=  <em>如果</em> CPI人工&lt;&gt; 0 - EAC人工=计划人工成本/CPI人工</pre><pre><em>ELSE</em> EAC人工=计划人工成本+实际人工成本</pre><pre>CPI人工=如果实际人工成本&lt;&gt; 0，则CPI人工= TotalBudgedCostWorkPerformed /实际人工成本</pre><pre>ELSE CPI劳动力= 1 </pre>在计算EAC时，会考虑以下字段：

* 已执行的预算成本总额(BCWP)=已计划工作的预算成本（预算成本）与迄今已完成任务的百分比之和的乘积。

   有关已执行预算成本工作(BCWP)的信息，请参阅 [计算已执行的预算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **对于非父任务：**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **对于父任务：**
已执行的预算成本工作合计=所有直接子任务的预算成本工作合计字段的总和。

   * **对于项目：**
执行的预算成本工作合计=所有顶层任务（父任务和独立任务）的“执行的预算成本工作合计”字段的总和。 

* EAC费用=将已发生实际费用成本加到未发生计划费用成本中的结果。 它由以下公式计算：

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * 已发生实际费用成本=“实际金额”字段> 0的所有费用的“计划金额”字段的总和。 例如，如果您为任务1创建费用，并在“计划金额”字段中输入$500.00，并在“实际金额”字段中输入金额> 0(例如，$600.00)，此任务的已发生计划费用成本为$500.00。
   * 未发生的计划费用=“实际金额”字段= 0的所有费用的“计划金额”字段的总和。 例如，如果为任务1创建两个费用，其中“计划金额”字段中的第一个费用值为$500.00，“实际金额”字段中的值为$600.00，对于第二个费用，则“计划金额”字段中的值为$300.00，“实际金额”字段的值为$0.00，则此任务的“未发生计划费用”值为$300.00。 

## 在项目或任务中找到EAC

1. 转到要查看EAC的项目或任务。
1. 展开 **项目详细信息** 或 **任务详细信息** 在项目或任务的左侧面板中，具体取决于您查看EAC的位置。

1. 单击 **金融**. 

   EAC值显示在 **完成时的估计** 字段。

   ![](assets/eac-highlighted-on-project-350x112.png)
