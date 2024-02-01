---
title: 记录类型和分类概述
description: 记录类型是Maestro工作区的构建块。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 记录类型和分类概述

{{maestro-important-intro}}

与Workfront中预定义对象类型不同，在Adobe管理器中，您可以创建自己的对象类型。 例如，在Workfront中，已创建Program、Portfolio、Project、Task或Issue的对象类型。

Maestro对象类型称为“记录类型”。 记录类型是Maestro工作区的构建块。 有关工作区的信息，请参见 [创建工作区](../architecture/create-workspaces.md).

## 记录类型概述

在Maestro中，您可以创建符合组织需求的自定义记录类型。

* 以下是Maestro记录类型：

   * [操作记录类型](#operational-record-type)：表示战略计划、计划或计划工作的记录类型。 例如， Campaign 、 Activity 、 Tactics 、 Opportunity可以是运营记录类型。
   * [分类](#taxonomy)：捕获有关操作记录类型的属性的记录类型。 例如，区域、地址、受众可以是分类。

* 在创建记录类型时，只有您和您授予工作区访问权限的用户才能查看记录类型。
* 必须先创建工作区，然后才能为工作区创建记录类型。
* 在一个工作区中总共可以有1,000种操作记录类型和分类。 这包括从头开始创建或从其他系统导入的记录类型或分类。

### 操作记录类型{#operational-record-type}

操作记录类型是一种表示工作相关对象的Maestro记录类型。

![](assets/operational-record-type-blank.png)

有关操作记录类型（包括如何创建操作记录类型）的详细信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

### 分类{#taxonomy}

分类法是一种记录类型，用于捕获有关操作记录类型的属性。

![](assets/taxonomy-record-type-blank.png)

有关分类记录类型的详细信息，请参阅 [创建分类](../architecture/create-a-taxonomy.md).

尽管创建分类与创建操作记录类型相同，但Maestro在概念上区分操作记录类型和分类记录类型。 分类法的目的是增强操作记录类型。 分类不应直接表示工作对象。  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

例如，“受众”、“区域”或“地址”可以是分类类型的记录类型。

有关更多信息，请参阅 [创建分类](../architecture/create-a-taxonomy.md).

## 运营记录类型和分类之间的异同

下表说明了运行记录类型和分类之间的一些异同：

| 记录类型和特征 | 操作记录类型 | 分类记录类型 |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| 它们是工作区的一部分 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以从工作区模板自动创建这些工作区 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以从头开始手动创建它们 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以通过复制和粘贴外部文件或列表中的信息来创建它们 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以通过导入Excel或CSV文件来创建 | ✓ {\f13 } |                     |
| 通过从其他应用程序连接到对象类型，可以创建只读记录类型 | ✓ {\f13 } |                     |
| 它们表示与工作相关的对象 | ✓ {\f13 } |                      |
| 它们表示与工作相关的对象的属性 |                         | ✓ {\f13 } |
| 您可以从头开始创建 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以通过导入Excel或CSV文件来创建 | ✓ {\f13 } |                      |
| 您可以将记录类型连接到第三方应用程序中的对象 | ✓ {\f13 } |                      |
| 您可以连接到其他主要记录类型 | ✓ {\f13 } |                    |
| 您可以在表视图中查看其关联的记录 | ✓ {\f13 } | ✓ {\f13 } |
| 您可以在时间线视图中查看其关联的记录 | ✓ {\f13 } | ✓ {\f13 } |
