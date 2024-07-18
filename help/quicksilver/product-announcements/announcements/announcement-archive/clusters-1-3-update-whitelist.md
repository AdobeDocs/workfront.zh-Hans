---
content-type: reference
navigation-topic: announcements
title: 列入允许列表群集1、2和3上的客户必须更新任何IP块，以防止阻塞Adobe Workfront服务
description: 为了增强和改进我们的核心基础架构，我们很快会将集群01、02和03上的Adobe Workfront客户迁移到AWS公共云。
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# 列入允许列表群集1、2和3上的客户必须更新任何IP块，以防止阻塞Adobe Workfront服务

为了增强和改进我们的核心基础架构，我们很快会将集群01、02和03上的Adobe Workfront客户迁移到AWS公共云。

作为此更改的一部分，您需要将以下IP添加到允许列表IP块，以防止阻止Workfront服务：

对于SSO和POP：

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

对于电子邮件：

* 54.240.60.174
* 54.240.60.175

请确保在2019年5月13日之前更新允许列表IP块。 有关详细信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

感谢您对Workfront的持续支持，我们正努力为客户营造更可靠和更强大的体验。

如果您有任何其他问题，请通过访问experience.workfront.com或致电844.306.4357 （美国）或+44.1256.274200 (EMEA)联系我们的支持团队。

## 常见问题解答

### 为什么Workfront要做出此更改？

为了始终如一地为客户提供最佳服务，Workfront不断寻找改善用户体验的方法。 这一变化利用了新技术，使我们能够提供最佳体验，并改进我们本已强大的安全模型。

### 作为Workfront管理员，我需要执行哪些操作？

请与您的内部IT或安全部门联系，以获得有关检查允许列表IP块和添加上面列出的IP的帮助。

### 如果我们不做出此更改，我的组织会期待什么？

在将服务迁移到新IP时，您将无法访问Workfront服务。
