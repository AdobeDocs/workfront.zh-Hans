---
content-type: reference
navigation-topic: announcements
title: 群集1、2和3上的客户必须更新任允许列表何IP块，以防止阻止Adobe Workfront服务
description: 为了增强和改进我们的核心基础架构，我们很快将在聚类01、02和03上将Adobe Workfront客户迁移到AWS公共云。
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# 群集1、2和3上的客户必须更新任允许列表何IP块，以防止阻止Adobe Workfront服务

为了增强和改进我们的核心基础架构，我们很快将在聚类01、02和03上将Adobe Workfront客户迁移到AWS公共云。

作为此更改的一部分，您需要将以下IP添加允许列表到您的IP块，以防止阻止Workfront服务：

对于SSO和POP:

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

请确保您允许列表的IP块已在2019年5月13日之前更新。 有关更多信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

感谢您对Workfront的持续支持，我们正在努力为我们的客户创造更可靠、更可靠的体验。

如果您有其他问题，请通过访问experience.workfront.com或致电844.306.4357（美国）或+44.1256.274200(EMEA)联系我们的支持团队。

## 常见问题解答

### 为什么Workfront要做这些更改？

为了始终如一地为客户提供尽可能最好的服务，Workfront会不断寻找改进用户体验的方法。 这一变化利用了新技术，使我们能够提供尽可能最佳的体验并改进我们已经强大的安全模型。

### 作为Workfront管理员，我需要执行哪些操作？

请联系您的内部IT或安全部门，以获得有关审核IP允许列表块和添加上面所列IP方面的帮助。

### 如果我们不进行此更改，我的组织会期待什么？

当我们将服务迁移到新IP时，您将无法访问Workfront服务。
