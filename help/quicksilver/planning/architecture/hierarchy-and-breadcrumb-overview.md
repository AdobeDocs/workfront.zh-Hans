---
title: 层次结构和痕迹导航概述
description: 您可以在工作区中的记录类型之间创建多个工作区层次结构。
hide: true
hidefromtoc: true
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# 层次结构和痕迹导航概述

作为工作区管理员，您可以在Adobe Workfront Planning中的记录类型和其他对象类型之间定义灵活但结构化的层次结构。

层级是记录类型之间或记录类型与Workfront项目之间的连接。

有关创建层次结构的信息，请参阅[创建工作区层次结构](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)。

以下是在工作区中使用层次结构的好处：

* 组织工作，以反映您的团队实际计划、操作和交付的方式。
* 供用户通过参考一组痕迹导航来了解他们的位置、记录类型如何连接以及策略如何进入执行流程，这些痕迹导航指示他们在系统中的位置。
* 提供更好的导航，并在所有工作流中创建清晰度和连续性。
* 定义适合您组织工作方式的流，支持所有工作阶段的灵活性和一致性。

## 使用层级时的注意事项

* 您可以为一个工作区创建多个层次结构。
* 在一个层次结构中最多可以连接4个记录和对象类型。
* 在工作区层次结构中，只能连接以下对象类型：
   * 记录属于您正在构建层次的工作区的类型。
   * Workfront项目。
* 您不能在层次结构中添加以下对象类型：
   * 来自其他工作区的记录类型，即使它们设置为可连接或全局记录类型也是如此。
   * 所有其他Workfront对象。
   * AEM Assets
* 层次结构可以同时包括Planning记录类型和Workfront对象类型。

      例如，您可以将Campaign记录类型与Planning Tactics和Workfront Projects作为同一工作区层次结构中的子项。
  * 如果所选记录类型之间已经存在连接，则系统将重用现有连接。
* 如果不存在连接，Workfront将在层次结构设置中创建一个。
* 必须为连接的字段打开&#x200B;**在链接记录类型**&#x200B;上创建对应的字段。

  如果记录类型具有未在其链接的记录类型上创建相应字段的连接，则这些记录类型也可以属于层次结构，但在层次结构设置期间创建新连接时，您始终必须在链接的记录类型上创建相应字段。
* 以下是层次结构设置的规则：
   * 在给定工作区中，记录类型只能有一个父记录类型。

     例如，策略记录类型不能同时将“营销活动”和“目标”记录类型作为同一工作区中的父级。
   * 记录类型可以是多个层次结构中的父级。

     例如，一个工作区中可以有三个不同的层次结构，每个层次结构都可以将促销活动作为其父记录类型。
   * 当您将一个记录连接到多个或多个或多个记录类型时，可以将一个记录连接到多个相同类型的父记录。
例如，策略A可以同时属于促销活动X和促销活动Y。
   * 记录类型可以连接到多个子记录类型。

     例如，Campaign记录类型可以是多个其他记录类型（如战术、测试和其他记录类型）的父级。
   * 将全局记录类型添加到多个工作区后，它们可能会显示在多个层次结构内的多个工作区中。

     例如，如果促销活动是全局记录类型，并且是Workspace 1中层次结构的一部分，则它可作为现有记录类型添加到Workspace 2，并且可以是该处的层次结构的一部分。 但是，只有在Workspace 1中指定为全局记录类型，但未将其添加到Workspace 2时，它才能成为Workspace 2中层级的一部分。


## 查看痕迹导航时的注意事项

在记录类型之间创建层级时，这些记录类型会为属于这些记录类型的记录生成痕迹导航。

例如，如果您创建一个层次结构并将促销活动与战术、方案以及项目连接起来，当您导航到层次结构中连接的任何类型的记录时，可以查看该记录在该层次结构中的位置。

请考虑以下事项：

* 如果记录类型属于多个层次结构，则可以从记录页面上的记录痕迹导航在层次结构之间切换。
* 痕迹导航可以在Workfront和Planning中使用。

  例如，在查看与Planning营销活动和战术以及Workfront项目组合和项目群相关的项目时，您可以从痕迹导航在Planning和Workfront对象类型之间切换。

  有关详细信息，请参阅[创建工作区层次结构](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)。


