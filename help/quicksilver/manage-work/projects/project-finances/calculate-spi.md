---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划绩效指数(SPI)
description: 计划绩效指数(SPI)描述了计划计划与实际计划之间的关系。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
TQID: https://experienceleague.adobe.com/WfZDTGfYIcngo8a3MQAh-Z7jnKm4nnBppV8hYSweygo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 398
ht-degree: 4%

---

# 计算计划绩效指数(SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

计划绩效指数(SPI)描述了计划计划与实际计划之间的关系。 Adobe Workfront在项目和任务级别计算SPI。 项目经理审查此量度，以确定任务或项目当前正在跟踪的时间是提前还是晚于。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>浅色或更高</p>
   <p>审核或更高</p></td>  
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>查看对项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>具有查看一般财务的权限的项目查看或更高权限</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 计划绩效指数(SPI)概览

* [SPI值显示的内容](#what-the-spi-value-shows)
* [Workfront如何计算SPI](#how-workfront-calculates-spi)

### SPI值显示的内容 {#what-the-spi-value-shows}

项目经理了解，SPI值为1表示项目按计划或按计划进行。  值大于1表示项目提前于计划，值小于1表示项目落后于计划。  与1越远，与计划的偏差越大。

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

“至今的计划小时数”计划是在您执行计算的分钟计算的。 它显示到当前日期的计划小时数。 当您将财务数据更改为准确时，会自动重新计算此值。 Workfront中没有指示此值的字段。

例如，如果您有一个具有1个任务的项目，并且该任务具有10个计划小时数和10天持续时间，则第5天的计划小时数计划至今为5。

## 在项目或任务中找到SPI

1. 转到要查看其SPI的项目或任务。
1. 根据您是要查看项目还是任务的SPI，执行以下操作之一：

   1. 单击左侧面板中的&#x200B;**项目详细信息**，然后查看&#x200B;**财务**&#x200B;区域。

   1. 单击左侧面板中的&#x200B;**任务详细信息**，然后查看&#x200B;**财务**&#x200B;区域。

      项目](assets/spi-on-project-nwe.png)上的![SPI

1. 查找&#x200B;**CPI/ SPI/ CSI**&#x200B;字段。
