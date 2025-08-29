---
content-type: release-notes
title: Adobe Workfront Planning 2025年第四季度发布活动
description: 这是Adobe Workfront Planning产品2025年第四季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: c7c958b09caf7e15f128a729f6b327f6c3fa21e8
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 0%

---

# Adobe Workfront Planning 2025年第四季度发布活动

本文介绍了在2025年第四季度版本中为Workfront计划发布的功能。

<!--keep the sentence below for all future quarterly release pages-->

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。



## 统一请求列表中新的组合状态列

>[!NOTE]
>
>* 预览： 2025年8月28日
>* 生产快速发布： 2025年9月11日
>* 适用于所有客户的生产： 2025年10月16日

为简化统一请求体验，状态列现在会同时显示请求状态和审批状态，两者均适用于给定请求。

有关创建请求的更多信息，请参阅：

* 对于Workfront： [创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* 对于Workfront Planning： [提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)

## 公式字段的新限制

>[!NOTE]
>
>* 预览： 2025年8月28日
>* 生产快速发布： 2025年9月11日
>* 适用于所有客户的生产： 2025年10月16日

我们对公式字段进行了以下限制：

* 每个记录类型最多有20个公式字段
* 公式表达式限制为50,000个字符

有关详细信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

## 无法解析公式值时显示错误

>[!NOTE]
>
>* 预览： 2025年8月28日
>* 生产快速发布： 2025年9月11日
>* 适用于所有客户的生产： 2025年10月16日

为了指示解析公式字段时出现问题，该字段现在将显示为“#ERROR！” 在以下任一情况中：

* 删除公式中使用的字段时。

* 当在聚合查找字段中使用的字段显示为#ERROR！

* 当公式值无法以所选格式显示时。

有关信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

## 新表达式已添加到Planning中的公式字段

>[!NOTE]
>
>预览： 2025年8月7日
>&#x200B;>所有客户的生产:August， 2025
>&#x200B;>[!BADGE 超出计划]{type=Neutral}

我们向Workfront Planning中的公式字段和Workfront中的计算自定义字段添加了具有以下用法的新表达式：

* **REMOVEACCENTS(string)**：从输入字符串中所有重音字符中删除变音标记。
* **REPLACEPATTERN （字符串、模式、替换字符串）**：将给定模式的匹配项替换为替换字符串。
* **PASCAL(string)**：将输入字符串转换为PascalCase，方法是将每个单词的第一个字母转换为大写，并删除所有空格。

有关详细信息，请参阅[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

## 向公式字段创建窗口添加最大化按钮和最小化按钮

>[!NOTE]
>
>预览： 2025年7月31日
>&#x200B;>适用于所有客户的生产： 2025年7月31日
>&#x200B;>[!BADGE 超出计划]{type=Neutral}

我们在记录表视图中创建或编辑公式字段时，添加了“最大化”按钮以放大该字段。 此外，我们在新的放大窗口中添加了“最小化”按钮，以还原到字段创建框。

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 现在，记录的预览区域中提供“连接的记录”页面

>[!NOTE]
>
>* 预览： 2025年7月31日
>* 生产快速发布： 2025年8月14日
>* 适用于所有客户的生产： 2025年10月16日

现在，我们已在预览框中使“连接的记录”页面的体验与记录“详细信息”区域完整页面中的体验相匹配。

在此增强功能之前，只能在记录的“详细信息”区域的整页查看已连接记录页面中的已连接记录。

有关信息，请参阅[管理记录页布局](/help/quicksilver/planning/records/manage-the-record-page.md)。

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## 在时间轴视图中创建记录

>[!NOTE]
>
>预览： 2025年7月24日
>&#x200B;>生产快速发布： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日

现在，您可以在时间轴上的任意位置双击来在记录类型的时间轴视图中创建记录。

您可以选择记录的日期范围，或打开记录的页面以编辑其所有详细信息。

在此增强功能之前，您只能使用表格视图中的“新建记录”按钮或内联按钮添加新记录。

有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

## 在记录类型卡片的更多菜单中添加共享选项

>[!NOTE]
>
>预览： 2025年7月24日
>&#x200B;>生产快速发布： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日

您现在可以从工作区页面上记录类型卡片的更多菜单共享记录类型。 在此增强功能之前，购股权仅在记录类型页面内可用。

有关信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。

## 以全屏模式显示所有Workfront Planning视图

>[!NOTE]
>
>预览： 2025年7月24日
>&#x200B;>生产快速发布： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日

您现在可以在全屏模式下显示所有Workfront Planning视图（表、时间轴和日历）。 视图功能将保留，您也可以在全屏模式下更改视图。

在此增强功能之前，此功能不存在。

有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

## 在Planning请求表单中将团队添加为批准者

>[!NOTE]
>
>预览： 2025年7月22日
>&#x200B;>快速发布生产： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日

为了使审批流程更灵活，我们增加了在Planning请求表单上添加团队作为审批者的功能。 现在，您可以在设置批准者时输入和选择团队名称。 任何团队成员都可以做出决定，这被视为整个团队的批准决定。

以前，只能将个人用户指定为批准者。

有关详细信息，请参阅[在Adobe Workfront Planning中为申请表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

## 用于显示记录审批信息的新字段

>[!NOTE]
>
>预览： 2025年7月17日
>&#x200B;>快速发布生产： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日

我们引进了以下字段，用于捕获通过提交经批准的请求而创建的记录的批准信息：

* 批准者
* 审批日期

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 根据应用的分组自动填充字段

>[!NOTE]
>
>预览： 2025年7月10日
>&#x200B;>生产快速发布： 2025年8月14日
>&#x200B;>适用于所有客户的生产： 2025年10月16日


现在，当您将分组应用于表视图时，向表中添加记录将自动填充与您将记录添加到的分组相关联的字段。

如果应用了多个分组，则仅当在最后一个分组标准内的列表末尾添加记录时，系统才会自动填充与所有分组关联的字段。

在此增强功能之前，您必须手动更新与分组关联的字段。

有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
