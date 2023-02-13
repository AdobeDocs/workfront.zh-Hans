---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront与Workfront校样之间的用户同步
description: 用户信息从Adobe Workfront同步到Workfront Proof;它未从Workfront校样同步到Workfront。 因此，无论您何时创建或修改用户，都必须在Workfront中进行这些更改。 您无法在Workfront校样中更改用户。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront与Workfront校样之间的用户同步

用户信息从Adobe Workfront同步到Workfront Proof;它未从Workfront校样同步到Workfront。 因此，无论您何时创建或修改用户，都必须在Workfront中进行这些更改。 您无法在Workfront校样中更改用户。

以下部分提供了有关从Workfront到Workfront校样的用户同步信息：

## 已同步的信息

Workfront将以下用户信息同步到Workfront校样：

* 名称（用户的名字和姓氏）
* 电子邮件地址

## 发生同步时

在以下情况下，用户信息会从Workfront同步到Workfront校样：

* 用户信息在Workfront中更新
* 用户在Workfront中创建

根据Workfront校样中是否存在具有相同电子邮件地址的用户，会出现以下任一情况：

* **如果Workfront校样和**

   * **为用户启用了校样：** 用户在Workfront校样中创建为用户。
   * **未为用户启用校对：** 用户将在Workfront校样中创建为联系人。

* **如果Workfront校样中存在具有匹配电子邮件的用户：** 校样在Workfront中为该用户启用（如果尚未启用），并且信息会在两个用户之间同步。

   有关更多信息，请参阅 [配置用户的校对访问权限](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [配置用户的校对访问权限](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >当具有匹配电子邮件的用户存在于其自己或其他校对环境中时，Workfront会通过在其电子邮件中添加用户帐户id作为后缀来创建别名电子邮件地址。 例如， *username+accountid@domain.com*. 在创建别名电子邮件时，用户仍会收到校样通知。
