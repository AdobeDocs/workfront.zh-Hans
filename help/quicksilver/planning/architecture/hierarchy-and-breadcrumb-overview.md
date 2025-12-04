---
title: 层次结构和痕迹导航概述
description: 您可以在工作区中的记录类型之间创建多个工作区层次结构。
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

以下是在工作区中使用层次结构的好处：

* 组织工作，以反映您的团队实际计划、操作和交付的方式。
* 用户通过引用一组痕迹导航来了解他们的位置、记录类型如何连接以及策略如何进入执行，这些痕迹导航指示他们在系统中的位置。
* 提供更好的导航，并在所有工作流中创建清晰度和连续性。
* 层级不会强制实施系统定义的刚性结构，而是允许您定义适合组织工作方式的流，从而支持工作所有阶段的灵活性和一致性。

## 使用层级时的注意事项

* 作为工作区管理员，您可以为一个工作区创建多个层次结构。
* 如果所选记录类型之间已经存在连接，则系统将重用现有连接。
* 如果不存在连接，Workfront将在层次结构设置过程中自动创建一个连接。
* 以下是层次结构设置的规则：
   * 在给定工作区中，记录类型只能有一个父记录类型。

     例如，策略记录类型不能同时将“营销活动”和“目标”记录类型作为同一工作区中的父级。
   * 当您将一个记录连接到多个或多个或多个记录类型时，可以将一个记录连接到多个相同类型的父记录。
例如，策略A可以同时属于促销活动X和促销活动Y。
   * 记录类型可以连接到多个子记录类型。

     例如，Campaign记录类型可以是多个其他记录类型（如战术、测试和其他记录类型）的父级。
   * 层次结构可以包括Planning记录类型和Workfront对象类型。

     例如，您可以将Campaign记录类型与规划策略和Workfront项目作为子项。
   * 全局记录类型可能出现在多个层次结构内的多个工作区中。
   * Workfront对象类型还可以出现在多个层次结构和不同的工作区中。
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * 如果记录类型具有未在其链接的记录类型中创建相应字段的连接，则这些记录类型也可以是层次结构的一部分。 默认情况下，在层级设置期间创建的新连接将始终在链接的记录类型上创建对应的字段。

## 查看痕迹导航时的注意事项


