---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 使用Adobe Workfront API跟踪小时记录
description: 如果贵组织使用Adobe Workfront输入工作时数，但使用其他工具作为该数据的记录系统，则可以使用Workfront API在两种系统之间同步数据。
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 使用Adobe Workfront API跟踪小时记录

如果贵组织使用Adobe Workfront输入工作时数，但使用其他工具作为该数据的记录系统，则可以使用Workfront API在两种系统之间同步数据。

仅跟踪小时记录并不可行，因为如果删除小时条目，将删除整个记录，这要求您拉取整个数据集并将其与旧数据集进行比较。 幸运的是，所有小时交易记录都记录在Workfront日记帐分录中。

在检索系统中所有当前小时数的初始集后，您可以通过日志条目跟踪任何和所有更改。
<pre>GET/attask/api/v5.0/JRNLE/search？subObjCode=HOUR&amp;fields=changeType，aux2，newNumberVal，oldNumberVal，subObjCode，subObjID</pre><pre>{<br>"data"： [<br>{<br>"ID"： "5785406d008d93dd35665f14d90d4929"，<br>"objCode"： "JRNLE"，<br>"changeType"： "A"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 1，<br>"oldNumberVal"： null，<br>"subObjCode" "HOUR"，<br>"subObjID"： "5785406d008d93dce3f7f2e0e8eda4ea"<br>}，<br>{<br>"ID"： "57854124008da2b9f372c01f8b9054bf"，<br>"objCode"： "JRNLE"，<br>"changeType"： "D"，<br>"aux2"： brad Littler”，<br>"newNumberVal"： null，<br>"oldNumberVal"： 1，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785406d008d93dce3f7f2e0e8eda4ea"<br>}，<br>{<br>"ID"： "5785416f08db05ecee934663968366"，<br>"objCode"： "JRNLE"，<br>"changeType"： "A"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 1，<br>"oldNumberVal"： null，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785416f008db05d9d2925c 112b10f521"<br>}，<br>{<br>"ID"： "57854176008db22fe974b7c67feea6b2"，<br>"objCode"： "JRNLE"，<br>"changeType"： "E"，<br>"aux2"： "Brad Littler"，<br>"newNumberVal"： 2，<br>"oldNumberVal"： 1，<br>"subObjCode"： "HOUR"，<br>"subObjID"： "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>以下是对所包含字段的描述：

* **changeType：**&#x200B;对对象所做的更改类型：

   * **A：**&#x200B;添加

   * **E：**&#x200B;编辑

   * **D：**&#x200B;删除

* **aux2：**&#x200B;小时记录所针对的用户名称。

* **newNumberVal：**&#x200B;小时记录的新值（如果changeType为D，该值将为Null）。

* **oldNumberVal：**&#x200B;小时记录的上一个值。

* **subObjCode：**&#x200B;正在修改的记录类型（应始终为HOUR）。

* **subObjID：**&#x200B;小时记录的ID。

您可以使用此信息发现哪些小时记录已更改、编辑或删除。 如有必要，您可以使用subObjID从小时记录中检索更多信息。
