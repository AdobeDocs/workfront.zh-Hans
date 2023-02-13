---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0，安全，证书，管理员，免除，配置，元数据
navigation-topic: security
title: 续订Adobe Workfront SAML 2.0元数据证书
description: 此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 续订Adobe Workfront SAML 2.0元数据证书

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则无需执行任何操作。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront服务器使用SAML 2.0协议进行身份验证和授权。 更新后，新证书的有效期为一年。 当您需要在身份提供程序上续订证书时，您会在Workfront中收到一则警告，提醒您必须进行此更改。 作为Workfront管理员，您可以在系统级别管理此更改。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>如果贵组织的Workfront实例通过Adobe IMS启用，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

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

## 在Workfront中配置SAML 2.0

要查看警告消息并确认身份提供程序中SAML 2.0元数据的更新，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **单点登录**.

1. 在 **类型** 下拉菜单，选择 **SAML 2.0**.

1. 单击 **下载SAML 2.0元数据**.

   此操作将下载SAML 2.0的续订Workfront证书，该证书包含您服务器的正确元数据。

   >[!CAUTION]
   >
   >在步骤5中将Workfront元数据上传到单点登录(SSO)提供商之前，请将您当前的断言使用者服务(ACS)URL复制到一个安全的位置。 在您的SSO提供商的Workfront配置页面上，可找到此URL（也称为回复URL）。
   >
   >
   >如果您在上传Workfront元数据后ACS URL发生更改，则意味着元数据可能包含错误的ACS URL。 您必须将其更改回您复制的连接，以避免破坏您的单点登录连接。 执行此操作后，更新的证书仍然正确。

1. 转到您的身份提供程序服务器，并更新您下载的新证书。
1. 在Workfront，在 **单点登录(SSO)页面**，请确保选中此选项： **新的Workfront证书已上传到身份提供程序**.

   选择此字段后，Workfront管理员可以使用其SSO凭据或Workfront凭据登录Workfront。

1. 单击&#x200B;**保存**。

   警告消息不再显示，因为您已确认身份提供程序服务器上的SAML 2.0证书已续订。

1. 单击 **测试连接** 来测试您的配置。

   您应会看到一条消息，确认连接成功。

有关更多信息或有关手动配置元数据的帮助，请联系我们的支持团队，如 [联系客户支持](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
