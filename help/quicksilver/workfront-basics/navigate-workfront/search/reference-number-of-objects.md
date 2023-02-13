---
content-type: reference
navigation-topic: search
title: 使用对象的引用数
description: 在 [!DNL Adobe Workfront]，则项目将被标识为对象。 对象与数据库相对应，用于将数据与项目关联。 在区分两个其他相似对象（例如具有相同名称的任务）时，引用编号非常有用。 您可以搜索引用编号并将其包含在报表中。
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 使用对象的引用数

在 [!DNL Adobe Workfront]，则项目将被标识为对象。 对象与数据库相对应，用于将数据与项目关联。

Workfront在创建对象时会自动为以下每个对象分配一个唯一的引用编号：

* 项目
* 任务
* 问题
* 文档

在区分两个其他相似对象（例如具有相同名称的任务）时，引用编号非常有用。 您可以搜索引用编号并将其包含在报表中。

>[!IMPORTANT]
>
>* [!DNL Workfront] 在所有客户和所有对象中连续分配引用编号。 例如，创建任务时， [!DNL Workfront] 可以为其分配参考号00005。 如果其他客户在下一步创建一个项目，则其项目可能会收到下一个可用的参考编号，例如00006。 如果您接下来创建问题，您的问题可能会收到参考号00007，等等。
>* 不能控制中任何对象的引用编号序列 [!DNL Workfront]. 序列始终由我们的数据库控制。
>




## 查看对象的引用编号

默认情况下，会为任务和问题显示参考编号。 您还可以轻松配置 [!DNL Workfront] 以显示其他类型对象的引用编号。

* [查看任务和问题的参考编号](#view-reference-numbers-for-tasks-and-issues)
* [查看其他对象的引用编号](#view-reference-numbers-for-other-objects)
* [在报表中查看参考编号](#view-reference-numbers-in-reports)

### 查看任务和问题的参考编号

默认情况下，在查看任务或问题时，会显示参考编号。  要查看参考编号，请单击 **[!UICONTROL 任务详细信息]** 或 **[!UICONTROL 问题详细信息]** 在左侧面板中，找到 **[!UICONTROL 基本信息]** 部分。

![](assets/reference-number-nwe-350x184.png)

### 查看其他对象的引用编号

要查看对象的引用编号，您可以创建自定义视图或修改现有视图并添加 [!UICONTROL 参考编号] 字段。 例如，您可以修改 [!UICONTROL 项目] 查看以显示所有项目的参考编号。

有关如何创建或修改视图的信息，请参阅 [视图概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 在报表中查看参考编号

您可以通过添加 [!UICONTROL 参考编号] 列。

有关如何向报表添加列的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 按引用编号搜索对象

[!DNL Workfront] 允许您按引用编号搜索对象。

在 **[!UICONTROL 搜索]** 字段，然后按 **[!UICONTROL 输入]**.

有关在Workfront中搜索的更多信息，请参阅 [搜索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
