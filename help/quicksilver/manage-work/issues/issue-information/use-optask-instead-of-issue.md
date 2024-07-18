---
product-area: projects
navigation-topic: issue-information
title: 在引用问题时使用“opTask”和“issue”
description: 问题的名称在Adobe Workfront数据库中显示为opTask。 尽管有时需要使用问题字段名称来引用问题，但大多数情况下，在引用问题时您必须使用opTask字段名称而不是issue。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 在引用问题时使用“opTask”和“issue”

问题的名称在Adobe Workfront数据库中显示为`opTask`。 尽管有时您需要使用`issue`字段名称来引用问题，但在大多数情况下，在引用问题时您必须使用`opTask`字段名称而不是`issue`。

有关对象如何在Workfront数据库中出现的详细信息，请参阅[API资源管理器](https://developer.adobe.com/workfront/api-explorer/)。

## `opTask`文件名

引用以下上下文中的问题时使用`opTask`字段名称：

* 在创建问题的文本模式自定义报告时，并且希望在视图、筛选器、分组或提示中引用问题。

  有关在报表中使用文本模式的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

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
