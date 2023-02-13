---
title: 22.1请求增强功能
description: 22.1请求增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 22.1请求增强功能

本页介绍了在“预览”环境中对22.1版本所做的所有请求增强。 这些增强功能将在生产环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日这一周。

有关22.1版本中可用的所有更改的列表，请参阅 [22.1版本概述](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 改进了无权创建请求的用户的界面

为了改善用户在处理请求时的体验，我们对界面进行了改进，以指示登录用户无权创建请求。 通过这项改进，对于无权创建问题的用户，“新建请求”按钮将变暗。 将鼠标悬停在灰显按钮上会显示工具提示，说明Workfront管理员限制了当前用户创建请求的访问权限。

在进行此增强之前，“新建请求”按钮未显示在这些用户的“请求”区域中。 复制和提交新请求也受到限制。

有关创建请求的更多信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

## 复制和提交请求

为了优化您提交请求的流程，我们引入了新功能，允许您复制现有请求并将其作为新请求提交。 当您经常提交类似请求时，这非常有用。 在这种情况下，您可以重复使用现有请求，进行一些更改，然后作为新请求提交。

根据这项更改，可以查看其他人提交的请求的用户也可以复制这些请求并将其作为新请求提交。 您可以通过更新请求队列项目中的以下设置来阻止这种情况发生：来自同一公司的人员将继承所有请求的相同权限。

>[!NOTE]
>
>在发布此功能之前，您无法复制并重新提交已提交到请求队列的问题，而没有队列主题。

有关更多信息，请参阅 [复制和提交请求](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## 更新了“请求”区域“已提交”部分的“摘要”面板体验

>[!NOTE]
>
>此功能于2021年11月12日从预览环境中暂时删除。 以后将重新添加该日期。

为了提高“摘要”面板的可见性和与“摘要”面板的交互性，我们在“请求”区域的“已提交”部分的“打开摘要”图标中添加了标签。 标签现在为动态标签，它会根据面板是打开还是关闭进行更新。

在未首先选择请求的情况下打开“摘要”面板时，现在会显示一个更加用户友好的图像，以明确指示用户在打开面板之前选择项目。 有关更多信息，请参阅 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

此外，根据这项变化，任务、问题和文档的“摘要”面板也进行了更新。 有关“摘要”面板的信息，请参阅 [概要概述](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
