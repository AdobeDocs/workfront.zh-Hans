---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager集成疑难解答
description: 问题：Assets未保存到Adobe Experience Manager
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Adobe Experience Manager集成疑难解答

## 问题：Assets未保存到Adobe Experience Manager

当用户选择要导出到Experience Manager Assets的资源或文件夹并单击选择时，选择器窗口关闭，但资源未保存到Experience Manager Assets。 Workfront中没有任何迹象表明资产未保存到Experience Manager Assets。

### 原因

这可能是因为Adobe Cloud Manager中的允许列表。 如果组织的Adobe Cloud Manager允许列表为空，则IP地址不受限制，Workfront可以在Adobe Experience Manager中访问组织的文件夹和资源。 但是，如果即使将单个IP地址添加到Cloud Manager，则允许列表列入允许列表会假定不允许列表以外的任何IP地址。 因此，如果Cloud Manager 列入允许列表包含任何IP地址，则还必须将Workfront 列入允许列表 IP地址添加到，以使Workfront能够将资源发送到Experience Manager Assets。

### 解决方案：

将Workfront IP地址添加到Adobe Cloud Manager 列入允许列表。

* 有关将IP地址添加到Adobe Cloud Manager的说明，请参阅Adobe Experience Manager文档中的[IP允许列表简介](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction)。
* 有关要添加到Workfront的列入允许列表 IP地址列表，请参阅[配置防火墙](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
