---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront中的单点登录概述
description: Workfront提供了一个集中管理的单点登录(SSO)配置，可轻松将Workfront与您现有的公司SSO解决方案集成。 此配置易于设置和管理，并适用于OnDemand和OnPremise Enterprise客户。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Adobe Workfront中的单点登录概述

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront提供了一个集中管理的单点登录(SSO)配置，将Workfront与您现有的公司SSO解决方案集成。 此配置适用于OnDemand和OnPremise Enterprise客户。

要在Workfront中使用SSO功能，您的组织需要设置SSO应用程序。 然后，您可以配置Workfront，以便它能与您的SSO解决方案进行通信。

联合解决方案允许用户通过在集中式登录门户中输入用户名和密码来登录其所有应用程序。

![SSO联合](assets/overview-sso-wf-fed-only.png)


## 配置防火墙

使用SSO解决方案时，Workfront会在指定端口上启动与服务器的连接。

如果您的防火墙或邮件服务器配置为只允许特定供应商访问，则必须将某些Workfront 列入允许列表 IP地址添加到防火墙。 有关详细信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 配置单点登录

Workfront与以下SSO解决方案集成：

* 支持SAML 2.0的联合解决方案

  有关将Workfront与SAML 2.0集成的信息，请参阅[使用SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)配置Adobe Workfront。

* 支持使用ADFS的SAML 2.0的联合解决方案

  有关使用ADFS将Workfront与SAML 2.0集成的信息，请参阅[使用ADFS使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)。
