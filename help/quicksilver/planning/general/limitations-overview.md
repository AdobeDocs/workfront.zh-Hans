---
title: Adobe Workfront Planning对象限制概述
description: Adobe Workfront Planning对实例中可创建的对象数量存在限制。 设置对象限制以提高产品性能并增强您对Workfront规划的体验。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1e62d5c7eff86432b4914793d75cdf4f835f3d5d
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 1%

---


<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning对象限制概述

{{planning-important-intro}}


Adobe Workfront Planning对实例中可创建的对象数量存在限制。 设置对象限制以提高产品性能并增强您对Workfront规划的体验。

下表显示了可在Workfront Planning中创建的对象数限制。 当我们进入开发的下一个阶段时，这些限制可能会发生变化。

| Adobe Workfront Planning对象 | 限制 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 一个Workfront实例的工作区数 | 无限制* |
| 一个工作区的部分数 | 50 |
| 一个工作区的记录类型数 | 1,000（这包括来自所有部分的记录类型以及在使用工作区模板时创建的记录类型） |
| 一种记录类型的记录数 | 25,000 |
| 一个工作区的记录数 | 25,000（计划为<br>的客户）500,000（计划为Planning Plus的客户） |
| Workfront Planning的一个实例的总记录数 | 500,000，适用于计划为<br>200,000的客户且适用于计划为Planning Plus的客户 |
| 一种记录类型或分类的字段数 | 500 |
| 单行文本字段的字符数 | 1,000个字符 |
| 段落字段的字符数 | 100,000个字符 |
| 一种记录类型的段落字段数 | 20个段落字段 |
| 可粘贴到记录类型表中的文件大小 | 1MB |
| 可通过API为记录类型表导入的文件的大小 | 1.5兆字节 |
| 发出API请求的速率 | 每分钟200个请求 |
| 一个用户可以为一个记录类型创建的视图数 | 100 |

*我们建议不要拥有太多工作区，因为它们可能会变得难以管理，并且您的工作流可能过于分散。

有关Workfront Planning定价和包装的信息，请参阅[Adobe Workfront定价和包装](https://business.adobe.com/products/workfront/pricing.html)。

<!--
****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

