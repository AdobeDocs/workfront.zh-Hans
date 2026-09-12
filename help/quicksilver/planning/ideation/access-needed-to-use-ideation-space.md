---
title: 使用构思空间所需的访问权限
description: Adobe Workfront Planning现在提供了一项可在启动营销活动之前进行构思的额外功能。 利用AI的强大功能将数据及直接输入转换为实际的计划，并为团队提供一个有根据的起点，而不是带Adobe Ideation空间的空白页。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---


# 使用构思空间所需的访问权限

<span class="preview">此页面上的信息引用了尚未公开的功能。 它只能作为&#x200B;**构思空间Beta**&#x200B;程序的一部分提供。</span>

<span class="preview">有关详细信息，请参阅[Adobe Workfront规划构思空间入门](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>


{{planning-important-intro}}

Adobe Workfront Planning现在提供了一项可在启动营销活动之前进行构思的额外功能。 利用AI的强大功能将数据及直接输入转换为实际的计划，并为团队提供一个有根据的起点，而不是带Adobe Ideation空间的空白页。

本文介绍了要从Workfront Planning访问构思空间必须具有的访问权限和权限。

有关构思空间的一般信息，请参阅[Adobe Workfront规划构思空间入门](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。

## 产品要求

构思空间不是独立的产品。 它需要Workfront Planning程序包，并且只能从Workfront Planning访问。 它还需要其他产品。

贵组织必须购买以下产品的产品包才能访问创意空间：

* Adobe Workfront工作流包以及计划包

  或

  作为独立产品购买的Adobe Workfront Planning。
* Adobe GenStudio for Performance Marketing许可证

  >[!TIP]
  >
  >需要GenStudio for Performance Marketing才能访问正确的字体授权。


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planning访问级别要求

在Workfront中配置创意空间访问。

要访问构思空间，您的Workfront访问级别必须包括以下内容：

* 标准工作流许可证，贵公司在该许可证中购买的除Planning包之外的Workflow包。
* Standard Planning许可证（当您的公司与Workflow和Planning包一起购买时），或Workfront Planning作为独立产品购买时。
* 必须取消选择访问级别的“设置其他限制”部分中的“禁用构思空间”设置。<!--***********check the UI for this***********-->

## Workfront Planning权限要求

每条Planning记录都与Ideation space中的一个摘要相连。

构思空间摘要权限继承自Workfront Planning记录权限。<!--not sure if this is right, because now you can share the ideation with others??-->

您必须对Planning中的记录类型具有“管理”权限才能创建记录，以便在创意空间中创建或编辑记录。

对记录具有“查看”权限的Planning用户可以查看记录的构思空间。

下表显示了Workfront Planning记录权限与构思空间简介权限之间的关系：

| 规划记录级别权限 | 构思空间简要级别权限 |
|---|---|
| 管理记录的权限 | 可以在记录的构思空间中创建摘要 |
| 查看记录的权限 | 可以在构思空间中读取该记录的摘要，但不能对其进行修改 |

## 构思空间权限

<!--this is also duplicated in the intro of the Share an ideation space article-->

计划权限将转移到记录的构思空间。

此外，您还可以向其他用户授予使用构思空间的权限并向其添加构思。

请考虑以下事项：

* 构思创建者始终对其自己的构思具有编辑者权限。

* 您必须对构思空间具有编辑器权限，才能创建摘要并将其导出到其他应用程序。

以下是创意空间权限及其提供的功能：

| 构思空间权限 | 功能 |
|---|---|
| 编辑者 | 可以编辑、下载和共享创意空间 |
| 评论者 | 可以查看和评论构思空间 |
| 查看者 | 可以查看构思空间 |

有关共享构思空间的更多信息，请参阅[共享构思空间](/help/quicksilver/planning/ideation/share-the-ideation-space.md)。

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
