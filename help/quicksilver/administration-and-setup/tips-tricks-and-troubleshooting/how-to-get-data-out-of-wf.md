---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '从Adobe Workfront导出历史数据：优缺点'
description: 本文介绍了可用于从Workfront导出历史数据的4个选项的优缺点。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 从[!DNL Adobe Workfron]t导出历史数据：优缺点

本文说明可用于从[!DNL Workfront]导出历史数据的4个选项的优缺点。

## 使用我们的合作伙伴之一

[!DNL AtAppStore]是[!DNL Workfront]认证合作伙伴，它有一个易于使用的应用程序，允许您下载数据。 此应用程序还包含一个查看器，可让您轻松查看数据。

* **优点：**&#x200B;已导出所有[!DNL Workfront]对象，包括自定义字段。 查看器的界面易于使用和读取，并且很容易导入到[!DNL MS Access]数据库中。

* **缺点：**&#x200B;文档未导出。 您必须单独下载它们。 有关详细信息，请转到[http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx。](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 从我们的数据库团队请求[!DNL Postgres]数据转储文件

您的客户经理可以向我们的数据库团队提交请求，以导出包含您数据的数据库转储文件（.dmp [!DNL Postgres]文件）。 另外，我们的AOS团队将收到一个请求，要求您检索所有存储的文档。

* **优点**：获取整个数据加载，包括自定义字段以及存储在系统中的文档。

* **缺点**：数据库文件很难读取：除非将其上载到[!DNL Postgres]数据库并重新建立表之间的关系，否则无法读取此文件。 文档存储在单独的文件服务器上，必须由AOS团队使用单独的进程单独提取。 这样做时，文档没有组织，并且它们都由其GUID引用。
* **成本**：此下载会产生成本，具体取决于团队创建文件所需的时间。 请与您的AE/CAE联系，以了解详细信息或开始此流程。

## 通过[!UICONTROL Kick-Start]导出

无论您是否拥有远程咨询时间，您都可以使用我们的顾问之一以报告或[!UICONTROL kick-starts]的形式导出您的数据，或者您可以自己运行这些报告：

* **优点**：报告易于阅读，可以在各种应用程序中导入；可以对其进行自定义以包含所需的任何分组和视图。

* **问题**：必须单独下载文档。

* **费用**：如果您可以自行运行报告（只需系统管理员登录即可），或者可以使用剩余的远程咨询时间，则免费。 如果您有兴趣为此购买远程咨询，请与您的AE/CAE联系。

  有关使用Kick-Starts导出数据的详细信息，请参阅[通过[!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)从 [!DNL Adobe Workfront] 导出数据。

## 使用我们的开放API

如果您所在的组织中拥有正确的资源，则可以构建自定义API以从Workfront检索您的所有数据：

* **优点**：您控制着从系统中导出的内容。

* **缺点**：时间在您的身边，您必须找到资源为API编码并执行导出。

* **成本**：组织内部成本。
