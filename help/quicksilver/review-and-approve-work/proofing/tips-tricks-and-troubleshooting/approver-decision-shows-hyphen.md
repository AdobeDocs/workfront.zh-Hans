---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 审批者决策在验证审批报告中显示连字符
description: 验证审批报告的审批者决策字段中的连字符表示收件人不再处于验证的决策角色。
author: Courtney
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 73c78912e15a03bfd09c127e39d94bf5af42b8e2
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# 审批者决策在验证审批报告中显示连字符

## 问题

在验证审批报告中，收件人的“审批者决策”字段显示连字符(-)，即使“决策日期”字段显示日期且等待决策为False。

![审批者决策在验证审批报告中显示连字符](assets/approver-decision-hyphen.png)

## 原因

审批者决策字段中的连字符意味着收件人不再处于验证上的决策角色。 出现以下情况时，可能会发生这种情况：

* 收件人已添加到验证并作出了决定，随后又从工作流中删除。 如果收件人修改了验证，则验证系统将访问记录为决策更改。 由于收件人不再是批准者，因此系统会将新决策记录为连字符。
* 收件人的验证角色已更改为不包含审批权限的验证角色，例如查看者。 有关每个角色可以对验证执行的操作的信息，请参阅[验证角色概述](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md)。
* 收件人的验证权限配置文件在做出决定后被降级。

## 在报表中这意味着什么

连字符是有意为之。 它可告知您，系统没有等待收件人审批验证，并且收件人不再拥有验证的决策角色。

决策日期字段仍显示收件人最近决策活动的日期，但收件人的决策不再计入报告中。

有关创建和使用验证审批报告的信息，请参阅[使用验证审批报告](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md)。




