---
product-area: projects
navigation-topic: issue-information
title: 引用问题时使用“opTask”和“issue”
description: 问题的名称在Adobe Workfront数据库中显示为opTask。 尽管有时需要使用问题字段名称来引用问题，但大多数情况下，在引用问题时您必须使用opTask字段名称而不是issue。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 1%

---

# 在引用问题时使用“opTask”和“issue”

<!--Audited: 08/2025-->

问题的名称在Adobe Workfront数据库中显示为`opTask`。 尽管有时您需要使用`issue`字段名称来引用问题，但在大多数情况下，在引用问题时您必须使用`opTask`字段名称而不是`issue`。

有关对象如何在Workfront数据库中出现的详细信息，请参阅[API资源管理器](https://developer.adobe.com/workfront/api-explorer/)。

## `opTask`字段名称

引用以下上下文中的问题时使用`opTask`字段名称：

* 在创建问题的文本模式自定义报告时，并且希望在视图、筛选器、分组或提示中引用问题。

  有关在报表中使用文本模式的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

* 当您更新快速启动数据导入器工作表中的问题字段时。

  有关使用Kick-Start在Workfront中导入数据的详细信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

## `issue`字段名称

使用`issue`字段名称引用以下上下文中的问题：

* 当您在报告中使用文本模式引用收藏集中的问题时。
* 当您使用Workfront API引用问题集合时。

有关集合报表的信息，请参阅[报表中的引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
