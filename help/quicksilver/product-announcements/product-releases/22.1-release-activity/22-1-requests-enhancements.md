---
title: 22.1请求增强功能
description: 22.1请求增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1请求增强功能

本页介绍了22.1版本对“预览”环境所做的所有请求增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日这一周。

有关22.1版本的所有可用更改列表，请参阅[22.1版本概述](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)。

## 改进了没有权限创建请求的用户的界面

为了改善用户处理请求时的体验，我们对界面进行了改进，向登录用户指示他们无权创建请求。 经过这项改进后，对于无权创建问题的用户，“新建请求”按钮将变灰。 将鼠标悬停在灰显按钮上会显示工具提示，其中说明Workfront管理员已限制当前用户创建请求的访问权限。

在此增强功能之前，新请求按钮不显示在这些用户的请求区域中。 此外，复制请求并将其提交为新请求也受到限制。

有关创建请求的更多信息，请参阅[创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

## 复制并提交请求

为了优化提交请求的流程，我们将引入新功能，通过该功能，您可以复制现有请求并将其作为新请求提交。 当您频繁提交类似请求时，这非常有用。 在这种情况下，您可以重用现有请求，进行一些更改，然后将其作为新请求提交。

进行此更改后，可以查看其他用户提交的请求的用户也可以复制这些请求，并将其作为新请求提交。 您可以通过更新请求队列项目中的以下设置来防止发生这种情况：来自同一公司的人员将继承所有请求的相同权限。

>[!NOTE]
>
>在发布此功能之前，您无法复制和重新提交提交提交到没有队列主题的请求队列的问题。

有关详细信息，请参阅[复制并提交请求](../../../manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 更新了请求区域已提交部分中的摘要面板体验

>[!NOTE]
>
>2021年11月12日，此功能暂时从预览环境中移除。 稍后将重新添加它。

为了改进可见性和与“摘要”面板的交互，我们在请求区域的已提交部分的打开摘要图标中添加了一个标签。 标签现在为动态标签，它会根据面板是打开还是关闭而更新。

现在，当打开“摘要”面板而未首先选择请求时，会显示一个更加用户友好的图像，以明确指示用户在打开面板之前选择项目。 有关详细信息，请参阅[查找已提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md)。

此外，根据这项变化，更新了任务、问题和文档的摘要面板。 有关摘要面板的信息，请参阅[摘要概述](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)。
