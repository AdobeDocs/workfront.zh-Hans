---
product-area: documents
navigation-topic: approvals
title: Workfront AI Reviewer入门
description: 使用Workfront AI审阅者在审阅和批准工作流程期间根据品牌准则评估内容。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 2%
---
# Workfront AI Reviewer入门

AI查看者是一个AI协作者，它是一种AI代理，可添加到您的项目、任务和文档中。 AI协作者可以在设置区域中配置，并像用户一样进行分配。

在Workfront中，AI Reviewer有助于在整个审阅和批准过程中提高内容速度并改善品牌合规性。 您可以将AI审阅人添加到批准模板，或将其包含在单个审阅和批准请求中。

## 访问权限要求

要在Workfront中设置AI审阅者，您必须是系统管理员。

任何用户都可以将AI审阅者添加到审阅和批准请求。

## 要求

* 您的Workfront实例必须启用统一批准。
* 您的组织必须具有GenStudio Foundation。
  * Workfront中的AI审阅者提供了GenStudio Foundation中用于资源审阅和批准工作流的功能。 您无需直接访问GenStudio Foundation即可完成工作。 您通过AI查看器访问GenStudio Foundation功能是受Workfront合同条款约束的。
* Adobe必须有一个已签署的Adobe Gen AI协议文件。
有关签署协议的更多信息，请参阅[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* AI查看器在沙盒环境中不可用。


## 支持的文件类型 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="不支持的文件类型"
>abstract="此 AI 审阅者不支持所选的文件类型。 上载支持的文件类型，或删除AI审阅者以提交请求。"

AI审阅者可审阅以下文件类型：

* PNG (.png)
* JPEG (.jpeg， .jpg)
* WEBP (.webp)
* 非动画GIF (.gif)
* PDF (.pdf)
* PPT (.ppt， .pptx)
* DOC (.doc， .docx)

如果您上传的文件类型不受支持，则在创建审批工作流时，AI查看器选项将不可用。

## 设置品牌指南

Workfront AI审核者在审核内容时使用品牌准则。 Workfront管理员可以在Workfront设置区域中设置品牌指南。 在GenStudio Foundation中创建的品牌也可以在Workfront中使用。

要设置品牌指南，系统管理员必须：

1. [授予对品牌权限的访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [创建和管理AI审阅者的品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。


## 创建AI审阅者

至少设置了一个品牌后，Workfront管理员便可以在“设置”区域开始创建AI审阅者。 您可以创建多个侧重于不同准则的AI审阅者：

* **图像**：此AI审阅人将依据您在Workfront中设置的图像品牌指南审阅资产。 [!BADGE Beta 版]{type=Positive tooltip="此功能当前处于测试阶段。"}
  * 系统管理员必须签署测试版协议才能启用此功能。
* **品牌声音**： AI审阅人将依据您在Workfront中设置的品牌声音准则审阅资产。

随后，可以将AI审阅人分配给审批模板以及单个审阅和审批请求。

有关详细信息，请参阅[配置AI协作者](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## AI审阅者评估的内容 {#what-ai-reviewer-evaluates}

AI审阅者根据以下准则类型对内容进行不同的评估：图像或品牌声音。

### 图像

AI审阅者会评估：

* **合成**：焦点、背景、裁剪、创意框架
* **灯光和情绪**：使用光线、活力、乐观主义
* **多样性和包容性**：人员的代表性（种族、性别、年龄、能力）

AI审阅者不评估：

* **徽标用法**：位置、空间、大小、正确的徽标版本
* **调色板**：符合品牌颜色要求，避免未经批准的颜色
* **排版规则**：字体系列、粗细、间距、对齐方式
* **插图样式**：与品牌的插图方法一致
* **辅助功能**：对比度符合性、清晰度

### 品牌声音

AI审阅者会评估：

* **语调**：对话、清晰、人性，与品牌个性一致
* **行话/形式**：避免使用流行语、精英主义或过度形式
* **消息**：鼓励、诚实、负责任的定位（例如，AI主题）

AI审阅者不评估：

* **法律/合规性**：商标使用、免责声明、本地化规则

有关编写与AI审阅者评估的内容一致的品牌准则的指导，请参阅[为AI审阅者创建和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。

## 添加AI审阅人审阅和批准请求

用户可以将AI审阅人添加到现有审批模板或单个审阅和审批请求。

### 审批模板

如果贵组织经常添加相同人员来审阅和审批请求，则Standard许可证用户可以在Workfront设置区域创建审批模板。

用户可将AI审阅人添加到批准模板，以在使用模板创建请求时自动检查品牌合规性。

创建后，审批模板可应用于项目、任务或问题的文档区域中的资产。

有关详细信息，请参阅[为文档创建审批工作流模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。

显示AI审阅者的![模板列表](assets/ai-review-templates.png)

### 单个审阅和批准请求

当用户创建单个审阅和批准请求时，他们可以与其他参与者一起添加AI审阅人，也可以仅使用AI审阅人创建单个请求以检查品牌合规性。

有关详细信息，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。


![AI审阅者已添加到单个审批请求](assets/new-stage.png)

## 查看AI审核者得分和反馈

在提交具有AI审阅人的审阅和批准请求后的几秒内，来自AI审阅人的得分和反馈将显示在“文档摘要”面板中 — 即使其他参与者仍在审阅和做出决策。

审批所有者还会收到一封电子邮件，通知他们已对该资产完成审核。 在电子邮件中，单击&#x200B;**前往**&#x200B;查看Workfront中的分数和反馈。

AI审阅者并非旨在成为审阅和批准工作流中的决策者。 它仅提供分数和建议，以将资产与指定的品牌要求保持一致。

如果资产不符合品牌指南，创意人员可以上传新版本，审批所有者可以使用AI审阅者创建第二个审阅和审批请求。

有关查看分数和反馈的详细信息，请参阅[查看AI审阅者分数和反馈](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)。

