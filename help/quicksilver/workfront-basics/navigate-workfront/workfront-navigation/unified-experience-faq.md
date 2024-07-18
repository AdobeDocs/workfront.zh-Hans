---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe统一Experience常见问题解答
description: ' [!DNL Workfront] 和Adobe Experience Cloud的一些功能不同，在将 [!DNL Workfront] 实例迁移到统一体验时，您可能会遇到一些问题。'
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience]常见问题解答

[!DNL Workfront]的[!DNL Adobe Unified Experience]允许您在单一登录位置管理所有[!DNL Adobe]应用程序。 [!DNL Adobe]导航区域与[!DNL Workfront]无缝集成。 一些功能不同，在将[!DNL Workfront]实例迁移到统一体验时，您可能会有一些问题。

有关如何登录到[!DNL Adobe Unified Experience]的信息，请参阅 [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)的[[!DNL Adobe Unified Experience] 。

## [!DNL Adobe Unified Experience]和[!DNL Workfront only]体验的比较

只有使用[!DNL Adobe Business Platform] / [!DNL Adobe Admin Console]的客户才能访问[!DNL Adobe Unified Experience]。 尚未迁移的客户将看到[!DNL Workfront only]体验，无法在[!DNL Adobe]应用程序之间切换。

此表介绍了两种体验之间的一些不同功能。

| [!DNL Adobe Unified Experience] | 仅[!DNL Workfront]体验 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront]主菜单]位于左侧![主菜单](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront]主菜单]位于右侧![主菜单](assets/main-menu-icon.png) |
| 单个登录URL可用于所有[!DNL Adobe Experience Cloud]应用程序 | 使用自定义[!DNL Workfront] URL登录到[!DNL Workfront] |
| “组织切换器”允许您在[!DNL Workfront]组织和环境之间移动 | “组织切换器”不可用 |
| 导航除[!DNL Workfront]导航栏外，还包括[!DNL Adobe]产品、[!DNL Adobe]通知、帮助和您的用户配置文件的顶级导航区域 | 导航仅包括[!DNL Workfront]导航栏 |
| 可通过[!UICONTROL 主菜单]和顶部导航区域访问帮助 | 可通过[!UICONTROL 主菜单]和[!DNL Workfront]导航栏访问帮助 |

{style="table-layout:auto"}

## 常见问题解答

### 如何确定我使用的是AdobeUnified Experience还是Adobe Workfront？

要确定您的组织是否位于Unified ExperienceAdobe上，请检查用于访问Workfront的URL。

| URL | Adobe体验 |
|------------|------------|
| （公司名称）.my.workfront.com | Workfront体验 |
| experience.adobe.com | AdobeUnified Experience |

### 如何了解有关[!DNL Adobe Admin Console]的更多信息？

有关[!DNL Admin Console]的信息，请查看以下文章：

* [准备 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)

### 作为客户，我需要做什么来促进迁移？

将与现有客户联系以安排迁移。 迁移团队支持同事将引导客户完成该过程，提出[!DNL Admin Console]设置的建议，并提供所需的文档链接以使迁移尽可能简单和轻松。

* [[!DNL Adobe Workfront] 支持概述](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] 信息](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] 和 [!DNL Admin Console] 常见问题解答](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### 对于已为Federated ID启用此选项与设置[!DNL Workfront] SSO不同的公司，您如何处理[!DNL Adobe Admin Console]？

[!DNL Adobe Admin Console]可以选择包含[!DNL Workfront]，将SSO替换为IMS。 所有用户设置都在[!DNL Admin Console]中进行，用户将看到[!DNL Adobe]登录屏幕以访问[!DNL Experience Cloud]，他们将在其中看到[!DNL Workfront]作为选项（如果他们被授予访问权限）。

### 这对已具有[!DNL Adobe Assets]的AEM管理面板的客户有何影响 — 但SSO的配置方式与[!DNL Workfront?]不同

将[!DNL Workfront]添加为[!DNL Admin Console]应用程序后，您无需为[!DNL Workfront]执行任何其他操作即可利用您为[!DNL Adobe Assets]执行的现有SSO设置。

### 这如何影响使用SSO设置的用户？

SSO在[!DNL Admin Console]中设置，并由[!DNL Workfront]应用程序继承。

### 我们的内部[!DNL Active Directory]的SSO是否仍是IMS的一个选项？

IMS是SSO的替代品，其功能大致相同。 所有用户权限都在[!DNL Adobe Admin Console]中授予并设置，用户将看到[!DNL Adobe]登录屏幕，他们可以在其中选择“[!UICONTROL 个人帐户]”或“[!UICONTROL 公司帐户]”登录（如果您有[!DNL Active Directory]，则大多数登录将使用公司帐户）。

### 对于未使用SSO的用户，[!DNL Workfront]登录URL是否会发生更改？

登录URL将更改；但是，旧URL将重定向到新登录URL，因此您应该重新培训用户转到何处。

### 我们设置的别名是否仍然有效，或者[!DNL Workfront]链接是否将随此迁移而更改？

有[!DNL Workfront]个重定向/别名可用于访问主页。

### 是否将会禁用重定向？ 或者，我们始终能够键入my.company.workfront.com吗？

您将始终可以使用任何自定义URL。 单击其中的任何链接后，它将引导您转到[!DNL Workfront]并显示其他URL。 但是，最好是[!DNL experience]登录到experience.adobe.com，并将链接从[!DNL Experience Cloud]内加入书签。 更少的重定向等于更少的延迟时间/加载时间。

### 到请求队列的直接链接是否会断开？

所有直接链接都应重定向到新的URL模式。 但是，如果您已将链接分发给人员，则应发送更新以利用直接链接，并防止在到达预期页面时出现延迟。

### 我们会全局迁移到[!DNL Experience Cloud]吗？还是可以为某些用户(并非所有用户都使用其他Adobe产品)选择？

将迁移整个[!DNL Workfront]客户帐户。 无法逐个用户执行此操作。

### 所有[!DNL Workfront]用户都必须通过[!DNL Experience Cloud]登录吗？ 还是只是管理员？

是，所有用户都将通过[!DNL Experience Cloud]登录。 IMS登录将替换SSO。 这是非常相似的体验，只是登录屏幕不同。

### 如果用户已经同时拥有其[!DNL Adobe]帐户和[!DNL Workfront]帐户，用户是否必须将其帐户关联到这两个帐户？

是，有一个针对此问题的流程，当您的组织需要迁移到IMS时，将会提供更多详细信息。

### 没有[!DNL Adobe]帐户的[!DNL Workfront]用户会发生什么情况？

未在[!DNL Adobe Admin Console]中授予访问[!DNL Workfront]权限的用户必须创建“[!UICONTROL 个人帐户]”或[!DNL Adobe] ID帐户才能登录。 这会向管理员发送一封电子邮件，以批准或拒绝他们的请求，并且管理员还可以配置该用户具有的访问权限类型。 登录时，他们将转到experience.adobe.com，输入电子邮件地址，然后选择[!UICONTROL 个人帐户]。 他们将从此处访问[!DNL Workfront]。

### 如果我们没有[!DNL Workfront?]以外的任何[!DNL Adobe]产品，该怎么办

仍建议将您的组织迁移到[!DNL Adobe Unified Experience]。 您将收到[!DNL Adobe] ID以及上面列出的好处。

### 我们的[!DNL Workfront]实例中包含外部用户。 我们不希望他们有权访问[!DNL Adobe]中包含的任何其他产品。 我们如何限制他们在控制台中的访问？

[!DNL Admin Console]让管理员能够充分控制用户可以访问和无法访问的内容。 每当外部用户想要访问时，他们需要创建一个[!DNL Adobe] ID，以向管理员发送电子邮件。 然后，管理员可以接受或拒绝对产品的访问权限，并定义他们可以/无法访问该组织所拥有产品的内容。 然后，[!DNL Workfront]系统管理员可以进入[!DNL Workfront]的[!UICONTROL 用户]区域，为外部用户设置更细粒度的权限。

### 组管理员用于在[!DNL Workfront]中创建人员。 迁移到[!DNL Experience Cloud]后，组管理员是否仍能够创建人员？

是，仍可以通过[!DNL Workfront]创建用户。 这些用户可自动添加到[!DNL Experience Cloud]。 您还可以在[!DNL Admin Console]中将您的组管理员设置为产品所有者，以允许他们将[!DNL Workfront]分配给用户。

### 切换到[!DNL Experience Cloud]的截止日期是多少？

目前没有移至[!DNL Adobe Experience Cloud]的截止日期。 我们正在与客户合作，让他们选择何时可以迁移。

### 我们的支持团队是否需要为此更改执行任何操作？

如果支持团队负责创建新用户，则需要熟悉用于创建用户并向Workfront分配权利的[!DNL Admin Console]界面。 否则，您的内部支持团队可能不会发生重大变化。

### 这对我们通过API功能实现的集成有何影响？

现有的URL路径将继续可用于API流量。 您无需执行任何操作即可更新集成中的端点。 但是，不支持通过用户名和密码直接登录 — 您必须使用API密钥，但[!DNL Workfront Fusion]连接器除外。

### [!DNL Creative Cloud]用户呢？ 迁移对它们有何影响？ 这对他们有什么好处吗？

迁移到[!DNL Adobe Unified Experience]对[!DNL Creative Cloud]用户没有影响。

### [!DNL Workfront]移动用户的登录次数是否会发生变化？

迁移到[!DNL Adobe Unified Experience]不应影响[!DNL Workfront]移动用户。
