---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划绩效指数(SPI)
description: 计划绩效指数(SPI)描述了计划计划与实际计划之间的关系。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 计算计划绩效指数(SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

计划绩效指数(SPI)描述了计划计划与实际计划之间的关系。 Adobe Workfront在项目和任务级别计算SPI。 项目经理审查此量度，以确定任务或项目当前正在跟踪的时间是提前还是晚于。

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

## 计划绩效指数(SPI)概览

* [SPI值显示的内容](#what-the-spi-value-shows)
* [Workfront如何计算SPI](#how-workfront-calculates-spi)

### SPI值显示的内容 {#what-the-spi-value-shows}

项目经理了解，SPI值为1表示项目按计划或按计划进行。  值大于1表示项目提前于计划，值小于1表示项目落后于计划。  与1越远，与计划的偏差越大。

| **SPI值** | **指示“按计划”** |
|---|---|
| 1 | 按计划或按计划 |
| > 1（大于1） | 提前计划 |
| &lt; 1（小于1） | 晚于计划 |

{style="table-layout:auto"}

### Workfront如何计算SPI  {#how-workfront-calculates-spi}

Workfront通过以下公式计算SPI：

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;如果计划小时数截止日期= 0，则SPI = 1*。

“至今的计划小时数”计划是在您执行计算的分钟计算的。 它显示到当前日期的计划小时数。 当您将财务数据更改为准确时，会自动重新计算此值。 Workfront中没有指示此值的字段。

例如，如果您有一个具有1个任务的项目，并且该任务具有10个计划小时数和10天持续时间，则第5天的计划小时数计划至今为5。 

## 在项目或任务中找到SPI

1. 转到要查看其SPI的项目或任务。
1. 根据您是要查看项目还是任务的SPI，执行以下操作之一：

   1. 单击左侧面板中的&#x200B;**项目详细信息**，然后查看&#x200B;**财务**&#x200B;区域。

   1. 单击左侧面板中的&#x200B;**任务详细信息**，然后查看&#x200B;**财务**&#x200B;区域。

      项目![&#128279;](assets/spi-on-project-nwe.png)上的SPI

1. 查找&#x200B;**CPI/ SPI/ CSI**&#x200B;字段。
