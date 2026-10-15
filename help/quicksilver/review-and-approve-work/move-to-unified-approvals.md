---
product-area: documents
navigation-topic: approvals
title: 从旧文档审批移至统一审批
description: 了解当您的组织迁移到支持统一审批的Workfront版本时，现有文档审批工作流会发生什么情况。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 1%
---
# 从旧文档审批移至统一审批

默认情况下，Adobe云存储项目使用统一批准。 本文介绍了与旧文档审批相比，统一审批中可用的功能。


>[!NOTE]
>
>只有在Adobe云存储中创建的新对象，才会默认使用统一审批。 旧版Workfront存储对象保留其当前的批准服务。<br>
>有关详细信息，请参阅[在Adobe云存储上移动到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

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

在旧版文档审批中创建的投放中审批继续像之前一样运行。 Adobe云存储对象的新批准使用统一批准。 对旧版Workfront存储对象的新审批保留这些对象已使用的审批服务。


## 准备迁移

* 与最终用户共享[统一审核和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章。
* 查看现有Workfront Fusion场景。 如果您使用带有校对的旧文档审批，在将团队引入Workfront云存储之前，请参阅[更新Adobe Fusion方案以进行统一审阅和审批](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。
* 在画布功能板中设置审阅和批准功能板以替换任何旧版批准报表。 有关详细信息，请参阅[创建审核和批准仪表板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。


### 面向最终用户的帮助文章

* [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [用于文档审批的可用功能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [统一审查和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [使用Frame.io查看器审阅和批准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [将统一审批和验证结合使用](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [文档决策状态概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Workfront内容审查者入门](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
