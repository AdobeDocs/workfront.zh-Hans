---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: 融合
navigation-topic: fusion-release-activity
title: 'Workfront Fusion发布活动：2020年11月30日当周'
description: 本页介绍了2020年11月30日这一周在Adobe Workfront Fusion中所做的所有增强。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Workfront Fusion发布活动： 2020年11月30日开始的周

本页介绍了2020年11月30日这一周在Adobe Workfront Fusion中所做的所有增强。

有关所有最近更改的列表，请参阅[Adobe Workfront Fusion发行活动](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)。

有关Workfront Fusion中最近的错误修复列表，请参阅[Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)页面，并检查任何标记为Workfront Fusion维护更新的更新。

## Workfront Fusion 2.0 Webhook的速率限制。

我们为Workfront Fusion 2.0引入了新的性能护栏。现在，webhook具有每秒100个请求的速率限制。 达到此限制后，Workfront Fusion 2.0会发送429（请求过多）状态。

以前，webhook请求不受限制。

有关详细信息，请参阅[Adobe Workfront Fusion性能护栏](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md)。

## 在Workfront Fusion 2.0中将自定义表单添加到Workfront对象

为了使您能够将自定义表单添加到Workfront Fusion 2.0中的对象，我们已在Workfront >杂项中添加了AssignCategories操作。 操作模块。

以前，无法使用Workfront Fusion 2.0模块将自定义表单添加到Workfront中的对象。

有关Workfront >其他内容的更多信息。 操作模块，请参阅[Adobe Workfront模块](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
