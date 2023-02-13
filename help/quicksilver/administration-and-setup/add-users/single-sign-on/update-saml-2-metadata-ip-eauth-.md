---
title: 使用增强的身份验证时，更新IDP中的SAML 2.0元数据
description: 作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML)2.0协议的身份提供程序相集成。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: b6fc4775953e47a1b9d84d7537a6d9f5d35b1f2c
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# 使用增强的身份验证时，更新IDP中的SAML 2.0元数据

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML)2.0协议的身份提供程序相集成。

以下各节介绍了将您的Workfront帐户升级为增强的身份验证体验（尚不适用于所有组织）时的集成过程。 有关增强的身份验证体验的更多信息，请参阅 [增强的身份验证概述](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

有关在迁移到增强的身份验证体验之前配置SAML的信息，请参阅 [在您的身份提供程序中更新SAML 2.0元数据](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用Okta作为身份提供者

Okta是支持SAML 2.0的身份提供程序的一个示例。本节将介绍如何将Okta用作您的身份提供程序。 配置支持SAML 2.0的其他身份提供程序时，需要执行类似步骤。

>[!NOTE]
>
>用户会根据其电子邮件地址进行映射。 要使用Okta登录Workfront，您必须在Workfront客户中创建具有相同（不区分大小写）电子邮件地址的用户。

请完成以下部分，以在Workfront中将Okta配置为身份提供者。

* [在Okta中创建Workfront应用程序](#create-a-workfront-app-in-okta)
* [在Workfront中将您的Okta实例添加为身份提供程序](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### 在Okta中创建Workfront应用程序 {#create-a-workfront-app-in-okta}

1. 登录到Okta环境。
1. 确保 **经典UI** 在Okta界面的左上角选择。
1. 在菜单中，单击 **应用程序** > **应用程序**.

1. 单击 **添加应用程序**，然后单击 **创建新应用程序**.

1. 在 **创建新的应用程序集成对话框** 框，选择 **SAML 2.0**，然后单击 **创建**.

1. 指定Workfront应用程序的名称，然后单击 **下一个**.
1. 在显示的“SAML设置”页面中，找到SAML设置页面所需的信息：

   1. 不退出显示Okta界面的浏览器选项卡，请打开单独的浏览器选项卡或窗口。
   1. 在浏览器中指定以下URL:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. 在生成的XML文件中，识别 **entityID** 和 **位置**.

      ![sso-okta.png](assets/sso-okta.png)

   1. 从 **entityID** 字段。 请勿关闭此浏览器选项卡。

1. 返回到您在步骤6中打开的“SAML设置”页面。
1. 粘贴 **entityID** 字段 **受众URI（SP实体ID）** 字段。

1. 在其他浏览器选项卡的XML文件中，从 **位置** 字段。
1. 粘贴 **位置** 字段 **单点登录** **URL** 字段。

1. 滚动到 **属性语句（可选）** 中。
1. 在 **名称** 字段，指定 **电子邮件**.

1. 在 **值** 字段，指定 **user.email**.

1. （可选）添加任何高级值。
1. 单击 **下一个**.
1. 选择 **我是Okta客户，正在添加一个内部应用程序**，然后单击 **完成**.

### 在Workfront中将您的Okta实例添加为身份提供程序 {#add-your-okta-instance-as-an-identity-provider-in-workfront}

此过程提供了在Workfront中将Okta配置为身份提供者的基本信息。 有关其他映射或配置选项的其他信息，请参阅 [使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. 下载Okta实例的身份提供程序元数据：

   1. 登录到Okta环境。
   1. 确保 **经典UI** 在Okta界面的左上角选择。
   1. 在菜单中，单击 **应用程序** > **应用程序**.

   1. 单击您创建的Workfront应用程序，如 [在Okta中创建Workfront应用程序](#create-a-workfront-app-in-okta)
   1. 在 **登录** ，单击 **身份提供程序元数据**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      在新的浏览器选项卡中以XML形式打开元数据。

   1. 复制浏览器URL字段中显示的URL。

1. 以Workfront管理员身份登录Workfront。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **单点登录(SSO)**.

1. （视情况而定）如果您看到两个选项卡，请单击 **新的SSO提供程序** 选项卡。

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >请勿在 **当前SSO提供程序** 选项卡，直到您的帐户更新为增强的身份验证体验，并且新的SSO配置完全正常运行。

1. 单击 **新的SSO提供程序**.
1. 指定名称（如Okta IDP），然后指定描述。
1. 在 **从身份提供程序元数据填充字段** 中，将您在步骤1中复制的URL粘贴到 **元数据URL** 字段。\
   或者，您也可以单击 **选择文件** 上传.xml文件，但我们建议您粘贴该URL。

1. 在 **映射用户属性** 部分，在 **目录属性** 字段，类型 **电子邮件**. (**电子邮件地址** 已在 **Workfront用户属性** 字段。)

1. （可选）启用 **创建默认SSO提供程序** 将未经授权的用户发送到身份提供程序登录屏幕，而不是Workfront登录屏幕进行身份验证。 仅当系统中的所有用户通过身份提供程序访问Workfront时，我们建议您启用此选项。
1. 选择 **启用** 复选框。 在执行此操作之前，请确保您系统中的用户了解新的登录体验，以确保他们不会丢失对Workfront系统的访问权限。
1. 单击 **测试连接**.\
   您应会看到一条消息，告知您连接已成功。

1. 单击&#x200B;**保存**。

## 使用其他身份提供程序

使用Okta以外的身份提供程序（例如Ping或Centrify）时，必须将Workfront元数据重新上传到您的身份提供程序。
