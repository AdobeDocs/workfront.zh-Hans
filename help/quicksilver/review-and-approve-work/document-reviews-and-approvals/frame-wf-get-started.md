---
product-area: documents
navigation-topic: approvals
title: 开始使用Frame.io进行资产审查和批准
description: 了解有关使用Workfront和Frame.io中的正式审核和批准流程的更多信息。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# 开始使用Frame.io进行资产审查和批准

新的资源审查和批准工作流程是围绕Workfront与Frame.io之间的紧密集成构建的。 此集成充分利用了每个产品所具有的功能，并将它们组合在一起，创建出一种体验，使得参与内容创建的每个人都可以使用他们选择的工具进行工作，同时还可以访问评论、文件和状态更新 — 所有这些内容都实时跨两个系统同步。

有关Frame.io的详细信息，请参阅[Frame.io快速入门](https://support.frame.io/en/collections/49298-getting-started)。

## Workfront中的工作启动和规划

Workfront管理员通过在“设置”区域中配置默认Frame.io帐户，然后在Workfront中指定Frame.io用户，来启用Workfront与Frame.io之间的集成。 这允许协调员使用Workfront项目以及正式的审阅和批准工作流来计划和启动工作。

### 配置默认Frame.io帐户[!BADGE 即将推出]{type=Informative}

Workfront管理员通过在Workfront的“设置”区域添加默认的Frame.io帐户来启动Workfront和Frame.io集成。 设置默认的Frame.io帐户后，在Workfront中创建的任何项目都将在Frame.io中创建镜像项目。

>[!IMPORTANT]
>
>此功能即将推出。 目前，Frame.io帐户由Workfront团队手动添加。 请联系您的Adobe客户代表寻求帮助。

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### 启用Frame.io用户现在可用

经常使用Frame.io的Workfront用户应标记为Frame.io用户。 Workfront管理员可以在Workfront用户配置文件中指定Frame.io用户。

>[!TIP]
>
>我们建议使经常使用创意工具并上传资源的用户能够作为Frame.io用户进行审阅和批准。

在Workfront中将用户标记为Frame.io用户并将其添加到项目中时：

* 它们将作为协作者添加到Frame.io中。
* 他们可以将Frame.io中的资源发送到Workfront以进行正式审查和批准。
* 他们可以从Workfront的单向同步文件夹中查看信息。 [!BADGE 即将推出]{type=Informative}

有关详细信息，请参阅[配置 [!DNL Workfront] 和 [!DNL Frame.io] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md)。

![帧启用的用户](assets/Frame-enabled-user.png)


### 创建与Frame.io连接的项目

添加默认Frame.io帐户并指定Frame.io用户后，项目协调员可以创建与Frame.io连接的Workfront项目。 在创建连接的项目时，您可以

* **将Frame.io用户分配给任务**：启用Frame.io的用户在分配给Workfront任务时会收到电子邮件通知，告知有工作要完成。
* **与Frame.io用户共享项目**：与启用了Frame.io的用户共享项目时，用户可以访问Workfront和Frame.io中的项目。
* **与Frame.io共享创意资料**：项目协调员可以使用单向同步项目文件夹，直接从Workfront将说明和资料发送给Frame.io中的创意用户。 [!BADGE 即将推出]{type=Informative}
* **跟踪任务进度**：创意人员可以发送完成的资源并将任务标记为完成 — 所有这些操作无需离开Frame.io。

有关详细信息，请参阅[创建与Frame.io连接的项目](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md)。


## Frame.io中的内容创建和协作

创意人员可以停留在他们选择的工具中，并自由地在Frame.io中创建、迭代和执行同行评审。

将创意添加到连接的项目时，他们可以在Frame.io中执行以下操作：

<!--* Access instructions from the project coordinator -->
* 进行非正式同行审查
* 将完成的资源发送到Workfront进行正式审查和批准
* 更改任务的状态或将其标记为完成
* 上载新版本，然后重新提交它们以供审批<!--do they have to send to frame.io again?-->

有关Frame.io的详细信息，请参阅[我受邀对项目进行协作](https://support.frame.io/en/articles/11125-i-ve-been-invited-to-collaborate-on-a-project)。

## 审阅和批准资源

一旦创意人员将完成的资产从Frame.io发送到Workfront，项目协调员就可以在Workfront中启动正式的审核和批准流程。

创建批准工作流后，审阅人和批准者可返回Frame.io添加注释并标记资产。 他们还可以在Frame.io查看器中作出批准决定。

### 在Workfront中启动正式审查和批准

项目协调员可以创建一次性审阅和审批或可恢复审批模板。 Frame.io中的所有审阅和批准活动也会记录在Workfront中。

项目协调员可以选择分配审阅人、批准者或两者的组合：

* **审阅人**&#x200B;可以添加评论和标记资源。 完成后，他们可以将其审阅标记为完成。 资产无需在审批流程中继续前进，即可将审核标记为完成。
* **审批者**&#x200B;可以添加评论和标记资源。 他们必须决定推进审批流程。


#### 创建审阅和批准工作流

可以将审阅人和审批人添加到一次性审批工作流或可重复使用的审批模板中：

* **一次性审批**：在资产所在的项目或任务中，项目协调器可以分配审阅人和审批人并设置完成截止日期。 截止日期前72和24小时，以及截止日期本身，通过电子邮件提醒查看者和审批者。

  有关详细信息，请参阅* [为Frame.io资源创建审阅或批准请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md)。

* **审批模板**：在Workfront设置区域，项目协调员可以创建可恢复的审批模板。 在模板中，用户可以添加审阅人和批准者，并指定完成时间范围。 将审批模板应用于资产时，截止日期从指定的时间范围中计算。

  创建模板后，可将其应用于从Frame.io发送的资源，以在Workfront中开始正式的审阅和批准流程。

  有关详细信息，请参阅[创建审批模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![分配模板](assets/assign-template.png)


#### 访问Frame.io查看器

用户可以通过以下方式访问Frame.io查看器：

* Workfront电子邮件通知
* 新Workfront主页区域中的我的审批小组件
  ![等待我的审批](assets/awaiting-my-approval.png)

>[!NOTE]
>
>外部Workfront用户会通过电子邮件收到通知，并被要求创建一个Frame.io登录名来查看和批准资源。

#### 添加注释和标记资源

在Frame.io查看器中所做的所有注释也会记录在“Workfront更新”选项卡中。 在Workfront中进行的回复不会显示在Frame.io中。 如果在Frame.io查看器中将评论标记为“仅团队”，则这些评论不会出现在“Workfront更新”选项卡中。

#### 做出决定

完成所有审阅活动后，审批者必须作出以下决策之一：

* **批准**：该资产不需要更改，可以随时使用。
* **批准，但有更改**：资产需要更改，并且更改完成后即可使用。 不需要额外审批。
* **需要工作**：该资产需要更改，并且未准备就绪。 完成指定的更改后，必须将资源上传为新版本，并经过另一轮批准。<!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

审阅人可以在Frame.io审阅人中将其审阅标记为完成，但资产在审批过程中无需进行此标记。

有关Workfront中决策的详细信息，请参阅[文档决策状态概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)。

![帧查看器和决策](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### 跟踪审阅和批准指标

项目协调员可以使用以下小组件在Workfront主页区域监控所有正在进行的审批的进度：

* **所有审批**：显示2个图表，其中包含有关平均审批时间和决策的信息，以及未决和超期审批的列表视图。
  ![所有审批](assets/all-approvals.png)
