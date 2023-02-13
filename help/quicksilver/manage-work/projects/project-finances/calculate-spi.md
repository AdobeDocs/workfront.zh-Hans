---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划性能索引(SPI)
description: 计划性能指数(SPI)描述计划计划与实际计划之间的关系。
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 计算计划性能索引(SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

计划性能指数(SPI)描述计划计划与实际计划之间的关系。 Adobe Workfront在项目和任务级别计算SPI。 项目经理会查看此量度，以确定任务或项目当前是提前还是延迟跟踪。

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
   <td> <p>查看对项目和财务数据的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限，并具有查看财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 计划性能索引(SPI)概述

* [SPI值显示的内容](#what-the-spi-value-shows)
* [Workfront如何计算SPI](#how-workfront-calculates-spi)

### SPI值显示的内容 {#what-the-spi-value-shows}

项目经理们明白，SPI值为1表示项目已按计划或按计划进行。  大于1的值表示项目提前到达计划进度，小于1的值表示项目落后于计划进度。  距1越远，与计划的偏差越大。

| **SPI值** | **指示“按时”** |
|---|---|
| 1 | 按计划或按计划 |
| > 1（大于1） | 提前 |
| &lt; 1（小于1） | 晚于计划 |

{style=&quot;table-layout:auto&quot;}

### Workfront如何计算SPI  {#how-workfront-calculates-spi}

Workfront通过以下公式计算SPI:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;如果计划时间计划至日期= 0，则SPI = 1*.

“计划时间计划至日期”是在您执行计算时的分钟计算。 它显示计划到当前日期的计划小时数。 当您将财务数据更改为准确时，系统会自动重新计算它。 Workfront中没有指示此值的字段。

例如，如果您的项目有1个任务，而任务有10个计划小时和10天持续时间，则第5天的“计划小时数计划至今”为5。 

## 在项目或任务中查找SPI

1. 转到要查看SPI的项目或任务。
1. 根据您是要查看项目还是任务上的SPI，执行下列操作之一：

   1. 单击 **项目详细信息** 在左侧面板中，查看 **金融** 的上界。

   1. 单击 **任务详细信息** 在左侧面板中，查看 **金融** 的上界。

      ![](assets/spi-on-project-nwe.png)

1. 查找 **CPI/SPI/CSI** 字段。
