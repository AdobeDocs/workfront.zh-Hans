---
product-area: documents
navigation-topic: approvals
title: Frame.io集成入门
description: Frame.io集成入门。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# Frame.io集成入门

Workfront和Frame.io集成使创意人员、营销人员和利益相关者与无缝工作流程保持一致。 访问实时更新，避免重复工作，并确保资产在启动之前获得批准。

有关Frame.io的详细信息，请参阅[Frame.io快速入门](https://support.frame.io/en/collections/49298-getting-started)。

## Workfront中的工作启动和规划

项目协调员可以在Workfront中创建项目和计划工作。 在启用了Frame.io集成的实例中创建的项目，将利用Adobe企业存储，从而允许在Adobe生态系统中存储和管理资产。

如果您的组织具有Frame.io Enterprise许可证，则在Workfront中创建的项目也可在Frame.io中看到，从而允许用户在任何一个产品中进行交互和上传资源。

有关Adobe Enterprise Storage或Frame.io中的项目的信息，请参阅

* [Workspace概述：项目](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)

## 审阅和批准资源

资源完成后，项目协调员可以在Workfront中启动正式审查和批准流程。

创建批准工作流后，审阅人和批准者可以使用Frame.io查看器添加注释并标记资产。 他们还可以在Frame.io查看器中作出批准决定。

有关设置项目的更多信息，请参阅

* [创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Frame.io集成概述](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### 在Workfront中启动正式审查和批准

项目协调员可以创建一次性审阅和审批或可恢复审批模板。 他们可以分配审阅人、批准人或两者的组合：

* **审阅人**&#x200B;可以添加评论和标记资源。 完成后，他们可以将其审阅标记为完成。 资产无需在审批流程中继续前进，即可将审核标记为完成。
* **审批者**&#x200B;可以添加评论和标记资源。 他们必须决定推进审批流程。

#### 创建审阅和批准工作流

可以将审阅人和审批人添加到一次性审批工作流或可重复使用的审批模板中：

* **一次性审批**：在资产所在的项目或任务中，项目协调器可以分配审阅人和审批人并设置完成截止日期。 查看者和审批者将在截止日期前72小时、截止日期前24小时以及截止日期本身收到电子邮件提醒。

  有关详细信息，请参阅[创建文档审阅或审批请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

* **审批模板**：在Workfront设置区域，项目协调员可以创建可恢复的审批模板。 在模板中，用户可以添加审阅人和批准者，并指定完成时间范围。 将审批模板应用于资产时，截止日期从指定的时间范围中计算。

  创建模板后，可将其应用于资源以在Workfront中开始正式审查和批准流程。

  有关详细信息，请参阅[创建批准模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。


  ![分配模板](assets/assign-template.png)

### 在Frame.io查看器中审阅和批准资源

在Workfront中启动审阅和批准工作流后，审阅人和批准者可以访问Frame.io查看器以添加注释、标记资产并做出决策。

有关详细信息，请参阅[使用Frame.io查看器审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)。

#### 访问Frame.io查看器

用户可以通过以下方式访问Frame.io查看器：

* Workfront电子邮件通知
* Workfront主页区域中的我的审批小组件

>[!NOTE]
>
>外部Workfront用户会通过电子邮件收到通知，并被要求创建一个Frame.io登录名来查看和批准资源。

![从主页打开帧查看器](assets/open-fio-viewwer.png)

#### 添加注释和标记资源

注释和资产标记在Frame.io查看器中可见。 有关使用Frame.io查看器的详细信息，请参阅[在媒体上发表评论](https://help.frame.io/en/articles/9105251-commenting-on-your-media)。

#### 做出决定

完成所有审阅活动后，审批者必须作出以下决策之一：

* **批准**：该资产不需要更改，可以随时使用。
* **需要工作**：该资产需要更改，并且未准备就绪。 完成指定的更改后，必须将资源上传为新版本，并经过另一轮批准。<!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

审阅人可以在Workfront中将他们的审阅标记为完成，但资产在审批过程中无需进行此标记。

有关Workfront中决策的详细信息，请参阅[文档决策状态概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)。

![帧查看器和决策](assets/decision-fio.png)


### 跟踪审阅和批准指标

项目协调员可以在Workfront主页区域或通过画布功能板中的自定义报告监控所有正在进行的审批的进度：

* **自定义仪表板**：在“画布仪表板”区域创建一个报告仪表板，以显示有关具有统一审批功能的审阅和审批的高级和详细信息。 有关如何开始的信息，请参阅[创建报表仪表板以供审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。
* **文档审批量度主页小组件**：显示2个图表，其中包含有关平均审批时间和决策的信息以及待审批和超期审批的列表视图。
  ![所有审批](assets/all-approvals.png)