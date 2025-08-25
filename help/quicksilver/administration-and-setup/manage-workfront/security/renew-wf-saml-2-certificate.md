---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0，安全性，证书，管理员，劐免，配置，元数据
navigation-topic: security
title: 续订Adobe Workfront SAML 2.0元数据证书
description: Adobe Workfront服务器利用SAML 2.0协议进行身份验证和授权。 更新后，新证书的有效期为一年。 轮到您在身份提供程序上续订证书时，Workfront中会显示一则警告，提醒您必须进行此更改。 作为Workfront管理员，您可以在系统级别管理此更改。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 续订Adobe Workfront SAML 2.0元数据证书

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入Admin Console的组织。 如果您的组织已载入到Adobe Admin Console，则无需执行任何操作。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

Adobe Workfront服务器利用SAML 2.0协议进行身份验证和授权。 更新后，新证书的有效期为一年。 轮到您在身份提供程序上续订证书时，Workfront中会显示一则警告，提醒您必须进行此更改。 作为Workfront管理员，您可以在系统级别管理此更改。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>如果您组织的Workfront实例已启用Adobe IMS，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

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
  <td> <p>新增：标准 </p>
 <p>或</p> 
<p>当前：计划 </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront中配置SAML 2.0

查看警告消息并确认您的身份提供程序中的SAML 2.0元数据的更新：

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **单点登录**。

1. 在&#x200B;**类型**&#x200B;下拉菜单中，选择&#x200B;**SAML 2.0**。

1. 单击&#x200B;**下载SAML 2.0元数据**。

   这将下载续订的Workfront SAML 2.0证书，其中包含您服务器的正确元数据。

1. 在您的身份提供商中，将您当前的断言消费者服务(ACS) URL（也称为回复URL）复制到安全位置。

   >[!CAUTION]
   >
   >在步骤6中将Workfront元数据上传到单点登录(SSO)提供商之前，请将当前断言客户服务(ACS) URL复制到安全位置。 此URL（也称为回复URL）可在您的SSO提供商的Workfront配置页面上找到。
   >
   >
   >如果您在上传Workfront元数据后ACS URL发生更改，这意味着元数据可能包含不正确的ACS URL。 您必须将其更改回复制的值，以避免破坏单点登录连接。 执行此操作后，您更新的证书仍将是正确的。

1. 在身份提供程序服务器中，更新下载的新证书。
1. （视情况而定）如果您的身份提供方中的断言客户服务(ACS) URL或回复URL已更改，请将其更改回您在步骤5中复制的URL。
1. 在Workfront的&#x200B;**单点登录(SSO)页面**&#x200B;上，确保选中此选项： **新的Workfront证书已上载到身份提供程序**。

   >[!NOTE]
   >
   >* 仅当满足以下所有条件时，此选项才可见：
   >   * 您的组织已为SAML 2.0进行了设置
   >   * 当前证书已准备好过期
   >   * 新证书可用
   >* 如果选择此字段，Workfront管理员可以使用其SSO凭据或Workfront凭据登录Workfront。

1. 单击&#x200B;**保存**。

   警告消息不再显示，因为您确认了在您的身份提供程序的服务器上续订了SAML 2.0证书。

1. 单击&#x200B;**测试连接**&#x200B;以测试您的配置。

   您应该会看到一条消息，确认连接成功。

有关详细信息或手动配置元数据的帮助，请联系我们的支持团队，如[联系客户支持](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)中所述。
