---
title: 使用增强型身份验证时更新IDP中的SAML 2.0元数据
description: 作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML) 2.0协议的身份提供程序集成。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# 使用增强型身份验证时更新IDP中的SAML 2.0元数据

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以将Workfront单点登录(SSO)与任何支持安全断言标记语言(SAML) 2.0协议的身份提供程序集成。

以下部分介绍了将您的Workfront帐户升级到增强型身份验证体验（尚未提供给所有组织）时的集成过程。 有关增强的身份验证体验的详细信息，请参阅[增强的身份验证概述](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md)。

有关在迁移到Enhanced Authentication Experience之前配置SAML的信息，请参阅[在身份提供程序中更新SAML 2.0元数据](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

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
1. 确保在Okta界面的左上角选择了&#x200B;**经典UI**。
1. 在菜单中，单击&#x200B;**应用程序** > **应用程序**。

1. 单击&#x200B;**添加应用程序**，然后单击&#x200B;**新建应用程序**。

1. 在&#x200B;**新建应用程序集成对话框**&#x200B;框中，选择&#x200B;**SAML 2.0**，然后单击&#x200B;**创建**。

1. 为您的Workfront应用指定一个名称，然后单击&#x200B;**下一步**。
1. 在显示的“SAML设置”页中，找到“SAML设置”页所需的信息：

   1. 无需退出显示Okta界面的浏览器选项卡，请打开单独的浏览器选项卡或窗口。
   1. 在浏览器中指定以下URL：

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. 在生成的XML文件中，识别&#x200B;**entityID**&#x200B;和&#x200B;**Location**&#x200B;的值。

      ![sso-okta.png](assets/sso-okta.png)

   1. 将&#x200B;**entityID**&#x200B;字段中的值复制到系统剪贴板。 请勿关闭此浏览器选项卡。

1. 返回在步骤6中打开的“SAML设置”页面。
1. 将&#x200B;**entityID**&#x200B;字段中的值粘贴到&#x200B;**受众URI （SP实体ID）**&#x200B;字段中。

1. 在其他浏览器选项卡的XML文件中，复制&#x200B;**位置**&#x200B;字段中的值。
1. 将&#x200B;**位置**&#x200B;字段中的值粘贴到&#x200B;**单点登录** **URL**&#x200B;字段中。

1. 滚动到&#x200B;**Attribute语句（可选）**&#x200B;部分。
1. 在&#x200B;**名称**&#x200B;字段中，指定&#x200B;**电子邮件**。

1. 在&#x200B;**值**&#x200B;字段中，指定&#x200B;**user.email**。

1. （可选）添加任何高级值。
1. 单击&#x200B;**下一步**。
1. 选择&#x200B;**我是Okta客户，正在添加内部应用程序**，然后单击&#x200B;**完成**。

### 在Workfront中添加您的Okta实例作为身份提供程序 {#add-your-okta-instance-as-an-identity-provider-in-workfront}

此过程提供了在Workfront中将Okta配置为身份提供程序的基本信息。 有关其他映射或配置选项的其他信息，请参阅[使用SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)配置Adobe Workfront。

1. 下载Okta实例的身份提供程序元数据：

   1. 登录到您的Okta环境。
   1. 确保在Okta界面的左上角选择了&#x200B;**经典UI**。
   1. 在菜单中，单击&#x200B;**应用程序** > **应用程序**。

   1. 单击您创建的Workfront应用程序，如[在Okta中创建Workfront应用程序](#create-a-workfront-app-in-okta)部分所述
   1. 在&#x200B;**登录**&#x200B;选项卡上，单击&#x200B;**身份提供程序元数据**。

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      元数据在新的浏览器选项卡中以XML形式打开。

   1. 复制浏览器URL字段中显示的URL。

1. 以Workfront管理员身份登录Workfront。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **单点登录(SSO)**。

1. （视情况而定）如果看到两个选项卡，请单击&#x200B;**新建SSO提供程序**&#x200B;选项卡。

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >请勿删除&#x200B;**当前SSO提供程序**&#x200B;选项卡中的现有SSO配置设置，直到您的帐户更新为增强型身份验证体验并且新的SSO配置完全正常工作为止。

1. 单击&#x200B;**新建SSO提供程序**。
1. 指定名称（如Okta IDP），然后指定描述。
1. 在&#x200B;**填充来自身份提供程序元数据**&#x200B;的字段中，将您在步骤1中复制的URL粘贴到&#x200B;**元数据URL**&#x200B;字段中。\
   或者，您可以单击&#x200B;**选择文件**&#x200B;以上传.xml文件，但我们建议您粘贴该URL。

1. 在&#x200B;**映射用户属性**&#x200B;部分的&#x200B;**目录属性**&#x200B;字段中，键入&#x200B;**电子邮件**。 (**Workfront用户属性**&#x200B;字段中已填充&#x200B;**电子邮件地址**。)

1. （可选）启用&#x200B;**设为默认SSO提供程序**&#x200B;以将未经身份验证的用户发送到身份提供程序登录屏幕而不是Workfront登录屏幕以进行身份验证。 我们建议您仅在系统中的所有用户都通过身份提供程序访问Workfront时才启用此选项。
1. 选中&#x200B;**启用**&#x200B;复选框。 在执行此操作之前，请确保系统中的用户知道新的登录体验，以确保他们不会失去对Workfront系统的访问权限。
1. 单击&#x200B;**测试连接**。\
   您应该会看到一条消息，告诉您连接成功。

1. 单击&#x200B;**保存**。

## 使用其他身份提供程序

使用非Okta身份提供程序（例如Ping或Centrify）时，必须将Workfront元数据重新上传到您的身份提供程序。
