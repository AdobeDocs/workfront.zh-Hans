---
title: 使用增强型身份验证时更新IDP中的SAML 2.0元数据
description: 作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML) 2.0协议的身份提供程序集成。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 使用增强型身份验证时更新IDP中的SAML 2.0元数据

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML) 2.0协议的身份提供程序集成。

以下部分介绍了将您的Workfront帐户升级到增强型身份验证体验（尚未提供给所有组织）时的集成过程。 有关增强的身份验证体验的详细信息，请参阅 [增强型身份验证概述](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

有关在迁移到增强型身份验证体验之前配置SAML的信息，请参阅 [在身份提供程序中更新SAML 2.0元数据](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用Okta作为您的身份提供程序

Okta是支持SAML 2.0的标识提供程序的示例。本节介绍如何使用Okta作为您的身份提供程序。 在配置另一个支持SAML 2.0的标识提供程序时，需要执行类似的步骤。

>[!NOTE]
>
>将根据用户的电子邮件地址来映射用户。 要使用Okta登录Workfront，您必须让某个用户使用在Workfront客户中创建的相同（不区分大小写）电子邮件地址。

请完成以下各节，以在Workfront中将Okta配置为您的身份提供程序。

* [在Okta中创建Workfront应用程序](#create-a-workfront-app-in-okta)
* [在Workfront中添加您的Okta实例作为身份提供程序](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### 在Okta中创建Workfront应用程序 {#create-a-workfront-app-in-okta}

1. 登录到您的Okta环境。
1. 确保 **经典UI** 在Okta界面的左上角选择。
1. 在菜单中，单击 **应用程序** > **应用程序**.

1. 单击 **添加应用程序**，然后单击 **创建新应用程序**.

1. 在 **新建应用程序集成对话框** 框，选择 **SAML 2.0**，然后单击 **创建**.

1. 指定Workfront应用程序的名称，然后单击 **下一个**.
1. 在显示的“SAML设置”页中，找到“SAML设置”页所需的信息：

   1. 无需退出显示Okta界面的浏览器选项卡，请打开单独的浏览器选项卡或窗口。
   1. 在浏览器中指定以下URL：

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. 在生成的XML文件中，确定 **entityID** 和 **位置**.

      ![sso-okta.png](assets/sso-okta.png)

   1. 从以下位置复制值 **entityID** 字段到您的系统剪贴板。 请勿关闭此浏览器选项卡。

1. 返回在步骤6中打开的“SAML设置”页面。
1. 粘贴来自以下位置的值： **entityID** 字段到 **受众URI（SP实体ID）** 字段。

1. 在其他浏览器选项卡的XML文件中，从 **位置** 字段。
1. 粘贴来自以下位置的值： **位置** 字段到 **单点登录** **URL** 字段。

1. 滚动到 **属性语句（可选）** 部分。
1. 在 **名称** 字段，指定 **电子邮件**.

1. 在 **值** 字段，指定 **user.email**.

1. （可选）添加任何高级值。
1. 单击 **下一个**.
1. 选择， **我是Okta客户，正在添加内部应用程序**，然后单击 **完成**.

### 在Workfront中添加您的Okta实例作为身份提供程序 {#add-your-okta-instance-as-an-identity-provider-in-workfront}

此过程提供了在Workfront中将Okta配置为身份提供程序的基本信息。 有关其他映射或配置选项的其他信息，请参见 [使用SAML 2.0配置Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. 下载Okta实例的身份提供程序元数据：

   1. 登录到您的Okta环境。
   1. 确保 **经典UI** 在Okta界面的左上角选择。
   1. 在菜单中，单击 **应用程序** > **应用程序**.

   1. 单击您创建的Workfront应用程序，如部分所述， [在Okta中创建Workfront应用程序](#create-a-workfront-app-in-okta)
   1. 在 **登录** 选项卡，单击 **身份提供程序元数据**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      元数据在新的浏览器选项卡中以XML形式打开。

   1. 复制浏览器URL字段中显示的URL。

1. 以Workfront管理员身份登录Workfront。
1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统** > **单点登录(SSO)**.

1. （视情况而定）如果看到两个选项卡，请单击 **新的SSO提供商** 选项卡。

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >请勿删除中的现有SSO配置设置 **当前SSO供应商** 选项卡，直到您的帐户更新为增强的身份验证体验并且新的SSO配置完全起作用。

1. 单击 **新建SSO供应商**.
1. 指定名称（如Okta IDP），然后指定描述。
1. 在 **填充身份提供程序元数据中的字段** 部分，将您在步骤1中复制的URL粘贴到 **元数据URL** 字段。\
   或者，您可以单击 **选择文件** 上传.xml文件，但我们建议您粘贴该URL。

1. 在 **映射用户属性** 部分，在 **目录属性** 字段，类型 **电子邮件**. (**电子邮件地址** 已填充在 **Workfront用户属性** 字段。)

1. （可选）启用 **设为默认SSO供应商** 将未经身份验证的用户发送到身份提供程序登录屏幕而不是Workfront登录屏幕以进行身份验证。 我们建议您仅在系统中的所有用户都通过身份提供程序访问Workfront时才启用此选项。
1. 选择 **启用** 复选框。 在执行此操作之前，请确保系统中的用户知道新的登录体验，以确保他们不会失去对Workfront系统的访问权限。
1. 单击 **测试连接**.\
   您应该会看到一条消息，告诉您连接成功。

1. 单击&#x200B;**保存**。

## 使用其他身份提供程序

使用非Okta身份提供程序（例如Ping或Centrify）时，必须将Workfront元数据重新上传到您的身份提供程序。
