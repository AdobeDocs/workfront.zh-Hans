---
content-type: release-notes
keywords: 注释，季度，更新
navigation-topic: product-releases
title: 21.1项目管理增强功能
description: 本页介绍了在“预览”环境中21.1版本所做的所有项目管理增强功能。 这些增强功能将于2021年2月15日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# 21.1项目管理增强功能

本页介绍了在“预览”环境中21.1版本所做的所有项目管理增强功能。 这些增强功能将于2021年2月15日这一周的生产环境中提供。

有关21.1版本中可用的所有更改的列表，请参阅 [21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 导出现在可在项目的“量度”部分中使用

为了更轻松地共享项目的状态和进度，您现在可以将项目“量度”部分的整个功能板导出为.png文件。

有关更多信息，请参阅 [项目量度概述](../../../manage-work/projects/manage-projects/project-metrics.md).

此功能现在包含在 [新Workfront体验的计划员基础知识，第3部分：管理项目](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) 学习Workfront一号。

## 更新从问题更新转换的项目或任务完成的问题百分比

我们更新了已转换为项目或任务的问题完成百分比的工作方式。 使用新功能，当问题转换为任务或项目时，当从设置中启用“解决对象更改状态时自动更新可解决的问题状态”设置时，问题完成百分比将与解决任务或项目完成百分比同步更新。

有关转换问题的信息，请参阅 [解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 新提交的请求列表

为了让您以更简单、更一致的方式管理已提交的请求，我们删除了“请求”区域中的“我已提交的请求”和“所有请求”部分，并将其替换为新的“已提交”列表。 该列表具有与系统中所有其他列表相匹配的熟悉外观，允许您筛选不同类别的已提交请求，并快速搜索可能难以找到的请求。

有关如何查找已提交请求的信息，请参阅 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。

此功能现在包含在 [新Workfront体验中的请求](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) 学习Workfront一号。

## 从“新请求”页面中删除的字段

>[!NOTE]
>
>已从版本中删除。

在重新设计“新请求”页面时，我们更新了在项目的“队列设置”部分中设置的“新问题字段”。

只有在从项目的“问题”部分创建问题时，才会显示以下新问题字段。 使用“请求”区域中的请求队列提交问题时，不会显示这些问题：

* 严重程度
* 计划小时
* 计划开始日期
* URL
* 分派给
* 工作角色
* 团队

我们已在“新请求”(New Request)页面上将“分配给”(Assigned To)、“作业角色”(Job Role)和“团队”(Team)字段替换为新的“分配”(Assignments)字段，以便在您提交新请求时，在公用字段中有效地指定用户、作业角色或团队。

有关为项目定义新问题字段的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 在“请求”区域提交请求时的新体验

>[!NOTE]
>
>从版本中删除；将保留在“预览”状态，并在21.2的“生产”版本中发行。

为了在提交请求时与Workfront的新体验保持一致并提高效率，我们重新设计了“请求”区域的“新请求”框。 以下是一些改进：

* 与其余的新Workfront体验组成的用户界面
* 消除了“新请求”区域，提供更轻松、更直观的体验
* 将文档附加到请求中的一种新的、更高效的方法

能够在您输入请求时共享指向请求队列、主题组或队列主题的链接。

有关提交请求的信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## 提交请求时共享指向请求队列的链接

>[!NOTE]
>
>从版本中删除；将保留在“预览”状态，并在21.2的“生产”版本中发行。

现在，在创建请求时，我们允许共享指向请求队列、主题组或队列主题的链接。

在提交新请求之前，您可以复制指向请求的请求队列、主题组或队列主题的链接，并将其与其他用户共享，或将其嵌入功能板。

有关在提交请求时共享指向请求队列的链接的信息，请参阅 [共享到请求队列的链接](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## 搜索要分配给项目的群组并查看其详细信息

现在，在为项目分配群组时，更容易确保确定正确的群组。 将鼠标悬停在“组”框中找到的组名称上，然后单击该名称旁边显示的信息图标，以查看“组详细信息”工具提示。

此工具提示包括群组上方的群组（如果有）和群组管理员的层次结构。

根据为群组配置的详细信息，您还可能会看到群组的业务负责人和说明。

利用此信息，您可以确保选择了要分配给项目的正确组。

有关更多信息，请参阅 [在项目概述区域中管理信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## 新建用户委派报表

以前，任务、问题和项目批准委托的信息只能由其“主页”区域的代表查看。 为了让其他用户能够看到此信息，计划用户现在可以创建用户委派报表，该报表会告诉您：

* 已将这些批准委派给其他用户的人员
* 已将这些批准委派给哪个用户
* 这些代表团的开始和结束日期

要了解更多信息，请参阅 [创建用户委派报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
