---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront和Frame.io本机集成alpha：功能'
description: Adobe Workfront与Frame.io原生集成Alpha的计划功能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Adobe Workfront和Frame.io本机集成alpha：功能

## 用例和功能测试

通过这种集成，我们的目标是让创意人员留在他们选择的工具（CC或Frame.io）中来执行其内容创建和同行审阅，同时让项目经理从Workfront内部协调工作并初始化和监控正式审阅流程。 这可以通过利用两种解决方案中的最佳功能来实现：Workfront用于管理内容批准的新文档批准，以及Frame.io提供的内容审查功能。 总之，新文档批准和Frame.io将形成我们新的端到端内容审查和批准体验。 

要详细了解Alpha的运行方式和参与方式，请参阅 [Adobe Workfront和Frame.io集成alpha：概述](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>如果您是在没有您的公司参与此Alpha程序的情况下访问这些页面的，请确保谨慎处理此处的信息，并联系Workfront或Frame.io管理员以获取更多信息。

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## 功能计划

以下是有关我们寻求解决的主要用例以及我们当前计划这样做的功能的信息。 <!--, along with documentation to get you started testing.-->


### Workfront管理员可以在Workfront组和Frame.io帐户之间建立连接

* _在Workfront中，您可以将Workfront组连接到Frame.io帐户_

* 将在Frame.io中创建一个新的Frame.io团队，表示连接的Workfront组

**未来版本中的潜在改进：**

* 从Frame.io帐户断开Workfront组的连接

* 将Workfront组连接到现有的Frame.io团队

### 项目协调员可以配置将哪些Workfront项目发送到Frame.io，并将Workfront中分配的创意添加到Frame.io中的项目

* 能够通过分配连接了帧的组将Workfront项目标记为Frame.io已启用

* _增强：能够将Workfront项目中的任务切换为框架任务，这反过来将在Frame.io中创建任务文件夹_

* 当Workfront项目状态设置为“当前”时，将在Frame中创建相应的已连接项目，并将为Workfront分配的用户添加到Frame项目，并从Frame.io向他们发送电子邮件通知

   * 所有Workfront项目成员（用户和团队）将作为协作者添加到Frame.io项目（在创建项目时和以后创建项目时）

   * _更改：分配给“已启用Frame的Workfront”任务的用户和团队将作为协作者添加到Frame.io项目中，并在以后创建项目时收到通知_

* 添加到项目中的文档（创意摘要）以及启用Frame的任务将在创建项目时推送到Frame.io项目（位于相应的工作文件夹中）（触发器：项目状态设置为当前）

   * 我们建议您先限制添加到项目中的文档数量，然后再激活到创意摘要，以避免向Frame.io发送多个不必要的文档

* _增强：从Frame.io项目中删除从启用了框架的Workfront任务中明确取消分配的用户/团队_

**未来版本中的潜在改进：**

* 可以在项目模板上配置启用帧的任务

* 上传到创意简报的新版本将推送至框架

* 优化了项目同步（断开项目连接、重新同步项目和文档等）

### 在Frame.io中，创意人员可以将创建的资源发送到Workfront项目进行正式审查

* 能够将单个Frame.io资源连接到WF项目或任务。 将在Workfront中创建资源引用

* 在Frame.io中上传的新版本将在Workfront中自动在连接的资源上创建新文档版本

* _增强：能够从Frame.io中将引用的Workfront任务标记为完成_

* _增强：如果已连接的Workfront文档被删除，则它保留在Frame.io中，并可重新连接到同一项目任务或其他项目任务_

**未来版本中的潜在改进：**

* 能够一次将多个Frame.io资源发送到Workfront

* 从Frame.io中针对Workfront项目/任务记录时间

### 项目协调员可以将正式批准流程分配给从Frame.io链接的文档

* 可以将Workfront用户和团队添加到用于连接Frame.io的文档的新文档审批中

* _增强：当用户/团队从启用了Frame的文档取消共享时，他们也将失去对Frame.io查看器中的资产的访问权限_

**未来版本中的潜在改进：**

* 以单个审核方式发送多个资产

* 将审批者/审阅者批量分配给Workfront文档

### 利益相关者可以在Frame.io查看器中执行审核和批准

* 利益相关者将收到通知，可以在Frame.io查看器中查看框架连接的文档

* 可以从Workfront内的不同位置访问Frame.io查看器，例如文档列表、文档详细信息、Workfront主页

* 能够利用Frame.io查看器提供的现有审阅和注释功能，这些功能将与Workfront的更新流同步

* _能够在Frame.io查看器中作出新的文档批准决策_

### 在Frame.io中，将通知创意人员有关所连接Frame.io资产的整体决策

* _增强：Frame.io内的资产将显示整体文档审批状态_

### 项目协调员可以将最终资源发送到AEM

* _增强：可以使用现有的Workfront + AEM Asset CS连接器将包含元数据的帧连接文档发送到AEM_