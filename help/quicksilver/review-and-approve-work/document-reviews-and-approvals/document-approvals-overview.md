---
product-area: documents
navigation-topic: approvals
title: 统一审查和批准概述
description: 详细了解由Workfront和Frame.io提供支持的统一审阅和批准。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: d35e6c33479ed051aaa87b07ddf38811fffc0cc0
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# 统一审查和批准概述

由Workfront和Frame.io提供支持的统一审查和批准功能允许项目协调员在Workfront中管理项目和计划工作，而创意人员、营销人员和利益相关者可以在Frame.io中审查和批准资源。

## 集成要求

* Workfront和Frame.io必须部署到同一Identity Management system (IMS)组织。

* 用户只能属于IMS组织内的一个Workfront实例。

* 必须在Adobe Unified Experience和Adobe企业存储上启用Workfront实例。

* 该集成必须由Adobe Professional Services配置。


## 构建于Adobe企业级存储之上

统一审查和批准构建于Adobe企业存储之上，后者是一种基于云的存储解决方案，可作为Adobe企业产品（包括Workfront和Frame.io）中资产的中央存储库。<!--, and Creative Cloud.-->

Adobe企业存储的主要优势包括：

* 用于创意和工作管理资产的统一存储层
* 使用Adobe Identity Management system (IMS)集中管理权限以实现安全访问控制
* Workfront和Frame.io <!--, and Creative Cloud apps -->中的端到端资源可见性
* 满足企业需求的可扩展存储和配额管理

有关详细信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 统一审查和批准

通过统一审查和批准，您可以：

* 直接从Workfront创建和管理审阅和批准
* 实时跟踪审阅和批准状态
* 将反馈和批准集中到一个地方
* 确保所有利益相关者均有权访问最新版本的资产
* 利用AI评审员自动进行品牌合规性审查
* 等等

有关详细信息，请参阅[统一文档审批：文章索引](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)。


### 使用Frame.io查看器

使用Frame.io查看器审阅和批准资源。 Frame.io查看器提供

* 标记和注释工具
* 版本历史记录和比较
* 带有时间戳的视频评论评论
* 移动访问以进行移动审阅和批准

有关详细信息，请参阅[统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

#### 视频审查限制

视频验证请求的年度上限设置为组织的Workfront付费用户许可证总数的10% — 标准和轻量级。 此上限在组织级别应用。

当使用量达到上限的80%和100%时，Workfront管理员会收到通知。

此限制不适用于Frame.io Enterprise客户。

#### Frame.io查看器支持的文件类型

Frame.io查看器支持所有常见视频、图像、音频、PDF和MS® Office类型。 有关支持的文件的详细列表，请参阅Frame.io[上的](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)支持的文件类型。

#### Frame.io查看器的访问和许可

Frame.io查看器是所有Workfront审阅和批准工作流的默认查看器。 它自动包含在具有付费许可证的所有Workfront用户中。 使用Frame.io查看器进行审阅和批准不需要其他Frame.io许可证。

如果您的组织希望利用此集成中提供的其他Frame.io功能（如将资产直接上传到Frame.io中的项目），则可以购买Frame.io Enterprise许可证。 请联系您的Adobe客户代表以安排演示，并探索完整Frame.io解决方案的优势。

Workfront校对功能在此集成中不可用。

## Workfront中强大的项目管理

项目协调员可以利用Workfront强大的项目管理功能来规划、跟踪和管理工作。

有关在Workfront中管理项目的详细信息，请参阅[项目：文章索引](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。

### 强制的结构和命名约定

由于统一审查和批准是使用Adobe企业存储构建的，因此在管理项目和文档时，需要了解一些强制性的结构和命名约定。

* 对象名称必须是唯一的，并且不能重复
* Adobe企业存储要求层次结构树中具有相同父级的对等对象具有唯一的名称
* 如果文档属于同一项目，则不能具有相同的名称
* 文档名称不能包含以下任何特殊字符：\ / ： * ？ “ | &lt; >
* 文档名称限制为最多255个字符

考虑到这些限制，Workfront会根据需要自动重命名对象或文档，以防止冲突。

### 共享和权限

作为集成的一部分，用户权限在Workfront中进行控制，并流向Frame.io。 这意味着您无法邀请用户加入Frame.io中的项目或修改Frame.io中的用户权限。 这些操作需要通过Workfront中的项目共享模式完成。

下表显示了Workfront权限如何映射到Frame.io权限：

<table>
<tr>
<th>Workfront用户权限</th>
<th>Frame.io用户权限</th>
</tr>
<tr>
<td>管理</td>
<td>编辑和共享</td>
</tr>
<tr>
<td>贡献</td>
<td>编辑和共享</td>
</tr>
<tr>
<td>视图</td>
<td>仅注释</td>
</tr>
</table>



### Workfront中的文档管理

上传到Workfront的文档存储在Adobe企业存储中，可在Workfront和Frame.io中访问。 在Workfront中将文档上传到任务或问题时，系统会在Adobe企业存储中创建一个系统生成的文件夹，该文件夹继承任务或问题的权限。 上传到该任务或问题的所有文档都存储在该文件夹中，并从该文件夹继承权限。 有关Workfront中文档的更多信息，请参阅[新文档区域概述](/help/quicksilver/documents/managing-documents/documents-area.md)和[Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)。

### 文档体验限制

以下文档功能不包括在内：

<!--* External document providers-->
* 在Workfront中访问校对
* Workfront中的文档查看器
* 收藏的文档
* 请求文档










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->