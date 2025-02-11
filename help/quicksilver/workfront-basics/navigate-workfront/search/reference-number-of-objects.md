---
content-type: reference
navigation-topic: search
title: 使用对象的参考编号
description: 在 [!DNL Adobe Workfront]中，项被标识为对象。 对象与数据库对应，并用于将数据与项关联。 参考号有助于区分两个在其他方面相似的对象（如同名的任务）。 您可以搜索参考号并将其包含在报表中。
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 使用对象的参考编号

在[!DNL Adobe Workfront]中，项被标识为对象。 对象与数据库对应，并用于将数据与项关联。

在创建对象时，Workfront会自动为以下每个对象分配唯一的参考编号：

* 项目
* 任务
* 问题
* 文档

参考号有助于区分两个在其他方面相似的对象（如同名的任务）。 您可以搜索参考号并将其包含在报表中。

>[!IMPORTANT]
>
>* [!DNL Workfront]在所有客户和所有对象中连续分配参考编号。 例如，在创建任务时，[!DNL Workfront]可能会为其分配一个参考编号00005。 如果其他客户接下来创建项目，则其项目可能会收到下一个可用的参考编号，例如00006。 如果您接下来创建问题，则您的问题可能会收到参考号00007，依此类推。
>* 您无法控制[!DNL Workfront]中任何对象的参考编号顺序。 顺序始终由我们的数据库控制。
>



## 查看对象的参考编号

默认情况下，将显示任务和问题的参考编号。 您还可以轻松地将[!DNL Workfront]配置为显示其他类型对象的参考编号。

* [查看任务和问题的参考编号](#view-reference-numbers-for-tasks-and-issues)
* [查看其他对象的参考编号](#view-reference-numbers-for-other-objects)
* [在报表中查看参考编号](#view-reference-numbers-in-reports)

### 查看任务和问题的参考编号

默认情况下，查看任务或问题时会显示参考编号。  要查看参考编号，请单击左侧面板中的&#x200B;**[!UICONTROL 任务详细信息]**&#x200B;或&#x200B;**[!UICONTROL 问题详细信息]**，然后在概述中找到&#x200B;**[!UICONTROL 基本信息]**&#x200B;部分。

![参考编号](assets/reference-number-nwe-350x184.png)

### 查看其他对象的参考编号

要查看对象的参考编号，您可以创建一个自定义视图，或修改现有视图，并将[!UICONTROL 参考编号]字段添加到视图中的列。 例如，您可以修改[!UICONTROL 项目]视图以显示所有项目的参考编号。

有关如何创建或修改视图的信息，请参阅 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)中的[视图概述。

### 在报表中查看参考编号

通过将[!UICONTROL 参考编号]列添加到报表中，可以显示报表中对象的参考编号。

有关如何向报表中添加列的信息，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 按参考号搜索对象

[!DNL Workfront]允许您按参考号搜索对象。

在&#x200B;**[!UICONTROL 搜索]**&#x200B;字段中键入对象的参考编号，然后按&#x200B;**[!UICONTROL Enter]**。

有关在Workfront中搜索的详细信息，请参阅[搜索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)。
