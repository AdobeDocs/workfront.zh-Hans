---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront和Frame.io本机集成alpha：功能'
description: Adobe Workfront与Frame.io原生集成Alpha的计划功能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 15e2869417d8315bf8e96f7d9d537cd70a5e39df
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 0%

---

# Adobe Workfront和Frame.io本机集成alpha：功能和测试

通过这种集成，我们的目标是让创意人员留在他们选择的工具（CC或Frame.io）中来执行其内容创建和同行审阅，同时让项目经理从Workfront内部协调工作并初始化和监控正式审阅流程。 这可以通过利用两种解决方案中的最佳功能来实现：Workfront用于管理内容批准的新文档批准，以及Frame.io提供的内容审查功能。 总之，新文档批准和Frame.io将形成我们新的端到端内容审查和批准体验。 

要详细了解Alpha的运行方式和参与方式，请参阅 [Adobe Workfront和Frame.io集成alpha：概述](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>如果您是在没有您的公司参与此Alpha程序的情况下访问这些页面的，请确保谨慎处理此处的信息，并联系Workfront或Frame.io管理员以获取更多信息。

## 基本测试场景

为了让您轻松测试alpha程序的新功能，我们创建了一个新的测试Frame.io帐户，并将其连接到一个名为的新组 `Frame.io alpha testing` 在现有Workfront预览或沙盒环境中。

要测试该功能，请登录Workfront预览版或沙盒实例并执行以下步骤：

>[!NOTE]
>
><span class="preview">突出显示的文本</span> 以下提及尚未用于测试但将包含在更高版本中的功能。
>

1. **协调员：** 在Workfront中，使用创建项目 `Frame.io alpha testing` 组被指定为项目组。

1. **协调员：** 在Workfront中，将您的创意分配给项目 <span class="preview">或启用帧的任务</span> 并将项目状态更改为“当前”。

1. **创意人员：** 检查您的电子邮件中是否有邀请加入新创建的Frame.io项目

1. **创意人员：** 单击邀请电子邮件中的“加入项目”按钮，加入Frame.io项目，查看项目中的创意简报，然后在所选的Creative Cloud工具中开始创建内容。

1. **创意人员：** 将您创建的资源上传到Frame.io，并将其添加到链接的Workfront项目 <span class="preview">（或已分配了支持框架的任务）。</span>

1. **协调员：** 在Workfront中，找到项目中链接的Frame.io资源并分配审阅人/批准者(有关分配审阅人/批准者的详细信息，请参阅 [向文档添加其他批准者或审阅者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md))。

1. **利益相关者：** 在Workfront中，在“主页”或“文档详细信息”中查看您的审批请求，并在Frame.io查看器中查看框架连接的文档，然后留下包含反馈的注释。

1. <span class="preview">**协调员：** 在Workfront中，查看利益相关者在Frame.io连接文档的“更新”部分创建的评论。</span>

1. <span class="preview">**利益相关者：** 在Frame.io查看器中做出决策。</span>

1. <span class="preview">**创意人员：** 在Frame.io中，请注意针对您的资源作出的整体批准决定。</span>

1. **创意人员：** 在Frame.io中，通过将更新版本添加到所连接资源的版本栈栈来应用请求的更改。

1. **协调员：** 在Workfront中，将审批者/审阅者分配给新上传的版本，并监控进度，直到该版本实现注销。

## 功能计划

以下是有关我们寻求解决的主要用例以及我们当前计划这样做的功能的信息。 <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">突出显示的文本</span> 以下提及尚未实施，但将包含在更高版本中的功能。
>
>项目符号下 **“未来版本中的潜在改进”** 根据Alpha反馈和我们不断演变的开发计划，标头可能会也可能不会包含在将来的版本中。
>


### Workfront管理员可以在Workfront组和Frame.io帐户之间建立连接

* <span class="preview">在Workfront中，您可以将Workfront组连接到Frame.io帐户</span>

* 将在Frame.io中创建一个新的Frame.io团队，表示连接的Workfront组

**未来版本中的潜在改进：**

* 从Frame.io帐户断开Workfront组的连接

* 将Workfront组连接到现有的Frame.io团队

### 项目协调员可以配置将哪些Workfront项目发送到Frame.io，并将Workfront中分配的创意添加到Frame.io中的项目

* 能够通过分配连接了帧的组将Workfront项目标记为Frame.io已启用

* <span class="preview">增强：能够将Workfront项目中的任务切换为框架任务，这反过来将在Frame.io中创建任务文件夹</span>

* 当Workfront项目状态设置为“当前”时，将在Frame中创建相应的已连接项目，并将为Workfront分配的用户添加到Frame项目，并从Frame.io向他们发送电子邮件通知

   * 所有Workfront项目成员（用户和团队）将作为协作者添加到Frame.io项目（在创建项目时和以后创建项目时）

   * <span class="preview">更改：分配给“已启用Frame的Workfront”任务的用户和团队将作为协作者添加到Frame.io项目中，并在以后创建项目时收到通知</span>

* 添加到项目中的文档（创意摘要）以及启用Frame的任务将在创建项目时推送到Frame.io项目（位于相应的工作文件夹中）（触发器：项目状态设置为当前）

   * 我们建议您先限制添加到项目中的文档数量，然后再激活到创意摘要，以避免向Frame.io发送多个不必要的文档

* <span class="preview">增强：从Frame.io项目中删除从启用了框架的Workfront任务中明确取消分配的用户/团队</span>

**未来版本中的潜在改进：**

* 可以在项目模板上配置启用帧的任务

* 上传到创意简报的新版本将推送至框架

* 优化了项目同步（断开项目连接、重新同步项目和文档等）

### 在Frame.io中，创意人员可以将创建的资源发送到Workfront项目进行正式审查

* 能够将单个Frame.io资源连接到WF项目或任务。 将在Workfront中创建资源引用

* 在Frame.io中上传的新版本将在Workfront中自动在连接的资源上创建新文档版本

* <span class="preview">增强：能够从Frame.io中将引用的Workfront任务标记为完成</span>

* <span class="preview">增强：如果已连接的Workfront文档被删除，则它保留在Frame.io中，并可重新连接到同一项目任务或其他项目任务</span>

**未来版本中的潜在改进：**

* 能够一次将多个Frame.io资源发送到Workfront

* 从Frame.io中针对Workfront项目/任务记录时间

### 项目协调员可以将正式批准流程分配给从Frame.io链接的文档

* 可以将Workfront用户和团队添加到用于连接Frame.io的文档的新文档审批中

* <span class="preview">增强：当用户/团队从启用了Frame的文档取消共享时，他们也将失去对Frame.io查看器中的资产的访问权限</span>

**未来版本中的潜在改进：**

* 以单个审核方式发送多个资产

* 将审批者/审阅者批量分配给Workfront文档

### 利益相关者可以在Frame.io查看器中执行审核和批准

* 利益相关者将收到通知，可以在Frame.io查看器中查看框架连接的文档

* 可以从Workfront内的不同位置访问Frame.io查看器，例如文档列表、文档详细信息、Workfront主页

* 能够利用Frame.io查看器提供的现有审阅和注释功能，这些功能将与Workfront的更新流同步

* <span class="preview">能够在Frame.io查看器中作出新的文档批准决策</span>

### 在Frame.io中，将通知创意人员有关所连接Frame.io资产的整体决策

* <span class="preview">增强：Frame.io内的资产将显示整体文档审批状态</span>

### 项目协调员可以将最终资源发送到AEM

* <span class="preview">增强：可以使用现有的Workfront + AEM Asset CS连接器将包含元数据的帧连接文档发送到AEM</span>
