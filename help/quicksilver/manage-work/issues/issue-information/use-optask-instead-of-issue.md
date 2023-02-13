---
product-area: projects
navigation-topic: issue-information
title: 引用问题时，请使用“opTask”和“issue”
description: 问题的名称在Adobe Workfront数据库中显示为opTask。 尽管有时您需要使用问题字段名称来引用问题，但大多数情况下，在引用问题时，您必须使用opTask字段名称，而不是问题。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# 引用问题时，请使用“opTask”和“issue”

问题的名称显示为 `opTask` 在Adobe Workfront数据库中。 尽管有时您需要使用 `issue` 字段名称引用问题，大多数情况下您必须使用 `opTask` 字段名称，而不是 `issue` 引用问题时。

有关对象在Workfront数据库中的显示方式的详细信息，请参阅 [API Explorer](https://one.workfront.com/s/api-explorer).

## `opTask` 文件名

使用 `opTask` 在以下上下文中引用问题时的字段名称：

* 在创建文本模式的问题自定义报告时，您想引用视图、过滤器、分组或提示中的问题。

   有关在报表中使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* 在Kick-Start数据导入器工作表中更新问题字段时。

   有关使用Kick-Start在Workfront中导入数据的更多信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` 字段名称

使用 `issue` 用于引用以下上下文中问题的字段名称：

* 在报表中使用文本模式引用收藏集中的问题时。
* 使用Workfront API引用问题集合时。

有关报告收藏集的信息，请参阅 [在报表中引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://one.workfront.com/s/api-explorer" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
