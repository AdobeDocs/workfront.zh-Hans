---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 从Adobe Workfront导出历史数据：优缺点
description: 本文介绍了可用于从Workfront导出历史数据的4个选项的优缺点。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 从[!DNL Adobe Workfront]导出历史数据：优缺点

<!-- Audited: 5/2025 -->

本文介绍了可用于从Adobe Workfront导出历史数据的4个选项的优缺点。

## 使用我们的合作伙伴之一

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com))有一个易于使用的应用程序（其[Workfront快照](https://store.atappstore.com/product/workfront-snapshot/)解决方案），允许您自行下载数据。 可选查看器（其[Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)解决方案）允许您轻松地脱机查看数据。

* **优点：**&#x200B;所有核心[!DNL Workfront]对象均已导出，包括自定义字段和注释，并存储在易于访问的[!DNL MS Access]数据库中。 查看器的界面易于使用和读取。 “提取文档”也作为服务单独提供，输出组织为逻辑文件夹结构，该结构映射到每个文档及其以前版本。

* **缺点：**&#x200B;技术限制为2GB数据，但AtAppStore允许您仅购买所需的数据。

* **费用：**&#x200B;有关详细信息，请转到[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/)。



## 通过[!UICONTROL Kick-Start]导出

无论您是否拥有远程咨询时间，您都可以使用我们的顾问之一以报告或[!UICONTROL kick-starts]的形式导出您的数据，或者您可以自己运行这些报告：

* **优点**：报告易于阅读，可以在各种应用程序中导入。 可以对其进行自定义以包含所需的任何分组和视图。

* **问题**：必须单独下载文档。

* **费用**：如果您可以自行运行报告（只需系统管理员登录即可），或者可以使用剩余的远程咨询时间，则免费。 如果您有兴趣为此购买远程咨询，请与您的AE/CAE联系。

  有关使用Kick-Starts导出数据的详细信息，请参阅[通过 [!DNL Adobe Workfront] Kick-Starts[!UICONTROL 从]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)导出数据。

## 使用我们的开放API

如果您所在的组织中拥有正确的资源，则可以构建自定义API以从Workfront检索您的所有数据：

* **优点**：您控制着从系统中导出的内容。

* **缺点**：时间在您的身边，您必须找到资源为API编码并执行导出。

* **成本**：这是您组织的内部成本。
