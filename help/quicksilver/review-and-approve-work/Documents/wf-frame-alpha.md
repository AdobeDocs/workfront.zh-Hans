---
product-area: documents
navigation-topic: approvals
title: Beta计划 — Workfront + Frame.io
description: 我们很高兴地宣布推出Workfront + Frame.io的Beta计划。 您将在此处找到有关最新Beta版本的信息，以及引导您入门的简短视频演练。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 23d1e241-ea5b-43f5-b097-8d96e13cb267
source-git-commit: 2c9d52ad5e3d330d0a183d9cef545ff6b6aed6b2
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Beta计划 — Workfront + Frame.io

欢迎使用Workfront + Frame.io集成测试版计划！ 作为此测试版的一部分，您将可以抢先体验我们的Workfront + Frame.io原生集成，并可以分享您的反馈，这些反馈将最终影响我们向更广泛的客户群发布的最终体验。 借助此集成，我们的目标是在Workfront和Frame.io之间创建一个顺畅的端到端工作流程，重点是提供理想的统一审核和批准解决方案。

您将在此处找到有关最新Beta版本的信息，以及引导您入门的简短视频演练。

>[!NOTE]
>
>要参与此测试版，您必须由产品团队启用。 联系您的客户成功案例或客户经理并请求添加。


## Frame.io中的Beta版更新 — 2024年3月

在此测试版中，我们具有：

### 将多个资源从Frame.io添加到Workfront

现在，您最多可以一次性将10个资源从Frame.io添加到Workfront。 您可以选择添加到Workfront项目文档或特定项目任务。

### 改进了将Frame.io资源添加到Workfront时的体验

更新了用于将资源添加到Workfront的菜单项，以便更轻松地查看分配给您的任务、任务层次结构和任务状态。

>[!VIDEO](https://video.tv.adobe.com/v/3428213/)

## Workfront中的Beta版更新 — 2024年3月

在此测试版中，我们具有：

### 向文档审阅和审批添加截止日期

您现在可以为被分派审阅或审批文档的用户或团队指定截止日期。 查看者和批准者在指定截止日期前72小时和之后24小时收到电子邮件通知。 截止日期还反映在新“主页”区域的审批构件中。

有关更多信息，请参阅 [创建文档审阅或审批请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

### 创建和使用审批模板

您现在可以在“设置”区域创建批准模板，以简化审阅和批准流程。 批准模板允许您通过以下方式使审阅和批准流程更可重复

* 添加审阅者和批准者
* 设置时间范围

在为文档创建审批流程时，您可以从“文档”区域应用审批模板。

有关更多信息，请参阅 [创建审批模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

### 一次性查看有关所有审批的信息

为帮助您管理和分析批准请求概览，我们在“所有批准”构件中添加了以下关键绩效指标：

* 按决策审批
* 平均审批时间
* 待处理审批
* 逾期审批

您可以深入查看上面列出的类别，以获取更详细的视图。 “所有审批”小组件在新主页和画布功能板中提供。

有关更多信息，请参阅 [新主页入门](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

### 做出总体决策后锁定您的审阅和批准

为了确保法规遵从性和减少内容签核过程中的流失，我们将在作出总体决策后锁定文件上的任何批准。 这包括“已批准”、“已批准但有更改”或“需要工作”。

一旦锁定，审阅和/或批准的任何人员将无法再做出任何评论、回复、决策或添加绘图标记，从而确保您的审阅流程和相关审核保持不变。

上传新文档版本时，可以启动下一轮修订，同时保持锁定以前的修订。

>[!VIDEO](https://video.tv.adobe.com/v/3428179/)

## 功能测试

通过这种集成，我们的目标是让创意人员留在他们选择的工具（CC或Frame.io）中来执行其内容创建和同行审阅，同时让项目经理从Workfront内部协调工作并初始化和监控正式审阅流程。 这可以通过利用两种解决方案中的最佳功能来实现：Workfront用于管理内容批准的新文档批准，以及Frame.io提供的内容审查功能。 总之，新文档批准和Frame.io将形成我们新的端到端内容审查和批准体验。 

为了让您轻松测试Beta计划的新功能，我们创建了一个新的测试Frame.io帐户，并将其连接到一个名为的新组 `Frame.io testing` 在现有Workfront预览或沙盒环境中。

+++展开以查看基本测试说明

要测试该功能，请登录Workfront预览版或沙盒实例并执行以下步骤：

1. **协调员：** 在Workfront中，使用创建项目 `Frame.io testing` 组被指定为项目组。

1. **协调员：** 在Workfront中，将需要创意工作的任务标记为已启用框架（在任务详细信息中），并将您的创意分配给该任务（如果您希望测试整个工作流，请一并分配）。

>[!NOTE]
>
>子任务不能标记为已启用框架。
>

1. **协调员：** 上传您的创意简报并将项目状态更改为“当前”。

1. **创意人员：** 检查您的电子邮件中是否有邀请加入新创建的Frame.io项目

1. **创意人员：** 单击邀请电子邮件中的“加入项目”按钮，加入Frame.io项目，查看项目中的创意简报，然后在所选的Creative Cloud工具中开始创建内容。

1. **创意人员：** 将您创建的资源上传到Frame.io，并通过选择其中一个分配的启用Frame的任务来将其添加到链接的Workfront项目。 选择选项以将任务标记为完成。

1. **协调员：** 在Workfront中，在启用了frame的任务中找到链接的Frame.io资源，并检查该任务的状态是否更改为“完成”。

1. **协调员：** 将审阅者/批准者分配给链接的Frame.io资产。 如果要测试整个工作流，请将您自己指定为批准者。 (有关分配审阅/批准者的详细信息，请参阅 [向文档添加其他批准者或审阅者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md))。

1. **利益相关者：** 在Workfront的“主页”、“文档详细信息”或接收的电子邮件通知中查看您的审批请求。 在Frame.io查看器中打开资产，留下包含反馈的注释，然后做出决定。

1. **协调员：** 在Workfront中，查看在Frame.io连接文档的更新部分中创建的利益相关者评论，以及审批部分或文档摘要窗格中的决策。

1. **创意人员：** 在Frame.io中，请注意针对您的资源作出的整体批准决定。

1. **创意人员：** 在Frame.io中，通过将更新版本添加到所连接资源的版本栈栈来应用请求的更改。

1. **协调员：** 在Workfront中，将审批者/审阅者分配给新上传的版本，并监控进度，直到该版本实现注销。

+++

+++ 展开以查看详细的测试说明

对于希望测试附加功能的参与者，我们创建了一个更复杂的测试场景。 可在此处下载此详细测试方案的指南： [WF + Frame.io详细测试方案演练](/help/quicksilver/review-and-approve-work/Documents/assets/wf-frame-detailed-walk-through-may-release.pdf).
+++

<!-- 
## Demo Video

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)
-->

## 发送反馈

我们重视您的投入，并相信您的观点对于帮助我们创造尽可能最好的产品至关重要。

由于您对贵公司在生产环境中采用此解决方案所需条件有具体的反馈，请发送至 [etienneb@adobe.com](mailto:etienneb@adobe.com).
