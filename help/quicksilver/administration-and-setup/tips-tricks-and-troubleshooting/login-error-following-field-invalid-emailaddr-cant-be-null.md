---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''登录错误：以下字段无效：emailAddr不能为null'
description: 我尝试登录时 [!DNL Adobe Workfront] 我的域的URL将被重定向到SAML登录门户，然后重定向回 [!DNL Workfront] 中，出现一个错误，指示emailAddr字段不能为null。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# 登录错误：以下字段无效：emailAddr不能为null

## 问题

我尝试登录时 [!DNL Adobe Workfront] 使用我的URL(https://customerdomain.my.workfront.com)，我会被重定向到SAML登录门户，然后被重定向回 [!DNL Workfront] 出现以下错误：

“让我们再试一次。以下字段无效：emailAddr不能为null。”

## 原因

此错误是由SAML 2.0配置的“映射用户属性”区域中的项不正确导致的。 有关为SAML 2.0映射用户属性的更多信息，请参阅 [使用SAML 2.0配置Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## 解决方案

更新电子邮件地址的属性映射，然后单击 **[!UICONTROL 保存]**.
