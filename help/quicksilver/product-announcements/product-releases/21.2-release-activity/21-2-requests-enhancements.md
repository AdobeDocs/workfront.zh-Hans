---
content-type: release-notes
keywords: 注释，季度，更新，发行
navigation-topic: 2021-2-release-activity
title: 21.2请求增强功能
description: 本页介绍了在“预览”环境中对21.2版本所做的所有请求增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
exl-id: af9c801f-ae40-439a-8749-ae8d178040ae
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# 21.2请求增强功能

本页介绍了在“预览”环境中对21.2版本所做的所有请求增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅 [21.2版本概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 控制您在新请求中执行的分配类型

>[!NOTE]
>
>仅在新的Adobe Workfront体验中可用。

我们更改了在创建新请求时“工作总揽”字段的工作方式，以提供一致性，并且无论用户可以输入什么类型的工作总是显示相同的字段。

在设置请求队列时，如果启用“分配给”、“作业角色”或“团队”字段可见，则请求者将看到相同的“分配”字段，该字段可容纳这三种分配类型中的所有或任何一种。

“工作总揽”(Assignments)字段中有一个指示，说明允许使用哪些类型的工作总揽。 例如，在设置请求队列时启用“分配给”和“团队”字段时，系统会提示您输入“搜索人员或团队”，而不是“搜索人员、角色或团队”。

有关更多信息，请参阅以下文章：

* [创建和提交Adobe Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 改进了创建请求和管理草稿

>[!NOTE]
>
>仅在新的Adobe Workfront体验中可用。

随着我们继续在新的Workfront体验中纳入您有关创建请求的反馈，我们对新请求工作流进行了一些改进。 这些功能包括：

* 使用“显示选项”图标清楚地指示“请求类型”、“主题组”和“队列主题”字段是下拉列表，您可以从中选择之前定义的选项。
* 使用“x”图标明确指示在选择请求类型、主题组或队列主题后可以删除该选项。
* 创建新请求时提供“关闭”按钮，以便不丢失草稿即可离开请求。 除此更改外，“放弃”按钮已重命名为“放弃草稿”。

有关创建新请求的信息，请参阅 [创建和提交Adobe Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。

## 改进了请求工作流

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

在我们继续听取您的反馈并整合您的反馈时，我们在新请求工作流程中添加了一些改进，以便您更轻松、更直观地与Adobe Workfront进行交互。 这些改进包括：

* 在定义“队列设置”时，可以在创建请求队列时选择要放置文件上载文档部分的位置。 您可以将此部分放在请求表单的自定义字段之前或之后。 有关更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 现在，当您离开页面时，将保留按其中一列对已提交请求列表进行排序的情况。 有关更多信息，请参阅 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
* 创建新请求时，“提交”和“取消”按钮现在位于“新建请求”表单的底部。 有关更多信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。

## 在“请求”区域的“已提交”部分中打开“摘要”面板

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了使您在Adobe Workfront的所有区域中的体验保持一致，我们已在“请求”区域的“已提交”部分中添加了“打开摘要”图标。 现在，您可以打开已提交问题的“摘要”面板，并查看有关问题的更多信息、分配这些问题，或添加文档或评论。

有关已提交请求的信息，请参阅 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。

## 在新请求表单中返回已删除的新问题字段

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

重新设计了随上一版本一起启动的新请求表单后，我们在提交新请求时阻止了项目队列详细信息部分的“新问题字段”区域中的几个字段显示。 在收集了您的反馈后，我们决定重新显示这些字段，以便它们全部显示在“新请求”窗体中。

有关信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 在“请求”区域提交请求时的新体验

>[!NOTE]
>
>已在21.1版本的“预览”功能中添加，但将包含在21.2版本的“生产”功能中。

为了在提交请求时与Workfront的新体验保持一致并提高效率，我们重新设计了“请求”区域的“新请求”框。 以下是一些改进：

* 与其余的新Workfront体验组成的用户界面
* 消除了“新请求”区域，提供更轻松、更直观的体验
* 将文档附加到请求中的一种新的、更高效的方法

能够在您输入请求时共享指向请求队列、主题组或队列主题的链接。

有关提交请求的信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。

## 提交请求时共享指向请求队列的链接

>[!NOTE]
>
>已在21.1版本的“预览”功能中添加，但将包含在21.2版本的“生产”功能中。

现在，在创建请求时，我们允许共享指向请求队列、主题组或队列主题的链接。

在提交新请求之前，您可以复制指向请求的请求队列、主题组或队列主题的链接，并将其与其他用户共享，或将其嵌入功能板。

有关在提交请求时共享指向请求队列的链接的信息，请参阅 [共享到请求队列的链接](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

此功能现在包含在 [新Workfront体验的Collaborator基础知识](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) 学习Workfront一号。
