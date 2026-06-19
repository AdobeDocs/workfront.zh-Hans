---
product-area: documents
navigation-topic: approvals
title: 更新Workfront Fusion方案以进行统一审查和批准
description: 在您的组织采用Workfront云存储并统一审查和批准时，清点、分类和修复基于旧版Workfront Proofing构建的Adobe Fusion场景。
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 更新Workfront Fusion方案以进行统一审查和批准

基于旧版Workfront Proofing构建的Workfront Fusion方案不会自动针对Adobe云存储项目运行。 验证特定的模块、Webhook和API端点在某些情况下具有直接等效功能，而在其他情况下具有显着变化。 在将依赖这些方案的团队引入Adobe云存储推出之前，本文可帮助您清点受影响的方案、对它们进行分类并决定补救路径。

范围覆盖到旧版Workfront项目的方案将继续像现在一样工作。 本文中描述的修正工作适用于您打算针对Adobe云存储项目运行的场景。

>[!IMPORTANT]
>
>Adobe Workfront Unified Review and Approvals连接器现已在Workfront Fusion中可用。 在将Fusion与Adobe云存储结合使用时，我们建议使用此连接器以获得更简单、更可靠的方案。
>
>有关信息和说明，请参阅Workfront Fusion文档中的[Adobe Workfront统一审阅和审批模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules)。

使用本文清点场景并对场景进行分类，了解升级Fusion场景以考虑Adobe云存储的最佳方法。

有关您的组织在Adobe云存储上移动到Workfront时所做更改的高级摘要，请参阅[在Adobe云存储上移动到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。


## Fusion在Adobe云存储项目中的哪些变化

基于Workfront Proof构建的现有Fusion场景依赖于验证特定的模块、webhook触发器和不属于统一审查和审批数据模型的API端点。 下表将常见方案类型映射到其预期影响和前进的路径：

| 方案类型 | 影响 | 前进路径 |
|---|---|---|
| 校对创建和路由 | 断点 | 在2026年第3季度使用统一批准API重建 |
| 验证状态Webhook | 断点 | 在2026年第3季度触发新的批准事件以进行重建 |
| 文档上传触发器 | 部分：需要重新测试 | 在2026年第三季度迁移后进行审核和重新测试 |
| 审批提醒通知 | 断点 | 替换为审批模板截止日期 |
| 批准决策路由 | 断点 | 使用新的决策状态字段重新生成 |
| 自定义审批报告 | 部分：字段名称可能会更改 | 将旧版字段映射到新架构 |


## 将每个方案分类为“编辑”、“重建”或“停用”

每个方案所需的工作取决于其功能以及统一审查和批准中可用的内容。 使用以下分类：

* **编辑**：现有的验证相关操作在统一审阅和批准中具有直接等效操作，您可以更新方案以使用新操作。
* **重新生成**：基础步骤已发生显着变化，或者存在方案应使用的新功能，因此需要从头开始重新生成方案。
* **弃用**：本机统一审阅和审批功能（如带有截止日期提醒的多阶段审批模板）取代了生成方案的功能。

根据特定业务逻辑查看每个场景以确定其分类。

## 补救方法

请使用以下方法规划和执行Fusion修正：

1. **立即清点。** 提取活动Fusion场景的完整列表，并标记每个引用验证创建、验证状态、文档审批或审批路由的场景。 启用Adobe云存储后，请勿再等待。
1. **根据上一节中的条件将每个方案**&#x200B;分类为“编辑”、“重新生成”或“停用”。
1. **在将依赖校对的团队引入Adobe云存储试点之前，请暂停依赖校对的场景**。 对新模型运行过时的基于验证的自动化可能会产生静默故障或重复操作。
1. **使用审批模板替换简单路由逻辑。** 具有截止日期自动化的本机多阶段审批模板可以处理以前需要Fusion的许多用例。 有关详细信息，请参阅[为资源和文档创建批准模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。
1. **重建时使用Adobe Workfront统一审阅和批准连接器。** 更新的连接器公开了专门为统一审查和审批构建的模块，并使重建显着简化且更加可靠。 我们不建议预先针对Workfront API版本22进行重建。
1. **在生产环境中启用之前，在沙盒实例**&#x200B;中端到端地测试重新构建方案。 请特别注意事件订阅负载 — 字段名称和架构与旧版验证事件不同。

>[!TIP]
>
>许多组织积累了Fusion场景，这些场景是解决旧版验证中差距的解决方法。 本机统一审阅和批准功能（包括批准模板、截止日期提醒和多阶段路由）完全消除了对其中一些方案的需要。 在对每个场景进行分类时，请评估本机功能是否可以替换它。 退出情景往往比重建情景更清洁的长期结果。

## 相关文章

* [在Adobe云存储上迁移到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [统一审查和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [创建资产和文档的审批模板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
