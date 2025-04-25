---
title: 记录类型概述
description: 记录类型是Adobe Workfront Planning工作区的构建块。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---


# 记录类型概述

{{planning-important-intro}}

与Workfront中预定义的对象类型不同，在Adobe Workfront Planning中，您可以创建自己的对象类型。 例如，在Workfront中，已创建Program、Portfolio、Project、Task或Issue的对象类型。

Workfront Planning对象类型称为“记录类型”，它们仅在用户创建时存在。 记录类型是Workfront Planning工作区的构建块。 有关工作区的信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

## 记录类型概述

在Workfront Planning中，您可以创建符合组织需求的自定义记录类型。

有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

* 从模板创建工作区时，会在以下工作区部分中创建记录类型：

   * **操作记录类型**：表示战略计划、计划或计划工作的记录类型。 例如， Campaign 、 Activity 、 Tactics 、 Opportunity都是操作记录类型。
   * **分类**：捕获有关操作记录类型的属性的记录类型。 例如，区域、地址、受众是分类。

* 在自头创建的工作区中创建记录类型时，可以将记录类型放置到工作区中创建的任何部分中。
* 在创建记录类型时，只有您和您授予工作区访问权限的用户才能查看记录类型。
* 必须先创建工作区，然后才能为工作区创建记录类型。
* 有关在一个工作区或Workfront实例中可以有多少记录类型的限制，请参阅[Adobe Workfront Planning对象限制概述](/help/quicksilver/planning/general/limitations-overview.md)。


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
