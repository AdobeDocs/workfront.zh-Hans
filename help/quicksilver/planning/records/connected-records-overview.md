---
title: 连接的记录概述
description: 在记录类型之间创建连接后，可以将各个记录彼此连接。 本文介绍了在Adobe Workfront Planning中连接记录时必须考虑的注意事项。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# 连接的记录概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

您可以将Adobe Workfront Planning记录相互连接或与其他应用程序中的对象连接。

本文介绍了在Workfront Planning中连接记录时必须考虑的注意事项。

有关如何将记录相互连接或连接到另一个对象的信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

## 先决条件

在Workfront Planning中连接记录之前，必须连接以下各项：

* 两种记录类型
* 带有来自另一个应用程序的对象的记录类型

有关详细信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。


## 有关连接记录的注意事项

* 连接记录类型后，连接的记录类型在它们链接到的记录类型表中以及记录页面上显示为连接字段。
* 您可以从链接的记录字段中浏览和添加链接记录的记录和对象以及对象类型。
* 您可以在要链接的记录类型的表中添加链接记录类型的字段（查找字段）。

  此外，您还可以在要链接的记录类型的表格中添加要链接的记录类型的字段（查找字段）。

  例如，如果从“促销活动”记录类型链接产品记录类型，则可以显示促销活动的产品字段以及产品的促销活动字段。
* 您无法手动更新链接来源记录中的查找字段值。

  在原始记录或对象上更新查找字段的值后，会自动填充您要链接的Workfront Planning记录。

* 有权访问Workfront Planning和“查看”或者对工作区有更高权限且具有记录类型的每个人都可以查看您在记录之间或记录与其他应用程序的对象之间建立的连接。 他们可以查看连接的记录和对象，无论他们在您连接的应用程序中的权限如何。
* 如果您对工作区和所连接记录的记录类型具有管理权限，则可以查看和编辑其他人的连接。
* 您可以将一个记录连接到另一个应用程序的一个或多个对象。具体取决于您在连接记录类型时选择的连接类型。 有关详细信息，请参阅文章[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)中的“连接类型”部分。
* 当连接的记录类型是层次结构的一部分时，您可以从记录的页面访问层次结构中的任何对象类型。 有关信息，请参阅[层次结构和痕迹导航概述](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。
* 如果连接的记录类型是层次结构的一部分，则可从子记录类型将一个记录连接到父记录类型的多达10个记录。 有关信息，请参阅[层次结构和痕迹导航概述](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 可连接记录的区域

您可以在Workfront中手动或自动连接记录。

### 手动连接记录

您可以在以下区域中手动将记录连接到其他记录或从其他应用程序连接到对象：

* 您可以将Workfront Planning中的记录连接到Planning记录的以下区域中的Workfront对象、Experience Manager Assets对象或GenStudio Brands：

   * Planning中记录类型的表视图中的已连接记录字段。
   * 记录的预览或详细信息页面中的已连接记录字段。
   * 记录的“连接的记录”页面上的记录的预览或详细信息页面。

* 您可以在Workfront的以下区域中将Workfront对象连接到Workfront Planning记录：

   * Workfront对象的“规划”部分。
   * Workfront对象的自定义表单上的Planning连接字段。

  有关信息，请参阅[管理来自Workfront对象的记录连接](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。

### 自动连接记录

在将记录类型相互连接或将记录类型从另一个应用程序连接到对象类型后，可以通过以下方式自动连接记录和对象：

* 使用自动化

  您可以从配置自动化的Planning记录中创建记录或Workfront对象。

  当满足您定义的条件时，将创建记录或对象，并且自动连接到从中触发自动操作的记录。

  有关信息，请参阅[配置Adobe Workfront计划自动化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

* 使用请求表单创建记录

  您可以在提交Planning请求时创建记录。 请求和记录会自动连接。

  >[!NOTE]
  >
  >无法断开记录与其原始请求的连接。

  有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。
