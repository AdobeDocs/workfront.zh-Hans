---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 规划Adobe云存储转出
description: 选择Adobe Cloud Storage如何向您的用户显示，在单个组中进行试点，并对工作进行排序，以使审阅人、批准者和项目所有者不会感到意外。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# 规划Adobe云存储转出

由您决定Adobe云存储访问您的用户的方式和时间。 在Workfront管理员在设置区域中将Adobe云存储设置为默认存储选项之前，不会发生任何更改，这样您就有时间测试体验并在任何人都可以使用该体验之前准备您的团队。

本文介绍您可以选择哪些转出配置、如何与单个组一起试运行，以及建议的工作顺序。

## 选择Adobe云存储的推出方式

有两种配置，您可以将一种配置应用于整个组织或特定的Workfront组。 默认情况下，在Adobe云存储上创建的每个项目都使用统一审批和Frame.io查看器。

有关分步说明，请参阅[为您的组织启用Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

### 配置选项

* **仅限Adobe云存储**：默认情况下，新项目使用Adobe云存储。 用户无法创建旧版项目。
* **Adobe云存储和旧版Workfront存储**：用户创建项目时，他们会在Adobe云存储（标记为“新项目”）和旧版Workfront存储（标记为“旧版存储”）之间进行选择。 通过选中“设置”区域中的&#x200B;**允许用户选择存储提供程序**&#x200B;复选框，可启用此选项。

>[!TIP]
>
>要先将Adobe云存储放在较小的团队之前，请将任一配置应用于单个Workfront组。 这允许您在更广泛地推广之前运行定向试点。 我们建议从组级别推出开始，以实现受控步调，然后在试点小组验证体验后，扩展到整个组织。

现有对象会保留创建它们的存储模型。 更改默认存储首选项不会更改任何现有对象。

安装程序中的![存储首选项](assets/storage-preference-groups.png)

## 规划您的转出

每个Workfront环境都不一样。 在将Adobe云存储设置为用户的默认存储之前，请花些时间规划一下对于您的组织来说转出是怎样的一个成功案例。 下面的建议不是准确的清单，而是您自己的计划的起点。

### 选择试点小组

通过按组划分范围的转出，您可以先将Adobe云存储放在较小的团队之前、收集反馈并进行调整，然后再进行更广泛的转出。 选择一个其工作模式具有足够代表性的组，以便及早发现您想要了解的问题。

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### 上线前测试

Adobe云存储在Workfront沙盒环境中可用，因此您可以在生产之前验证大部分体验。 Frame.io查看器在Sandbox中不可用，因此您可以与试点小组一起验证生产过程中的完整审阅和批准体验。 有关详细信息，请参阅[为您的组织启用Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

### 将更改传达给最终用户

对于审阅人、审批人和项目所有者而言，最大的可见更改是新增的文档区域和Frame.io查看器，它们支持Adobe云存储项目的审阅和审批。 规划您将如何引入这些存储产品，以便用户了解在遇到他们的第一个Adobe云存储项目时会有什么样的体验。 [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章是面向最终用户的材料的有用起点。

### 查看您的权限和治理

在Adobe云存储项目中，“管理”和“贡献”映射到Frame.io中的“编辑和共享”，其中包括外部共享。 在将团队引入Adobe云存储之前，请查看共享模式并确定它是否符合您的治理模式。 有关详细信息，请参阅[Adobe云存储的不同之处](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping)。

### 审核模板和命名

Adobe云存储强制实施严格的命名规则，并且Workfront会自动重命名与其冲突的对象。 如果从模板创建项目，请查看这些模板，使其生成的名称和结构符合规则。 有关详细信息，请参阅[Adobe云存储的不同之处](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules)。

### 围绕Workfront Fusion规划

现有的基于验证的Fusion方案将继续用于旧版项目，但不会自动用于Adobe云存储项目。 在将依赖这些方案的团队引入Adobe云存储之前，请将每个方案分类为“编辑”、“重建”或“弃用”。 有关详细信息，请参阅[更新Workfront Fusion方案以进行统一审查和批准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。

### 计划报告更改

统一的审批工作流数据和报告会显示在画布功能板中。 旧版审批报告不会自动延续，因此在您的试点团队需要它之前设置一个替换仪表板。 有关详细信息，请参阅[创建报告仪表板以供审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。

## 建议的序列

使用此顺序作为模板，根据您的环境调整它：

1. 在沙盒中测试该体验，并在生产中测试该体验。
2. 分类和更新Fusion场景，并构建画布功能板报表。
3. 审核您的模板并查看您的权限和共享模型。
4. 将更改传达给将使用该更改的审阅者、批准者和项目所有者。
5. 将Adobe云存储设置为试点组的默认值，然后在试点组验证体验后，扩展到更多组或整个组织。
