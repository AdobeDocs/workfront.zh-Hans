---
title: Adobe Workfront Planning对象限制概述
description: Adobe Workfront Planning对实例中可创建的对象数量存在限制。 设置对象限制以提高产品性能并增强您对Workfront规划的体验。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Adobe Workfront Planning对象限制概述

Adobe Workfront Planning对实例中可创建的对象数量存在限制。 设置对象限制以提高产品性能并增强您对Workfront规划的体验。

下表显示了可在Workfront Planning中创建的对象数限制。 当我们进入开发的下一个阶段时，这些限制可能会发生变化。

| Adobe Workfront Planning对象 | 限制 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 一个Workfront实例的工作区数 | 1,000 |
| 一个工作区的部分数 | 50 |
| 一个工作区的记录类型数 | 1,000（这包括来自所有部分的记录类型以及在使用工作区模板时创建的记录类型） |
| 一种记录类型的记录数 | 50,000 |
| 一种记录类型或分类的字段数 | 500 |
| 文本字段的字符数 | 1,000个字符 |
| 可粘贴到记录类型表中的文件大小 | 1MB |
| 可通过API为记录类型表导入的文件的大小 | 1.5兆字节 |
| 发出API请求的速率 | 每分钟200个请求 |
| 可导入的Excel文件的CSV大小* | 5MB |
| 一个用户可以为一个记录类型创建的视图数 | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*此功能已被暂时禁用，并将在以后可用。

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->