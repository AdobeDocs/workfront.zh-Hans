---
content-type: release-notes
keywords: 注释，每季，更新
navigation-topic: product-releases
title: 21.1项目管理方面的改进
description: 本页介绍了21.1版本对“预览”环境所做的所有项目管理增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 21.1项目管理方面的改进

本页介绍了21.1版本对“预览”环境所做的所有项目管理增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。

有关21.1版本的所有可用更改列表，请参阅[21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 项目的量度部分现在提供了导出功能

为了更轻松地共享项目的状态和进度，您现在可以将项目的“量度”部分中的整个功能板导出到.png文件。

有关详细信息，请参阅[项目量度概述](../../../manage-work/projects/manage-projects/project-metrics.md)。

此功能现已包含在新Workfront Experience的[规划者基础知识部分，第3部分：在Workfront One上管理项目](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径。

## 当项目或任务从问题更新中转化时，更新问题完成百分比

我们更新了问题完成百分比处理已转换为项目或任务的问题的方法。 借助新功能，当问题转换为任务或项目时，当从设置启用“当解析对象状态更改时自动更新可解析问题状态”设置时，问题的完成百分比与解析任务或项目的完成百分比同步。

有关转换问题的信息，请参阅[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

## 新提交的请求列表

为了让您以更简单、更一致的方式管理您提交的请求，我们删除了我已提交的请求和请求区域中的所有请求部分，并将其替换为新的已提交列表。 该列表具有熟悉的外观，与系统中的所有其他列表匹配，允许您筛选不同类别的已提交请求，并快速搜索可能难以找到的请求。

有关如何查找已提交请求的信息，请参阅[查找已提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md)。

此功能现已包含在Workfront One上的新Workfront Experience[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)学习路径的Collaborator基础知识中。

此功能现已包含在Workfront One上的新Workfront Experience[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/understand-request-queues)学习路径的请求中。

## 从新请求页面中移除的字段

>[!NOTE]
>
>已从版本中删除。

作为重新设计新请求页面的一部分，我们更新了在项目的队列设置部分中设置的新问题字段。

以下新问题字段仅在从项目的问题部分创建问题时显示。 使用请求区域中的请求队列提交问题时，不显示请求队列：

* 严重性
* 规划小时数
* 计划开始日期
* URL
* 任务负责人
* 工作角色
* 团队

我们已在“新建请求”页面上的“分配给”、“工作角色”和“团队”字段中替换为“分配”字段，以便在您提交新请求时有效地在公共字段中指定用户、工作角色或团队。

有关为项目定义新问题字段的信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 在请求区域提交请求时的新体验

>[!NOTE]
>
>已从版本中删除；将保留在“预览”中，并从21.2发布到“生产”环境。

为了与新的Workfront体验保持一致，并提升提交请求时的效率，我们重新设计了请求区域的新请求框。 以下是一些改进：

* 提供了包含全新Workfront体验其余部分的组合用户界面
* 消除了“新请求”区域，体验更加简单直观
* 一种更高效的新方式可将文档附加到您的请求

输入请求时共享指向请求队列、主题组或队列主题的链接的功能。

有关提交请求的信息，请参阅[创建并提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

## 提交请求时共享指向请求队列的链接

>[!NOTE]
>
>已从版本中删除；将保留在“预览”中，并从21.2发布到“生产”环境。

现在，在创建请求时，我们可以共享指向请求队列、主题组或队列主题的链接。

在提交新请求之前，您可以复制指向请求的请求队列、主题组或队列主题的链接，并将其与其他用户共享，或将其嵌入功能板中。

有关提交请求时共享请求队列链接的信息，请参阅[共享请求队列链接](../../../manage-work/requests/create-requests/share-link-to-request-queue.md)。

## 搜索要分配给项目的组并查看其详细信息

现在，在将组分配给项目时，可以更轻松地确保标识正确的组。 将鼠标悬停在“组”框中找到的组名称上，然后单击该名称旁边显示的信息图标以查看组详细信息工具提示。

此工具提示包括组上方的组层次结构（如果有）以及组的管理员。

根据为组配置的详细信息，您还可能会看到组的业务负责人和描述。

有了这些信息，您就可以放心地选择要分配给项目的正确组。

有关详细信息，请参阅[在项目概述区域](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)中管理信息。

## 新建用户委派报告

以前，任务、问题和项目批准委托的信息只能由委托人在其“主页”区域查看。 为了允许其他用户查看此信息，计划用户现在可以创建用户委派报告，该报告将告诉您：

* 谁已将这些审批委派给其他用户
* 哪个用户已被委托这些审批
* 这些委托的开始日期和结束日期

若要了解详细信息，请参阅[创建用户委派报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md)。
