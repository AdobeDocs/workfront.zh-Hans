---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “从Adobe Workfront导出历史数据：优点和缺点'
description: 本文介绍了4个用于从Workfront导出历史数据的选项的优缺点。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 从导出历史数据 [!DNL Adobe Workfron]t:优点和缺点

本文说明了4个用于从导出历史数据的选项的利弊 [!DNL Workfront].

## 使用我们的合作伙伴之一

[!DNL AtAppStore], a [!DNL Workfront] 经认证的合作伙伴拥有一个易于使用的应用程序，可让您下载数据。 此应用程序还包含一个查看器，可让您轻松查看数据。

* **优点：** 所有 [!DNL Workfront] 将导出对象，包括自定义字段。 查看器的界面易于使用和阅读，并且在 [!DNL MS Access] 数据库。

* **缺点：** 文档不会导出。 您必须单独下载它们。 有关更多信息，请转到 [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx。](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 请求 [!DNL Postgres] 数据库团队的数据转储文件

您的客户经理可以向我们的数据库团队提交请求，以导出数据库转储文件(.dmp) [!DNL Postgres] 文件)。 我们的AOS团队将收到另一个请求，以检索您存储的所有文档。

* **优点**:您将获得整个数据加载，包括自定义字段以及存储在系统中的文档。

* **缺点**:数据库文件很难读取：除非您将此文件上传到 [!DNL Postgres] 数据库和重新建立表之间的关系。 文档存储在单独的文件服务器上，并且必须由AOS团队使用单独的进程单独提取。 这样做时，文档没有组织，所有文档均被其GUID引用。
* **成本**:根据团队创建文件所花费的时间，与此下载相关联的成本会有所不同。 请咨询您的AE/CAE ，以了解更多信息或开始此过程。

## 导出方式 [!UICONTROL 启动]

无论您是否拥有远程咨询小时数，您都可以使用我们的一位顾问以报告或 [!UICONTROL 启动]，或者您也可以自行运行这些报表：

* **优点**:这些报告易于阅读，可以在各种应用程序中导入；可以自定义这些组以包含您想要的任何分组和视图。

* **缺点**:文档必须单独下载。

* **成本**:如果您可以自行运行这些报表（只需系统管理员登录即可），或者您可以使用剩余的远程咨询时间，则此服务是免费的。 如果您有兴趣购买远程咨询服务，请咨询您的AE/CAE。

   有关使用Kick-Start导出数据的更多信息，请参阅 [从导出数据 [!DNL Adobe Workfront] 通过 [!UICONTROL 启动]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## 使用我们的开放API

如果您在组织中拥有正确的资源，则他们可以构建一个自定义API，以从Workfront中检索所有数据：

* **优点**:您可以控制从系统导出的内容。

* **缺点**:此时间花在您身边，您必须查找资源才能对API进行代码并执行导出。

* **成本**:组织的内部。
