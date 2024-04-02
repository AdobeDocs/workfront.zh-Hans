---
product-area: documents
navigation-topic: approvals
title: 资产审查和批准概述
description: 详细了解Workfront中的正式审核和批准流程。
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 63160895fc77994fdecd7aca8769b7d236d285d6
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# 资产审查和批准概述

新的资源审查和批准工作流程是围绕Workfront与Frame.io之间的紧密集成构建的。 此集成充分利用每个产品所具有的功能，并将其组合在一起，从而创造一种体验，使参与内容创建的所有角色都能够在其选择的工具中工作，同时能够实时访问跨两个系统同步的注释、文件和状态更新。

<!-- link to frame docs-->

## Workfront中的工作启动和规划

项目协调员从Workfront开始。 创建项目、分配任务并发送说明。

项目协调员创建WF项目，使用同步的项目文件夹将信息和支持资料发送给Frame.io中的创意人员

从头开始或通过模板设置审批工作流

分配任务

将项目设置为当前或等于创建框架项目和警报创意

### 配置默认Frame.io帐户

Workfront管理员通过在Workfront的“设置”区域添加默认的Frame.io帐户来启动Workfront和Frame.io集成。 设置了默认的Frame.io帐户后，集成便可以在Workfront和Frame.io之间创建连接的项目。

有关更多信息，请参阅 [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### 启用Frame.io用户

经常使用Frame.io的Workfront用户应标记为Frame.io用户。 Workfront管理员可以在Workfront用户配置文件中指定Frame.io用户。

在Workfront中将用户标记为Frame.io用户并将其添加到项目中时：

* 它们将作为协作者添加到Frame.io中
* 他们可以将Frame.io中的资源发送到Workfront以进行正式审查和批准

有关更多信息，请参阅 [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>我们建议使经常使用创意工具并上传资源的用户能够作为Frame.io用户进行审阅和批准。

### 创建与Frame.io连接的项目

项目协调员可以创建与Frame.io连接的Workfront项目。 在创建连接的项目时，您可以

* **将Frame.io用户分配给任务**：启用Frame.io的用户被分配给任务时，会收到电子邮件通知，告知他们有工作要完成。
* **与Frame.io用户共享项目**：与启用了Frame.io的用户共享的项目授予他们对Frame.io内部项目的访问权限。
* **与Frame.io共享创意材料**：您可以使用单向同步项目文件夹，在Frame.io中直接将Workfront中的说明和资料发送给创意用户。
* **跟踪任务进度**：创意人员无需离开Frame.io即可发送已完成的资源和将任务标记为完成。

有关更多信息，请参阅 [].

<!--Preassign approval templates to asks coming in the future-->


## Frame.io中的内容创建和协作

创意人员可以停留在他们选择的工具中，并自由地在Frame.io中创建、迭代和执行同行评审。

将创意添加到集成项目时，他们可以在不离开Frame.io的情况下完成以下所有操作：

* 项目协调员的访问说明
* 进行非正式同行审查
* 将完成的资源发送到Workfront进行正式审查和批准
* 更改任务的状态或将其标记为完成
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## 在Workfront中审阅和批准资源

一旦创意人员将完成的资产从Frame.io发送到Workfront，项目协调员就可以在Workfront中启动正式审查和批准流程。 所有审阅和批准活动都记录在Workfront中。

在Frame.io中所做的任何注释也会反映在Workfront的“更新”选项卡中。 在Workfront中进行的回复不会在Frame.io中反映出来。

标记为“仅限团队”的评论将不会显示在“Workfront更新”选项卡中。

### 启动正式审查和批准

您可以创建一次性审阅和批准，或在workfront的“设置”区域创建可恢复批准模板：

您可以选择分配审阅人、批准者或两者的组合：

* **审阅者** 可以对资产进行注释和标记。 完成后，他们可以将其审阅标记为完成。 <!--example of when to add reviewers-->
* **审批者** 可以添加评论、标记资产，并且必须做出决定以推进审批流程。

可以将审阅人和批准者添加到一次性使用或批准模板：

<!--can also assign teams and set deadline-->

* **一次性审批**：设置审批截止日期

* **审批模板**
在Workfront设置区域中，具有Standard许可证的用户可以创建可靠的审批模板。 在模板中，用户可以指定时间范围并添加审阅者和批准者。 <!--do we want to mention any upcoming plans here? -->

  创建模板后，可将其应用于从Frame.io发送的资源，以在Workfront中开始正式的审阅和批准流程。
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### 审阅和批准通知

与其他部分合并？

主页等待我审批的小组件电子邮件 — 截止日期电子邮件72、24和截止日期。

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### 审阅和批准资产

Frame.io连接的资产利益相关者可以在框架查看器中审阅和批准注释，并将其同步到workfront更新流、决策等

<!-- include screenshot from frame.io-->

将要求外部WF用户为框架创建登录

如果资产未连接帧，则他们可以在WF中查看缩略图并使用评论流。 可以作出审阅和批准决定。

### 跟踪审阅和批准指标

主页中的构件审批速度报表

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* 从Workfront上传资源并将其发送到框架以供审阅和批准 — 即将推出？

## 活动资产审批工作流示例

介绍段落？

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->