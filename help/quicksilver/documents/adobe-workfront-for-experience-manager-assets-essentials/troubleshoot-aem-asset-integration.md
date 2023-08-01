---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager集成疑难解答
description: 将您的工作与Experience Manager Assets Essentials中的内容连接起来 — 编辑我。
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Adobe Experience Manager集成疑难解答

## 问题：资源未保存到Adobe Experience Manager

当用户选择要导出到Experience Manager Assets的资源或文件夹并单击选择时，选择器窗口关闭，但资源未保存到Experience Manager Assets。 Workfront中没有任何迹象表明资产未保存到Experience Manager Assets。

### 原因

由于AdobeCloud Manager中的允许列表，可能会发生此情况。 如果组织的Cloud ManagerAdobe列入允许列表为空，则IP地址不受限制，Workfront可以在Adobe Experience Manager中访问组织的文件夹和资源。 但是，如果即使将单个IP地址添加到Cloud Manager，则允许列表列入允许列表会假定不允许列表中没有的任何IP地址。 因此，如果Cloud Manager包含任何IP地址，则还必须将Workfront 列入允许列表 IP地址添加到允许列表，以使Workfront能够将资源发送到Experience Manager Assets。

### 解决方案：

将Workfront IP地址添加到Adobe列入允许列表 Cloud Manager。

* 有关将IP地址添加到AdobeCloud Manager的说明，请参阅 [IP允许列表简介](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) 请参阅Adobe Experience Manager文档。
* 有关要添加到Workfront的列入允许列表 IP地址的列表，请参阅 [配置防火墙](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


