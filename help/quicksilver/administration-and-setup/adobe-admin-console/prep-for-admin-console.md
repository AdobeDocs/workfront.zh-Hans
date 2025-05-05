---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 准备将您的组织载入Adobe Admin Console
description: 由于Adobe Workfront是一种Adobe产品，因此您可以通过Adobe Admin Console访问它。 这使您能够在一个中心位置为用户管理Workfront以及其他Adobe帐户和产品。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# 准备将您的组织载入Adobe Admin Console

<!-- Audited: 12/2023 -->

由于Adobe Workfront是一种Adobe产品，因此您可以通过Adobe Admin Console访问它。 这使您能够在一个中心位置为用户管理Workfront以及其他Adobe帐户和产品。

所有Workfront客户最终都将移至Adobe Admin Console。 贵组织迁移到Adobe Admin Console后，Workfront身份验证由控制台管理。 为这一转变做好准备并提早行动，为提高工作管理效率奠定基础，并使您的组织能够在未来更快创新

有关Adobe Admin Console的概述，请参阅[Admin Console概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)。

## 迁移核对清单

要确保您的组织可以迁移到Adobe Admin Console，您必须执行以下操作。

1. 确定要在其中添加Workfront的所需Adobe Admin Console。

   * 如果您的组织没有现有的Adobe Admin Console，或者您不想使用现有的Adobe Admin Console，Workfront支持可以帮助您创建新的存储库。

   * 如果您有多个AdobeAdmin Console，并且不确定哪个页面最适合将Workfront添加到，请联系Workfront支持部门。

1. 通过Workfront支持确认您要使用现有Adobe Admin Console，或创建一个新帐户。

1. 在Adobe Admin Console上设置身份管理。

   >[!IMPORTANT]
   >
   >请准备好与Workfront支持人员和您的IT团队就身份验证首选项(例如单点登录(SSO)或非SSO)进行交谈。

   有关说明，请参阅[Adobe Admin Console部署指南](https://helpx.adobe.com/cn/enterprise/using/deployment-planning.html)的Identity Management部分。

1. （视情况而定）如果使用单点登录，请将新的Adobe Admin Console连接到您现有的SSO提供商。

   有关更多信息和说明，请参阅[设置标识](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html)。

   >[!NOTE]
   >
   >如果您的组织不使用单点登录，则任何迁移到Adobe Admin Console的用户都将收到一封电子邮件，用于创建其帐户和密码。

1. 确保用户电子邮件地址准备好进行迁移：

   1. 从Workfront中删除重复的电子邮件。

      有关说明，请参阅[防止重复用户](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md)中的[更新Workfront实例中现有用户的电子邮件地址](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance)。

      如果您的组织中存在重复的电子邮件地址，则由电子邮件地址表示的最新`lastLoginDate`用户将被移动到Adobe Admin Console组织。 将停用使用该电子邮件地址的任何其他用户。

      >[!NOTE]
      >
      >由于在给定时间只能有一个具有给定电子邮件地址的用户处于活动状态，因此，如果您需要激活另一个与当前活动用户具有相同电子邮件地址的用户，则必须先停用当前活动用户，然后再激活已停用的用户。

   1. （视情况而定）如果您使用的是自定义API集成，请确认这些用户具有他们可以访问的有效电子邮件地址。

   1. （可选）我们建议停用任何不再需要访问Workfront的用户，以便他们不会添加到Adobe Admin Console。

   >[!IMPORTANT]
   >
   >在贵组织开始迁移到Adobe Admin Console之前，必须完成这些有关用户电子邮件的操作。

1. （可选）更新所有自定义集成以使用OAuth2。

   有关设置OAuth2集成的说明，请参阅[为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)。

   >[!NOTE]
   >
   >此步骤是可选的，但强烈建议您执行此步骤，因为未来将弃用其他形式的API身份验证和授权。

使用Workfront配置Adobe Admin Console后，您可以用它来创建Workfront系统管理员。

有关详细信息，请参阅[在Adobe Admin Console中管理用户](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

有关根据贵组织是否已登记到Adobe Admin Console而不同的其他操作的列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
