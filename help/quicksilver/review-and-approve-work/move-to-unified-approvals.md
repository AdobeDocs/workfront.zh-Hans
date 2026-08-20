---
product-area: documents
navigation-topic: approvals
title: 从旧文档审批移至统一审批
description: 了解当您的组织迁移到支持统一审批的Workfront版本时，现有文档审批工作流会发生什么情况。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 8f3c5ed32c6496a13703a5dce771a84462aa7f05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# 从旧文档审批移至统一审批

迁移到支持Adobe Cloud Storage的Workfront版本还会将您的组织从旧版文档审批转移到统一审批。 本文提供了有关统一审批中可用的功能的信息，以及面向Workfront管理员的建议，即将用户从旧版文档审批中移出。


>[!IMPORTANT]
>
>当您迁移到支持Adobe云存储的Workfront版本时，这项更改会立即在组织范围内适用。 从传统文档审批过渡到统一审批时，没有试点组或逐步推出选项。<br>
>有关对Adobe云存储进行哪些更改的详细信息，请参阅[在Adobe云存储上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 了解从旧版文档审批到统一审批有何变化

|  | 旧文档审批 | 统一审批 |
| --- | --- | --- |
| 审批者和审阅者 | 仅由个人用户批准 | 单个用户或团队的批准或审阅 |
| 截止日期和提醒 | 无自动提醒 | 72小时、24小时以及截止日期的自动提醒 |
| 审批阶段和路径 | 一个审批阶段，无并行路径 | [多个审批阶段和并行审阅路径](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| 审批模板 | 每个审批都是从头开始配置的 | 在Workfront设置中提供了[可重用模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) |
| 审阅和标记 | 校对查看器 | 旧版Workfront存储对象上的[验证查看器](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)，或Adobe云存储对象上的[Frame.io查看器](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) |
| AI辅助审查 | 不可用 | 通过[内容审阅者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)自动进行品牌符合性检查 |
| 报告 | 旧版报表 | 主KPI小组件和[画布功能板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### 对已在进行中的审批有何影响

在旧版文档审批中创建的投放中审批将继续正常运行，就像升级之前一样。 但是，升级后创建的所有新批准都将使用统一批准。


## 准备升级

* 与最终用户共享[统一审核和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章。
* 查看现有Workfront Fusion场景。 如果将旧文档审批与验证一起使用，请在组织升级之前参阅[更新Workfront Fusion方案以进行统一审查和批准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。
* 在画布功能板中设置审阅和批准功能板以替换任何旧版批准报表。 有关详细信息，请参阅[创建审核和批准仪表板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。


### 面向最终用户的帮助文章

* [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [用于文档审批的可用功能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [统一审查和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [使用Frame.io查看器审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [将统一审批和验证结合使用](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [文档决策状态概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Workfront内容审查者入门](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)