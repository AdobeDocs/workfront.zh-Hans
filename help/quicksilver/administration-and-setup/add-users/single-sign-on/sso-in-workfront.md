---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront中的单点登录概述
description: Workfront提供集中管理的单点登录(SSO)配置，该配置可轻松将Workfront与您现有的企业SSO解决方案集成。 此配置易于设置和管理，适用于OnDemand和OnPremise Enterprise客户。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Adobe Workfront中的单点登录概述

{{important-admin-console-onboard}}


Workfront提供集中管理的单点登录(SSO)配置，该配置可轻松将Workfront与您现有的企业SSO解决方案集成。 此配置易于设置和管理，适用于OnDemand和OnPremise Enterprise客户。

要在Workfront中使用SSO功能，您的组织需要设置SSO应用程序。 然后，您可以配置Workfront，以便它可以与您的SSO解决方案通信。

联合解决方案允许用户通过在集中登录门户中输入其用户名和密码来登录其所有应用程序。

![](assets/overview-sso-wf.png)


## 配置防火墙

使用SSO解决方案时，Workfront会在指定端口上启动与服务器的连接。

如果您按需订阅Workfront，并且已将防火墙或邮件服务器配置为仅允许访问特定供应商，则需要将某些Workfront IP地址添加到防火墙允许列表。 有关更多信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 配置单点登录

Workfront与以下SSO解决方案集成：

* 支持SAML 2.0的联合解决方案

   有关将Workfront与SAML 2.0集成的信息，请参阅 [使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* 支持使用ADFS的SAML 2.0的联合解决方案

   有关使用ADFS将Workfront与SAML 2.0集成的信息，请参阅 [使用ADFS使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
