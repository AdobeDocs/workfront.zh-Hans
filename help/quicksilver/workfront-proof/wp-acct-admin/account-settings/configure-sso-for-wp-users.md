---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 为 [!DNL Workfront Proof] 用户配置单点登录
description: 如果您拥有Select或Premium计划，则可以提供单点登录(SSO)功能，该功能允许您使用现有组织的用户名和密码来访问您的 [!DNL Workfront Proof] 帐户。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# 为[!DNL Workfront Proof]用户配置单点登录

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果您拥有Select或Premium计划，则可以提供单点登录(SSO)功能，该功能允许您使用现有组织的用户名和密码访问您的[!DNL Workfront Proof]帐户。

这意味着您将针对自己的登录系统，而不是[!DNL Workfront Proof]登录页面进行身份验证。

>[!NOTE]
>
>必须在[!DNL Workfront Proof]帐户上设置自定义子域或域才能启用SAML。 自定义子域可自由设置。 有关详细信息，请参阅[品牌](https://support.workfront.com/hc/en-us/sections/115000921208-Branding)。您可以阅读有关我们的[品牌 [!DNL Workfront Proof] 网站 — 高级](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)上完全自定义域的详细信息。

## 在[!DNL Workfront Proof]中启用SSO

可以在[!UICONTROL 帐户设置]的[!UICONTROL 单点登录]选项卡上启用单点登录功能，该功能将应用于[!DNL Workfront Proof]帐户上的所有用户。 有关详细信息，请参阅[帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)。

## 实体Id

作为服务提供商，我们已在此处发布实体ID：

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) （其中“您的子域”是您帐户的子域）

[!DNL Workfront Proof]需要用户的电子邮件地址作为其唯一标识符，该唯一标识符可以作为以下属性之一传递：

* urn:mace:dir:attribute-def:电子邮件地址
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* 邮件
* 电子邮件
* 电子邮件地址

要配置SSO，请执行以下操作：

1. 打开&#x200B;**[!UICONTROL 单点登录]**&#x200B;选项卡(1)。
1. 输入&#x200B;**SSO URL** (2)。
这是指向您的SSO服务器的链接(例如，**https://sso.mycompany.com/opensso**)。

1. 输入&#x200B;**登录URL** (3)。
将调用此URL以将用户重定向到您的身份提供程序。

   这不是您在浏览器中输入的实际URL，而是端点，它将处理我们发送的信息以显示“登录”屏幕。

1. 输入&#x200B;**注销URL** (4)。
例如，这是您注销后返回到的URL

   **https://www.yourcompany.com/services/logout.asp**

1. 输入&#x200B;**证书指纹** (5)。
1. SAML身份提供程序提供的SAML证书的SHA1指纹。
1. 通过在您的身份提供程序中设置此项，确保包括密钥信息。
1. 将&#x200B;**SSO**&#x200B;切换为&#x200B;**[!UICONTROL 已启用]** (6)。
启用SSO后，您和您帐户上的其他用户将使用您自己的身份验证机制登录。 这意味着当用户访问您的[!DNL Workfront Proof]帐户登录屏幕(例如，**yourcompany.proofhq.com/login**)时，将会提示他们使用传输窗口转到您自己的身份验证登录页面。

1. （可选）启用&#x200B;**自动设置用户** (7)。
启用此选项后，将自动为没有自己的[!DNL Workfront Proof]配置文件但将使用其单点登录凭据访问您的[!DNL Workfront Proof]帐户的用户创建用户帐户。 仅当您的帐户尚未达到用户限制时，才会执行此操作。

1. 默认情况下，新设置的用户将分配有Manager配置文件权限。 如果您需要更多信息，请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的校对权限配置文件。

![启用_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## 为附属帐户启用SSO

当附属帐户连接到中心帐户时，您可以从中心帐户级别管理这些帐户。

单点登录是Select和Premium的一项功能，因此单点登录只能在Select和Premium计划中的卫星上启用。

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]** (1)。

1. 在下拉菜单(2)中单击附属帐户。
1. 打开&#x200B;**[!UICONTROL 单点登录]**&#x200B;选项卡(3)。
1. 开始编辑SSO配置(4)
1. ![正在启用_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
在此，您将有两种配置方法(5)：

1. **继承：** SSO，配置取自您的中心帐户。
如果用户通过&#x200B;**默认登录页面** ([https://business.adobe.com/cn/products/workfront/proofing-approvals.html](https://business.adobe.com/cn/products/workfront/proofing-approvals.html))访问[!DNL Workfront Proof]，则将有&#x200B;**两个级别的授权**：首先要求用户使用[!DNL Workfront Proof]访问数据（电子邮件和密码）登录；然后通过SSO窗口将该用户传输到SSO登录页面。
因此，启用SSO服务后，我们建议通过您自己的[!DNL Workfront Proof]子域/域登录。

   >[!NOTE]
   >
   >此时，当您的[!DNL Workfront Proof]帐户已启用单点登录时，您将无法使用这些凭据登录到iPhone应用程序。

   1. **手动**（默认）：具有不同配置的SSO（例如，指向另一个身份提供程序）。

      >[!NOTE]
      >
      >如果附属帐户从中心帐户继承SSO配置，则登录屏幕将是中心帐户的登录屏幕。 当卫星帐户用户在此页面上输入其SSO登录详细信息时，他们将被重定向回卫星帐户。

      ![正在启用_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. 单击&#x200B;**[!UICONTROL 保存]** (6)。

## 从中心帐户继承的SSO设置

当您选择从您的中心帐户继承设置时，您会注意到所有字段现在都使用来自您的中心帐户(7)的数据进行填充，并且单点登录在您的主帐户上自动启用/禁用(8)。 字段中也不再有编辑链接，因为现在可以从您的中心帐户设置并管理卫星帐户的整个SSO配置。

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

在您的中心帐户(9)中，[!UICONTROL SSO使用情况]字段显示此配置正由附属帐户(10)使用。\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## 手动配置SSO

如果已为卫星帐户(1)选择了手动SSO配置，则需要手动输入单点登录的数据。

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]** (1)。

1. 打开&#x200B;**[!UICONTROL 单点登录]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 编辑]，**&#x200B;填充该字段，然后单击&#x200B;**[!UICONTROL 保存]** (2)。

1. 在&#x200B;**[!UICONTROL SSO]**&#x200B;行上，单击&#x200B;**[!UICONTROL 已启用]** (3)。

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO登录

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]** (1)。

1. 打开&#x200B;**[!UICONTROL 单点登录]**&#x200B;选项卡。
1. 确保已设置您的[!DNL Workfront Proof]域/子域(1)，并且您的用户可通过此自定义域/子域访问您的[!DNL Workfront Proof]帐户。
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
启用单点登录后，您的子域登录URL(例如yourcompany.proofhq.com/login)将显示一个传输屏幕(2)，该屏幕会直接将您带到SSO登录页面。
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. 如果用户通过页面&#x200B;**([https://business.adobe.com/cn/products/workfront/proofing-approvals.html](https://business.adobe.com/cn/products/workfront/proofing-approvals.html))中的**&#x200B;默认日志访问[!DNL Workfront Proof]，将有&#x200B;**两个级别的授权**。 首先要求用户使用[!DNL Workfront Proof]访问数据（电子邮件和密码）登录。 然后，通过SSO窗口(2)将用户传送到SSO登录页。\
   因此，启用SSO服务后，我们建议通过您自己的[!DNL Workfront Proof]子域/域登录。

1. 目前，当您的Workfront Proof帐户上启用了单点登录时，您将无法使用这些凭据登录到iPhone应用程序。

## 关于添加新用户

当您的[!DNL Workfront Proof]帐户上启用了单点登录功能时，新用户将不会收到任何确认电子邮件，因为其帐户将被自动激活并可供使用。

在您的[!DNL Workfront Proof]登录页面上，单击[!UICONTROL 登录]按钮后，用户将被带到SSO登录页面并被要求输入您的单点登录登录凭据。

>[!IMPORTANT]
>
>在验证过程中，用户将通过电子邮件地址进行标识，这意味着用于SSO登录的电子邮件帐户必须是您在帐户中注册的用户的电子邮件地址。

## Active Directory联合身份验证服务(AD FS)

Active Directory联合身份验证服务(AD FS)是可以安装在Windows Server操作系统上的[!DNL Microsoft]软件组件，它为用户提供了对跨组织边界定位的系统和应用程序的单点登录访问。 有关详细信息，请参阅Microsoft开发人员网络网站上的“Active Directory联合身份验证服务”。

[!DNL Workfront Proof]系统支持SAML 2.0，并且仅与AD FS版本2.0或更高版本兼容。

有关详细说明，请参阅[在 [!DNL Workfront Proof]中单点登录： AD FS配置](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md)。
