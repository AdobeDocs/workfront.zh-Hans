---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop无法建立连接
description: 当您尝试将Tableau桌面连接到Data Connect时，您会收到错误。
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 0%

---

# Tableau Desktop无法建立连接

## 问题

当您尝试将Tableau Desktop连接到Data Connect时，您会看到以下错误：

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## 原因

此错误是由本地计算机上的代理设置导致的，该设置阻止从Data Connect加载数据。

Data Connect通过第三方Snowflake云服务提供。 Tableau需要打开网络才能与Snowflake通信。

## 解决方案

您可以尝试以下方法来解决此问题：

* **禁用安全工具以进行故障排除**：关闭安全工具（如Zscaler或Cisco）以查看它是否解决了连接问题。 如果这解决了连接问题，请确保您的安全工具已升级到最新版本，将Data Connect (Snowflake) IP地址添加到与内部网络团队的VPN 允许列表。

* **将IP地址添加到允许列表**：确保防火墙设置允许Data Connect使用的IP地址。 使用命令`SYSTEM$ALLOWLIST()`获取IP地址，然后可以在VPN中列入允许列表该地址。

* **检查防火墙和代理设置**：检查网络上的任何防火墙或代理配置是否阻止访问Snowflake端点。 您可能需要联系网络管理员，将所需的Snowflake IP地址和端口添加到公司的IP允许列表中。

* **解决方法选项**：在Tableau中，从工作表屏幕而不是Data Source窗格创建提取。 连接没有丢失，提取过程已完成。
