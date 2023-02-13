---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 使用Adobe Workfront API跟踪小时记录
description: 如果贵组织使用Adobe Workfront输入工作小时数，但使用其他工具作为该数据的记录系统，则可以使用Workfront API在两个系统之间同步数据。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 使用Adobe Workfront API跟踪小时记录

如果贵组织使用Adobe Workfront输入工作小时数，但使用其他工具作为该数据的记录系统，则可以使用Workfront API在两个系统之间同步数据。

仅跟踪小时记录不可行，因为如果删除了小时条目，则会删除整个记录，这要求您提取整个数据集并将其与旧数据集进行比较。 幸运的是，所有小时事务处理都记录在Workfront日记帐分录中。

在检索系统中所有当前小时的初始集后，您可以通过“日记帐分录”跟踪任何和所有更改。
<pre>GET/attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType，aux2,newNumberVal，oldNumberVal，subObjCode，subObjID</pre><pre>{<br>"data":[<br>{<br>"ID":"5785406d008d93dd35665f14d90d4929",<br>"objCode":"JRNLE",<br>"changeType":"A",<br>"aux2":“布拉德·利特勒”<br>"newNumberVal":1,<br>"oldNumberVal":null，<br>"subObjCode":“小时”，<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"57854124008da2b9f372c01f8b9054bf",<br>"objCode":"JRNLE",<br>"changeType":"D",<br>"aux2":“布拉德·利特勒”<br>"newNumberVal":null，<br>"oldNumberVal":1,<br>"subObjCode":“小时”，<br>"subObjID":"5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID":"5785416f008db05ecee934663a968366",<br>"objCode":"JRNLE",<br>"changeType":"A",<br>"aux2":“布拉德·利特勒”<br>"newNumberVal":1,<br>"oldNumberVal":null，<br>"subObjCode":“小时”，<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID":"57854176008db22fe974b7c67feea6b2",<br>"objCode":"JRNLE",<br>"changeType":"E",<br>"aux2":“布拉德·利特勒”<br>"newNumberVal":2,<br>"oldNumberVal":1,<br>"subObjCode":“小时”，<br>"subObjID":"5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>以下是所包含字段的描述：

* **changeType:** 对对象所做更改的类型：

   * **答：** 添加

   * **E:** 编辑

   * **D:** 删除

* **aux2:** 小时记录所针对的用户的名称。

* **newNumberVal:** 小时记录的新值（如果changeType为D，则此值将为null）。

* **oldNumberVal:** 小时记录的上一个值。

* **subObjCode:** 要修改的记录类型（应始终为HOUR）。

* **subObjID:** 小时记录的ID。

您可以使用此信息来发现哪些小时记录已更改、编辑或删除。 然后，您可以使用subObjID在必要时从小时记录中检索更多信息。
