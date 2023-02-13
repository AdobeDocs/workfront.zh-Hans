---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 准备将您的组织载入Adobe Admin Console
description: 由于Adobe Workfront是Adobe产品，因此您可以通过Adobe Admin Console访问它。 这样，您就可以在一个中心位置管理Workfront以及其他Adobe帐户和产品。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 准备将您的组织载入Adobe Admin Console

由于Adobe Workfront是Adobe产品，因此您可以通过Adobe Admin Console访问它。 这样，您就可以在一个中心位置管理Workfront以及其他Adobe帐户和产品。

最终，所有Workfront客户都将迁移到Adobe Admin Console。 在贵组织迁移到Adobe Admin Console后，Workfront身份验证由Adobe Admin Console管理。 尽早准备和实施此项举措为工作管理的效率奠定了基础，并使您的组织能够在未来更快地进行创新

有关Adobe Admin Console的概述，请参阅 [Admin Console概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html).

## 迁移核对清单

要确保贵组织可以迁移到Adobe Admin Console，您必须执行以下操作

1. 确定要在其中添加Adobe Admin Console的所需Workfront。

   * 如果贵组织没有现有Adobe Admin Console，或者如果您不想使用现有Adobe Admin Console,Workfront支持团队可以协助您创建新的。

   * 如果您有多个AdobeAdmin Console，并且不确定最适合将Adobe Workfront添加到的Workfront，请联系支持。

1. 通过Workfront支持确认您要使用现有Adobe Admin Console，或者已创建新的。

1. 在Adobe Admin Console上设置身份管理。

   >[!IMPORTANT]
   >
   >准备就身份验证首选项(如单点登录(SSO)或非单点登录)与Workfront支持团队和您的IT团队进行沟通。

   有关说明，请参阅《Adobe Admin Console部署指南》(https://helpx.adobe.com/enterprise/using/deployment-planning.html)的Identity Management部分。

1. （视情况而定）如果使用单点登录，请将新的Adobe Admin Console连接到您现有的SSO提供商

   有关更多信息和说明，请参阅 [设置标识](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >如果贵组织不使用单点登录，则迁移到Adobe Admin Console的任何用户都将收到一封电子邮件，用于创建其帐户和密码。

1. 确保用户电子邮件地址已准备好进行迁移：

   1. 从Workfront中删除重复的电子邮件

      有关说明，请参阅防止重复用户中的更新Workfront实例中现有用户的电子邮件地址。

      如果贵组织中存在重复的电子邮件地址，则用户代表的电子邮件地址为 `lastLoginDate` 将被移至Adobe Admin Console组织。 具有该电子邮件地址的任何其他用户都将被停用。

      >[!NOTE]
      >
      >由于给定时间只有一个具有给定电子邮件地址的用户可以处于活动状态，因此如果您需要激活另一个与当前活动用户具有相同电子邮件地址的用户，则必须先停用当前活动用户，然后再激活已停用的用户。

   2. （视情况而定）如果您使用自定义API集成，请确认这些用户拥有他们可以访问的有效电子邮件地址。

   3. （可选）我们建议取消激活任何不再需要访问Workfront的用户，以便不要将他们添加到Adobe Admin Console。
   >[!IMPORTANT]
   >
   >在贵组织开始迁移到Adobe Admin Console之前，有关用户电子邮件的这些操作必须完成。

1. （可选）更新所有自定义集成以使用OAuth2。

   有关设置OAuth2集成的说明，请参阅 [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   创建OAuth2集成仅在新的Workfront体验中可用。

   >[!NOTE]
   >
   >此步骤是可选的，但强烈建议执行，因为其他形式的API身份验证和授权将来会被弃用。

使用Workfront配置Adobe Admin Console后，即可使用它来管理用户。

有关更多信息，请参阅 [在Adobe Admin Console中管理用户](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

有关根据贵组织是否已载入Adobe Admin Console而不同的其他操作列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
