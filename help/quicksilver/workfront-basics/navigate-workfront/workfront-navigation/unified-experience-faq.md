---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe统一体验常见问题解答
description: 以下功能在 [!DNL Workfront] 和Adobe Experience Cloud，你可能有些问题 [!DNL Workfront] 实例将迁移到统一体验。
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] 常见问题解答

的 [!DNL Adobe Unified Experience] 表示 [!DNL Workfront] 允许您管理 [!DNL Adobe] 应用程序只需一次登录即可。 的 [!DNL Adobe] 导航区域与 [!DNL Workfront]. 一些功能不同，您可能会遇到一些问题，因为 [!DNL Workfront] 实例将迁移到统一体验。

有关如何登录的信息 [!DNL Adobe Unified Experience]，请参阅 [[!DNL Adobe Unified Experience] 表示 [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## 比较 [!DNL Adobe Unified Experience] 和 [!DNL Workfront only] 体验

仅使用 [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] 可以访问 [!DNL Adobe Unified Experience]. 尚未迁移的客户将看到 [!DNL Workfront only] 体验，而无法在 [!DNL Adobe] 应用程序。

此表介绍了这两种体验之间的一些不同功能。

| [!DNL Adobe Unified Experience] | [!DNL Workfront] 仅体验 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] 主菜单] 在左侧 ![主菜单](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] 主菜单] 在右侧 ![主菜单](assets/main-menu-icon.png) |
| 单个登录URL可供所有人使用 [!DNL Adobe Experience Cloud] 应用程序 | 登录到 [!DNL Workfront] 自定义 [!DNL Workfront] URL |
| 通过“组织切换器”，您可以在 [!DNL Workfront] 组织和环境 | “组织切换器”不可用 |
| 导航包括 [!DNL Adobe] 产品， [!DNL Adobe] 通知、帮助和用户配置文件，以及 [!DNL Workfront] 导航栏 | 导航包括 [!DNL Workfront] 仅限导航栏 |
| 可通过访问 [!UICONTROL 主菜单] 和顶部导航区域 | 可通过访问 [!UICONTROL 主菜单] 和 [!DNL Workfront] 导航栏 |

{style=&quot;table-layout:auto&quot;}

## 常见问题解答

**如何进一步了解 [!DNL Adobe Admin Console]?**

有关 [!DNL Admin Console]，请查看以下文章：

* [为 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)

**作为客户，我需要采取哪些措施来促进迁移？**

将联系现有客户以计划迁移。 迁移团队支持同事将引导客户完成该过程，并提供相关建议 [!DNL Admin Console] 设置，并提供所需文档的链接，以便尽可能简单、轻松地完成移动。

* [[!DNL Adobe Workfront] 支持概述](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] 信息](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] and [!DNL Admin Console] 常见问题解答](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

**您的处理方式 [!DNL Adobe Admin Console] 对于已启用此功能的公司，联合ID的使用方式与 [!DNL Workfront] SSO已设置？**

[!DNL Adobe Admin Console] 可选择包含 [!DNL Workfront]，将单点登录替换为IMS。 所有用户配置均在 [!DNL Admin Console]，用户将看到 [!DNL Adobe] 登录屏幕 [!DNL Experience Cloud] 他们将看到什么地方 [!DNL Workfront] 作为选项（如果他们被授予访问权限）。

**这对已具有AEM管理面板的客户有何影响 [!DNL Adobe Assets]  — 但SSO的配置方式与[!DNL Workfront?]**

一次 [!DNL Workfront] 作为 [!DNL Admin Console] 应用程序时，您不应为 [!DNL Workfront] 利用您现有的SSO设置 [!DNL Adobe Assets].

**这对使用单点登录(SSO)设置的用户有何影响？**

SSO是在 [!DNL Admin Console] 并由 [!DNL Workfront] 应用程序。

**是SSO与我们的内部 [!DNL Active Directory] 还是IMS的选项？**

IMS是SSO的替代方法，其功能基本相同。 在中授予和配置了所有用户权限 [!DNL Adobe Admin Console]，用户将看到 [!DNL Adobe] 登录屏幕，可在其中选择“[!UICONTROL 个人帐户]&quot;或&quot;[!UICONTROL 公司帐户]“ ”登录(如果 [!DNL Active Directory]，大多数客户将使用公司帐户登录)。

**对于未使用单点登录(SSO)的用户， [!DNL Workfront] 登录URL是否发生更改？**

登录URL将发生更改；但是，旧URL将重定向到新的登录URL，因此您应该重新培训用户以前往何处。

**我们设置的别名是否仍然有效，或者 [!DNL Workfront] 随此迁移而发生更改的链接？**

[!DNL Workfront] 可以使用重定向/别名访问主页。

**是否会有时间禁用重定向？ 或者，我们将始终能够在my.company.workfront.com中键入内容？**

您将始终能够使用任何自定义URL。 单击其中任意链接后，该链接会将您定向到 [!DNL Workfront] 和显示其他URL。 但是，这样更好 [!DNL experience] 登录experience.adobe.com，并将链接加入书签 [!DNL Experience Cloud]. 重定向越少，延迟时间/加载时间就越少。

**指向请求队列的直接链接是否会被断开？**

所有直接链接都应重定向到新的URL模式。 但是，如果您已经向人员分发了链接，则应发送更新以利用直接链接，并防止在访问预期页面时出现延迟。

**我们是否会迁移到 [!DNL Experience Cloud] 我们是否可以在全球范围内选择特定用户(并非所有用户都使用其他Adobe产品)?**

整个 [!DNL Workfront] 将迁移客户帐户。 无法按用户执行此操作。

**全部 [!DNL Workfront] 用户必须通过 [!DNL Experience Cloud]? 还是只是管理员？**

是，所有用户都将通过登录 [!DNL Experience Cloud]. IMS登录将替换SSO。 体验非常相似，只是不同的登录屏幕。

**用户是否必须关联 [!DNL Adobe] 帐户 [!DNL Workfront] 帐户（如果它们已同时具有两者）？**

是，这是一个过程，当您的组织需要迁移到IMS时，将提供更多详细信息。

**对 [!DNL Workfront] 没有 [!DNL Adobe] 帐户？**

未在 [!DNL Adobe Admin Console] 进入 [!DNL Workfront] 必须创建“[!UICONTROL 个人帐户]&quot;或 [!DNL Adobe] ID帐户。 这会向管理员发送一封电子邮件以批准或拒绝其请求，并且还允许管理员配置用户拥有的访问类型。 登录后，访客将转到experience.adobe.com，输入其电子邮件地址，然后选择 [!UICONTROL 个人帐户]. 从那里，他们将能够访问 [!DNL Workfront].

**如果我们没有 [!DNL Adobe] 产品除外[!DNL Workfront?]**

仍建议贵组织迁移到 [!DNL Adobe Unified Experience]. 您将收到 [!DNL Adobe] ID以及上面列出的优势。

**我们的 [!DNL Workfront] 实例。 我们不希望他们有权访问 [!DNL Adobe]. 我们如何限制他们在控制台中的访问权限？**

[!DNL Admin Console] 可让管理员对用户可以访问和无法访问的内容有很大控制权。 当外部用户想要访问时，他们需要创建 [!DNL Adobe] ID，用于向管理员发送电子邮件。 然后，管理员可以接受或拒绝对某个产品的访问，并定义他们对该组织拥有的产品可以/不能访问的权限。 然后， [!DNL Workfront] 系统管理员可以进入 [!UICONTROL 用户] 面积 [!DNL Workfront] ，以便为外部用户提供更细粒度的权限。

**组管理员用于在 [!DNL Workfront]. 移动到 [!DNL Experience Cloud]，组管理员是否仍能创建人员？**

是的，仍可以通过 [!DNL Workfront]. 这些用户可以添加到 [!DNL Experience Cloud] 自动。 您还可以在 [!DNL Admin Console] 允许他们分配 [!DNL Workfront] 到用户。

**切换到的截止时间是多长 [!DNL Experience Cloud]?**

目前没有截止日期要迁移到 [!DNL Adobe Experience Cloud]. 我们与客户合作，让客户在准备就绪时进行选择。

**我们的支持团队是否需要为此更改执行任何操作？**

如果支持团队负责创建新用户，则他们需要熟悉 [!DNL Admin Console] 用于创建用户并将权限分配给Workfront的界面。 否则，您的内部支持团队可能不会发生任何重大更改。

**这对通过API函数进行的集成有何影响？**

现有的URL路径将继续可用于API流量。 您无需执行任何操作即可更新集成中的端点。 但是，不支持通过用户名和密码直接登录 — 您必须使用API密钥，但是 [!DNL Workfront Fusion] 连接器。

**那 [!DNL Creative Cloud] 用户？ 迁移会对他们有何影响？ 他们有什么好处吗？**

对 [!DNL Creative Cloud] 迁移到的用户 [!DNL Adobe Unified Experience].

**登录将更改 [!DNL Workfront] 移动用户？**

[!DNL Workfront] 移动设备用户不应受到迁移到的影响 [!DNL Adobe Unified Experience].
