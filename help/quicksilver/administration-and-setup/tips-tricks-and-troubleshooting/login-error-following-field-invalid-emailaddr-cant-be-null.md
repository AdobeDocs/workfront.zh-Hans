---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 登录错误：以下字段无效： emailAddr不能为空
description: 当我尝试登录 [!DNL Adobe Workfront] 我的域的URL时，我将被重定向到SAML登录门户，然后重定向回 [!DNL Workfront] ，并返回一个错误，说明emailAddr字段不能为null。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# 登录错误：以下字段无效： emailAddr不能为空

## 问题

当我尝试使用我的URL (https://customerdomain.my.workfront.com)登录[!DNL Adobe Workfront]时，我将被重定向到SAML登录门户，然后重定向回[!DNL Workfront]，并出现以下错误：

“让我们再试一次。 以下字段无效： emailAddr不能为空。”

## 原因

此错误是由于SAML 2.0配置的“映射用户属性”区域中的项目不正确导致的。 有关为SAML 2.0映射用户属性的更多信息，请参阅[使用SAML 2.0配置Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)。

## 解决方案

更新电子邮件地址的属性映射，然后单击&#x200B;**[!UICONTROL 保存]**。
