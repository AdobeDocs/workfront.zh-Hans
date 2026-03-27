---
product-area: documents
navigation-topic: approvals
title: 统一审查和批准概述
description: 详细了解由Workfront和Frame.io提供支持的统一审阅和批准。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: f0cdbcb790af59245d550157e7d088503c60df24
workflow-type: tm+mt
source-wordcount: '3871'
ht-degree: 0%

---


# 统一审查和批准概述

统一的审核和批准将Adobe Workfront和Adobe Frame.io融于一个相互深入关联的体验中，从而弥合了营销管理、创意审核和内容交付之间的差距。
项目协调员在Workfront中管理工作，而创意人员、营销人员和利益相关者在Frame.io专业级查看器中审阅和批准资源，所有这些操作都无需在断开连接的工具之间移动文件。

![显示统一审阅和批准工作流的图表，其中项目协调员管理Workfront中的工作，审阅者和批准者在Frame.io查看器中提供反馈并做出决策。](assets/Unified-Review-Approvals-Image.png)

## 演示视频

>[!VIDEO](https://video.tv.adobe.com/v/3471078)


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

* 对象名称必须是唯一的，并且不能重复。
* Adobe企业存储要求层次结构树中具有相同父级的对等对象具有唯一的名称。
* 如果文档属于同一项目，则不能具有相同的名称。
* 对象名称不能包含以下任何特殊字符： \ / ： * ？ “ | &lt; >
* 对象名称限制为最多255个字符。

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




## 常见问题

### 统一审查和批准快速入门

+++ 展开以查看统一审查和批准快速入门的常见问题解答。

**什么是统一审阅和批准？**

统一审阅和批准是Adobe Workfront与Adobe Frame.io之间的本机集成，它将工作管理和创意审阅整合在单个连接的系统中。 项目协调员在Workfront中规划和跟踪工作，而审阅者和批准者使用专业级Frame.io查看器提供反馈、标记资源并作出批准决策，而无需在单独的工具或手动移动文件之间切换。

审核和批准是每个内容操作的中心。 它是创造性工作、利益相关者投入和业务决策汇聚的地方。 当这个过程被分散在断开连接的工具（电子邮件线程、聊天消息、屏幕快照标记）中时，结果会复杂化：上市时间变慢、反馈丢失、版本混淆，以及花费在管理文件而不是创建内容上的时间。

统一审阅和批准通过用一套现代系统代替零散散的审阅工具来解决这个问题 — 这套系统是一个真实性的单一来源，存在于工作已经发生的区域。

**使用此集成的要求是什么？**

要使用统一审阅和批准，必须满足以下条件：

* Workfront和Frame.io必须部署到同一Adobe Identity Management System (IMS)组织。

* 用户只能属于IMS组织内的一个Workfront实例。

* 必须在Adobe Unified Experience和Adobe企业存储上启用Workfront实例。

* 该集成必须由Adobe Professional Services配置。

* Workfront客户必须使用V2 SKU（这可能需要签订合同 — 请联系您的Adobe客户代表）。

**我是否需要Frame.io许可证才能使用此集成？**

不可以。对于拥有付费许可证的所有Workfront用户，Frame.io查看器会自动包含在内，无需额外付费。 您不需要单独的Frame.io许可证即可通过Workfront审查和批准资源。

如果您的组织希望访问其他Frame.io功能（如将资产直接上传到Frame.io中的项目），则可以购买Frame.io Enterprise许可证。 请联系您的Adobe客户代表以了解更多信息。

**它是否取代Workfront Proof？**

可以。启用统一审阅和批准后，Frame.io查看器将成为Workfront中的主要审阅界面，取代Workfront Proof。

对于在启用集成之前创建的任何项目，现有客户将保留对Workfront验证功能的访问权限。

**如何获得统一审查和批准的访问权限？**

**我需要做什么才能获得访问权限？**

要访问统一的审核和批准，您的组织必须位于Workfront V2 SKU上。 如果您当前不在V2 SKU上，则需要与Adobe签订合同事件。 若要开始，请执行以下操作：

* 请联系您的Adobe客户代表，以确认您当前的Workfront计划是否支持统一审查和批准。

* 如果需要升级SKU，您的客户代表将指导您完成合同过程。

* 一旦您的帐户使用正确的SKU后，Adobe Professional Services将为您的组织配置集成。

   * 如果您不确定您的Adobe客户代表是谁，可以通过Adobe支持门户联系或访问Experience League以了解联系人选项。

+++

### 统一审阅和批准的工作方式

+++ 展开以查看有关统一审阅和批准如何工作的常见问题。

**审核和批准工作流的工作原理是什么？**

该工作流遵循以下常规步骤：

1. 项目协调员在Workfront中创建项目，并上传或链接资源。

1. 当资产准备好进行审核时，协调员会创建一个审批工作流 — 一次使用审批或应用可重复使用的审批模板。

1. 已分配的审阅人和批准者会通过电子邮件收到通知，并且可以直接在Frame.io查看器中打开资产。

1. 审阅者可以添加注释和标记。 批准者必须做出正式决定。

1. 协调员从Workfront实时跟踪状态。

**审核者和批准者之间有何区别？**

审阅人可以在Frame.io查看器中添加注释和标记资源。 完成后，他们将审阅标记为完成。 但是，审批工作流无需执行他们的操作即可前进。

审批者必须作出以下决策之一才能推进审批工作流：

* **批准**：资产已准备好按原样使用。

* **需要工作**：资产需要更改，必须作为新版本重新提交以供重新批准。

**我可以创建哪些类型的审批工作流？**

* **一次性审批**：您可以直接对项目、任务或问题中的文档创建一次性审批。 您可以根据需要分配审阅人和批准者、设置截止日期并配置多个阶段。 自动电子邮件提醒会在截止日期前72小时、前24小时发送。

* **审批模板**：您可以在Workfront设置中创建可重用的模板。 模板定义审阅人、批准人和相对完成时间范围。 如果需要，可以创建多个阶段。 将模板应用于资产后，将自动计算截止日期。

**外部用户如何参与审阅？**

当外部Workfront用户被分配至审阅或审批时，会通过电子邮件通知他们。 系统将提示他们创建Frame.io登录以访问查看者并参与审核过程。

**如何跟踪审阅和批准进度？**

项目协调员可以通过多种方式监控所有正在实施的批准：

* Workfront主页区域中的“我的审批”小组件提供待审批和逾期审批的实时摘要。

* 文档审批量度小组件显示平均审批时间和决策细分。

* 可以在画布功能板中构建自定义报表功能板，以更深入地了解审阅和批准活动。

+++


### 审阅和批准资源和视频

+++ 展开以查看有关审阅和批准资产和视频的常见问题解答。

**对视频审阅是否有任何限制？**

可以。视频验证请求的年度上限设置为贵组织总付费Workfront用户许可证（标准和轻量级）的10%。 此上限适用于组织级别。

当使用率达到上限的80%和100%时，Workfront管理员将收到应用程序内通知。

此限制不适用于Frame.io Enterprise客户。 如果贵组织定期审查大量视频内容，请联系您的Adobe客户代表，了解有关Frame.io Enterprise许可的信息。

**同一用户能否出现在审批工作流的多个阶段？**

可以。一个用户可以分配到同一审批工作流中的多个阶段。

**我可以添加阶段以创建多阶段审批工作流吗？**

可以。支持多阶段审批工作流，允许您在每个阶段通过由不同参与者进行的连续轮次审阅和审批来路由资产。

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**审批模板是否可以包含组、团队或仅包含个人用户？**

目前，审批模板支持单个用户和团队。

**当审批者有需要审核的内容时，是否会通过电子邮件通知他们？**

可以。批准者和审阅者会在被分配到审阅或批准任务时收到电子邮件通知。 自动提醒电子邮件也会在截止日期前72小时、前24小时以及截止日期本身发送。

自定义电子邮件通知消息的功能目前不可用，但位于产品路线图中。

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**我是否可以保持其他参与者的审阅阶段私密性？**

当前没有专用暂存功能。 为了不向其他参与者公开审阅，建议的方法是专门为该审阅组创建单独的资产副本。 目前，评论不会按单个资产中的参与者组进行分段。

请注意，版本历史记录（包括过去和当前版本）始终对有权查看该资源的任何人可见。

**评论是否可以标记为已解决？**

可以。可在Frame.io查看器中将注释标记为已解决。

**Frame.io查看器中提供了哪些标记和注释工具？**

Frame.io查看器包括一组完整的可视标记工具，其中包括手绘绘图和标准形状，如圆形、箭头和正方形。 对于视频资源，评论带有时间戳，并具有帧精度，因此反馈始终与剪辑中的确切时间绑定，而不只是常规时间戳。

**在Frame.io查看器中所做的注释是否会出现在Workfront项目中？**

注释和批注保留在Frame.io查看器中，以便它们保留完整的上下文，包括时间戳和可视标记。 这在未来版本中可能会有所改进。

**是否可以向资源的下载版本（如PDF）添加注释？**

目前不支持此功能，但这是一项常用的功能，正在考虑在将来的版本中使用。

**能否将多个资产作为一个组一起审核？**

即将推出增强的批量审查选项。 同时，不同文件类型的资产（如视频和Word文档）可以一起包含在分组资产审核中。

**是仅对视频进行统一审阅和批准，还是支持其他文件类型？**

统一审阅和批准针对所有资产类型，而不仅仅是视频。 Frame.io查看器已得到重大更新，除了视频之外，还支持图像、文档、PDF和其他常见文件格式。

有关支持的文件类型的完整列表，请参阅Experience League上的Frame.io支持的文件类型文档。

**我是否可以在外部与无权访问Workfront的利益相关者共享资源？**

可以。Assets可以在外部共享。 系统会通过电子邮件通知外部用户，并提示外部用户创建Frame.io登录以访问查看器并参与审核。

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### 存储和文件管理

+++ 展开以查看有关存储和文件管理的常见问题。

**什么是Adobe企业存储以及它与此集成有何关系？**

Adobe企业存储是连接Workfront、Frame.io和Adobe Creative Cloud的通用存储层。 Assets位于一个位置，无需手动文件传输即可跨工具访问。 创意人员可以就地工作，审阅人始终会看到最新版本。

Adobe企业存储的主要优势包括：

* 一个存储层，用于跨Workfront和Frame.io的所有进程中的资源

* 通过Adobe Identity Management System (IMS)管理的集中访问控制

* 端到端资产可视性 — 没有版本漂移，没有丢失元数据

* 可扩展的企业级存储管理

**文件和项目是否有命名或结构要求？**

可以。由于该集成使用Adobe企业存储，因此适用以下约定：

* 对象和文档名称在文件夹层次结构的相同父级中必须是唯一的。

* 同一项目中的文档不能共享名称。

* 程序、项目组合、项目、模板、任务、问题、文档、文档文件夹名称不能包含以下特殊字符：`\\ / : \* ? \" \| \< \>`并且限制为255个字符。

Workfront会根据需要自动重命名对象或文档，以防止冲突。

**Frame.io查看器支持哪些文件类型？**

Frame.io查看器支持40多种文件格式，包括所有常见的视频、图像、音频、PDF和Microsoft Office类型。 视频支持包括专业格式（如ProRes、H.265和DNxHD）的本机播放，支持高达500 GB的文件。

Frame.io专为创意评论而构建，这意味着它可处理营销和创意团队使用的各种资产类型。

+++

### 权限和访问权限

+++ 展开以查看有关权限和访问权限的常见问题解答。

**如何管理用户权限？**

用户权限在Workfront中进行设置和控制，并自动流向Frame.io。 您不能直接在Frame.io中邀请用户或修改此集成的权限。 必须使用Workfront中的项目共享模式完成所有访问管理。

下表显示了Workfront权限如何映射到Frame.io权限：

<table>
  <thead>
    <tr>
      <th>Workfront权限</th>
      <th>Frame.io权限</th>
    </tr>
  </thead>
  <tbody>
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
  </tbody>
</table>

+++


### 集成和高级功能

+++ 展开以查看有关集成和高级功能的常见问题解答。

**这将如何影响现有Creative Cloud插件与Adobe Express和GenStudio的集成？**

当前正在开发支持Frame.io查看器体验的集成，以便用于Adobe Express和GenStudio性能营销。 新的集成将基于相同的统一审阅和批准系统构建，因此它们将利用Frame.io查看器，在所有三个产品之间提供一致的审阅体验。

**Frame.io是否已集成在Workfront中，或者用户是否导航到单独的界面？**

用户可以直接从Workfront启动Frame.io查看器。 所有审阅和批准活动均在Frame.io查看器中进行，并自动同步回Workfront。

**我能否将批准的资源发送到Adobe Experience Manager (AEM)？**

可以。资产完成审阅和批准周期后，您可以将其转移到Adobe Experience Manager Assets进行最终存储和分发。 这会将Workfront工作管理、Frame.io审查和AEM数字资产管理连接到一个统一的内容supply chain。

有关详细信息，请参阅。有关详细信息，请参阅[将Adobe Experience Manager与Frame.io集成一起使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

**统一审阅和批准如何适应Adobe GenStudio？**

统一审查和批准是Adobe GenStudio的基本组件 — Adobe对连接内容supply chain的更广泛愿景。 GenStudio将Workfront、Frame.io、Creative Cloud、Adobe Express、Adobe Experience Manager Assets和GenStudio for Performance Marketing连接到一个统一的工作流（从营销活动简报到内容交付）。

在该生态系统内，审查和批准是创建和执行之间的关键交接点。 在这里，创意工作会满足利益相关者的投入，质量会得到验证，内容会获得批准以供发布。 如果切换快速、可见且可靠，它会解锁整个supply chain内容的速度 — 人工智能可以加快创建，自动化可以处理分发，但审核的瓶颈限制了双方的优势。 连接Workfront和Frame.io可消除该瓶颈。

**什么是AI Reviewer功能？**

统一审查和批准包括AI审核者功能，可在审核过程中自动进行品牌合规性检查。 AI审阅者可以根据品牌准则评估资产，并在参与人工审阅者之前标记潜在问题，帮助团队更早发现问题并更快地行动。

有关设置和使用AI查看器的更多信息，请参阅Experience League上的Workfront文档。

+++

### 合同、 SKU和存储

+++ 展开以查看有关合同、SKU和存储方面的常见问题。

**我何时可以使用统一审阅和批准？**

统一审查和批准功能现已可用。 访问需要升级到Workfront V2 SKU。 如果您的合同是在V2 SKU可用之前签署的，则可以通过以下两种方式之一获得访问权限：

* 续订后：将在您下次合同续订日期启用访问。

* 提前重新合同：您的Adobe客户团队可以提前重新合同，在保留现有合同结束日期的同时添加新的SKU权利。 转向同等套餐时，价格不会上涨。

请联系您的Adobe客户代表以确定适合您组织的最佳路径。

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**升级到V2 SKU是否为我提供了更多存储空间？**

可以。使用V2 SKU，每个获得许可的用户可接收60 GB的存储，而上一版本中为30 GB。

**如何在Adobe企业级存储与旧版Workfront存储之间进行选择？**

企业存储启用Frame.io查看器体验，需要统一审查和批准。 旧版存储仍会使用Workfront Proof查看器(ProofHQ)作为默认值。

如果您的组织包含简单的工作流和更加复杂的验证工作流，则可以优先迁移哪些工作流。

企业存储让您能够灵活地以增量方式推出新体验，从最有益的工作流开始。

**如何管理Frame.io许可证？**

签署V2 SKU后，所有Workfront用户都将有权访问Frame.io查看器以查看和批准工作流 — 此操作不需要单独的Frame.io Enterprise许可证。

如果您的组织需要其他Frame.io Enterprise功能，例如

* 高级水印（动态和取证）
* 具有自动资产删除功能的数字版权管理
* AI生成内容的内容凭据
* 自定义创意元数据
* Camera与云的集成
* 您自己的创意工作进行中工作区

您可以与Adobe客户团队合作，确定适当的Frame.io Enterprise许可证数量。 所有许可证都通过Adobe Admin Console进行管理。

+++

### 沙盒和转出

+++ 展开以查看沙盒和转出的常见问题解答。

**我是否可以在沙盒环境中测试统一审阅和批准？**

部分。 可以在Workfront沙盒环境中测试审批工作流。 但是，Frame.io查看器体验在沙盒中不可用。 测试审阅表面本身需要生产环境。

要限制转出过程中的风险，您可以在Workfront生产环境中为特定组启用统一审查和批准。 这样，您就可以在更广泛地推出之前，通过一组更少的用户来运行定向试点。

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### 交互式验证和HTML

+++ 展开以查看交互式验证和HTML的常见问题解答。

**统一审阅和批准是否支持交互式验证或HTML URL？**

当前支持Zip HTML文件进行交互式审阅。 HTML URL支持（实时Web URL审查）位于路线图上，预计将在第三季度提供。

有关更新，请查看Experience League上的Workfront发行说明。

+++

### 融合与自动化

+++ 展开以查看Fusion和自动化的常见问题解答。

**我是否需要Workfront Fusion才能使用统一的审阅和批准？**

不可以。统一审查和批准是本机产品集成，不需要Fusion。 工作流直接内置到Workfront中。

**Fusion Connectors是否可以进行统一审核和批准？**

可以。用于统一审阅和批准的融合操作目前正在开发中，预计将在第三季度提供。 查看Experience League上的Workfront发行说明，了解更新何时可用。

**Fusion能否在上传文档时自动触发审阅？**

可以。通过将Workfront Webhook与Fusion结合使用，可以实现这种类型的自动化。

**在Workfront Proof上构建的现有Fusion工作流将受到什么影响？**

根据每个工作流的构建方式，影响会有所不同。 一般而言：

* **编辑或更新**：可以更新现有验证相关操作在统一审批中具有直接等效操作的工作流以使用新操作。

* **重新生成**：基础步骤已发生重大更改或存在新功能的工作流，可能需要从头开始重新生成。

一旦用于统一审批的Fusion API可用，将呈现更清晰的图像。 建议审核您现有的Fusion工作流，并根据当时新的统一审批功能评估它们。

+++






