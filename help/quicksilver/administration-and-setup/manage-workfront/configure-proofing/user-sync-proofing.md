---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront和Workfront Proof之间的用户同步
description: 用户信息会从Adobe Workfront同步到Workfront Proof；而不会从Workfront Proof同步到Workfront。 因此，无论您何时创建或修改用户，都必须在Workfront中进行这些更改。 您不能更改Workfront Proof中的用户。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront和Workfront Proof之间的用户同步

用户信息会从Adobe Workfront同步到Workfront Proof；而不会从Workfront Proof同步到Workfront。 因此，无论您何时创建或修改用户，都必须在Workfront中进行这些更改。 您不能更改Workfront Proof中的用户。

以下部分提供了有关用户从Workfront同步到Workfront Proof的信息：

## 已同步的信息

Workfront将以下用户信息同步到Workfront Proof：

* 名称（用户的名字和姓氏）
* 电子邮件地址

## 发生同步时

在以下情况下，用户信息会从Workfront同步到Workfront Proof：

* 用户信息在Workfront中更新
* 在Workfront中创建用户

根据Workfront Proof中是否存在具有相同电子邮件地址的用户，会发生以下任一情况：

* **如果Workfront Proof中不存在具有匹配电子邮件的用户，则**

   * **已为以下用户启用校对：**&#x200B;该用户在Workfront Proof中创建为用户。
   * **未为用户启用校对：**&#x200B;该用户在Workfront Proof中创建为联系人。

* **如果Workfront Proof中存在具有匹配电子邮件的用户：**&#x200B;已在Workfront中为该用户启用校对（如果尚未启用），并且两个用户之间的信息已同步。

  有关详细信息，请参阅[配置用户的验证访问权限](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)中的[配置用户的验证访问权限](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)。

  >[!IMPORTANT]
  >
  >当具有匹配电子邮件的用户在其自己或其他验证环境中存在时，Workfront会通过将该用户的帐户ID作为后缀添加到其电子邮件中来创建别名电子邮件地址。 例如，*username+accountid@domain.com*。 创建别名电子邮件时，用户仍会收到验证通知。
