---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: AdobeUnified Experience常见问题解答
description: 以下几项功能有所不同 [!DNL Workfront] 和Adobe Experience Cloud，您可能会有一些问题 [!DNL Workfront] 实例将迁移到统一体验。
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] 常见问题解答

此 [!DNL Adobe Unified Experience] 对象 [!DNL Workfront] 允许您管理所有 [!DNL Adobe] 应用程序只需一次登录即可在一个位置。 此 [!DNL Adobe] 导航区域与无缝集成 [!DNL Workfront]. 一些功能是不同的，您可能会有一些问题，例如 [!DNL Workfront] 实例将迁移到统一体验。

有关如何登录到 [!DNL Adobe Unified Experience]，请参见 [[!DNL Adobe Unified Experience] 对象 [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## 比较 [!DNL Adobe Unified Experience] 和 [!DNL Workfront only] 体验

仅使用 [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] 可以访问 [!DNL Adobe Unified Experience]. 尚未迁移的客户将看到 [!DNL Workfront only] 体验，无法在这两种体验之间切换 [!DNL Adobe] 应用程序。

此表介绍了两种体验之间的一些不同功能。

| [!DNL Adobe Unified Experience] | [!DNL Workfront] 仅体验 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] 主菜单] 在左侧 ![主菜单](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] 主菜单] 在右侧 ![主菜单](assets/main-menu-icon.png) |
| 所有用户都可以使用单个登录URL [!DNL Adobe Experience Cloud] 应用程序 | 登录 [!DNL Workfront] 带有自定义 [!DNL Workfront] URL |
| “组织切换器”允许您在 [!DNL Workfront] 组织和环境 | “组织切换器”不可用 |
| 导航包括顶层导航区域，用于 [!DNL Adobe] 产品、 [!DNL Adobe] 通知、帮助和您的用户配置文件，以及 [!DNL Workfront] 导航栏 | 导航包括 [!DNL Workfront] 仅导航栏 |
| 可通过以下方式访问帮助 [!UICONTROL 主菜单] 和顶部导航区域 | 可通过以下方式访问帮助 [!UICONTROL 主菜单] 和 [!DNL Workfront] 导航栏 |

{style="table-layout:auto"}

## 常见问题解答

### 如何确定我使用的是AdobeUnified Experience还是Adobe Workfront？

要确定您的组织是否位于Unified ExperienceAdobe上，请检查用于访问Workfront的URL。

| URL | Adobe体验 |
|------------|------------|
| （公司名称）.my.workfront.com | Workfront体验 |
| experience.adobe.com | AdobeUnified Experience |

### 如何进一步了解 [!DNL Adobe Admin Console]？

欲知关于 [!DNL Admin Console]，请查看以下文章：

* [准备好 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 概述](https://helpx.adobe.com/cn/enterprise/using/admin-console.html)

### 作为客户，我需要做什么来促进迁移？

将与现有客户联系以安排迁移。 迁移团队支持同事将引导客户完成该过程，并提供以下建议 [!DNL Admin Console] 设置，并提供所需的文档链接，以尽可能简化移动和避免麻烦。

* [[!DNL Adobe Workfront] 支持概述](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] 信息](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] 和 [!DNL Admin Console] 常见问题解答](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### 你的处境 [!DNL Adobe Admin Console] 适用于已经为Federated ID启用此功能的公司 [!DNL Workfront] 设置了SSO？

[!DNL Adobe Admin Console] 具有包含的选项 [!DNL Workfront]，将SSO替换为IMS。 所有用户预配都发生在中 [!DNL Admin Console]，用户将看到 [!DNL Adobe] 登录屏幕以访问 [!DNL Experience Cloud] 他们将看到的位置 [!DNL Workfront] 作为选项（如果授予他们访问权）。

### 这对已拥有AEM管理面板的客户有何影响 [!DNL Adobe Assets]  — 但SSO的配置方式与 [!DNL Workfront?]

一次 [!DNL Workfront] 添加为 [!DNL Admin Console] 应用程序，您不必为任何其他操作 [!DNL Workfront] 要利用您为使用的现有SSO设置 [!DNL Adobe Assets].

### 这如何影响使用SSO设置的用户？

SSO设置于 [!DNL Admin Console] 并由 [!DNL Workfront] 应用程序。

### SSO与我们的内部 [!DNL Active Directory] 仍将是使用IMS的一个选项？

IMS是SSO的替代品，其功能大致相同。 所有用户权限均在中授予和设置 [!DNL Adobe Admin Console]，用户将会看到 [!DNL Adobe] 登录屏幕，用户可在其中选择»[!UICONTROL 个人帐户]”或“[!UICONTROL 公司帐户]”以登录(如果您拥有 [!DNL Active Directory]，大多数登录帐户为公司帐户)。

### 对于未使用SSO的客户， [!DNL Workfront] 登录URL更改？

登录URL将更改；但是，旧URL将重定向到新登录URL，因此您应该重新培训用户转到何处。

### 我们设置的别名是否仍然有效，或者 [!DNL Workfront] 链接会随此迁移而更改？

[!DNL Workfront] 重定向/别名可用于访问主页。

### 是否将会禁用重定向？ 或者，我们始终能够键入my.company.workfront.com吗？

您将始终可以使用任何自定义URL。 单击其中的任何链接后，均会将您定向到 [!DNL Workfront] 和显示其他URL。 不过，这样更好 [!DNL experience] 登录experience.adobe.com，并将中的链接加入书签 [!DNL Experience Cloud]. 更少的重定向等于更少的延迟时间/加载时间。

### 到请求队列的直接链接是否会断开？

所有直接链接都应重定向到新的URL模式。 但是，如果您已将链接分发给人员，则应发送更新以利用直接链接，并防止在到达预期页面时出现延迟。

### 我们是否会迁移到 [!DNL Experience Cloud] 全球范围内还是我们可以为某些用户(并非所有用户都使用其他Adobe产品)进行选择？

整个 [!DNL Workfront] 将迁移客户帐户。 无法逐个用户执行此操作。

### 全部将 [!DNL Workfront] 用户必须通过登录 [!DNL Experience Cloud]？ 还是只是管理员？

是，所有用户将通过以下方式登录： [!DNL Experience Cloud]. IMS登录将替换SSO。 这是非常相似的体验，只是登录屏幕不同。

### 用户是否必须关联其 [!DNL Adobe] 帐户至其 [!DNL Workfront] 帐户（如果他们已经拥有这两个帐户）？

是，有一个针对此问题的流程，当您的组织需要迁移到IMS时，将会提供更多详细信息。

### 将发生什么情况 [!DNL Workfront] 没有 [!DNL Adobe] 帐户？

在中未被授予访问权限的用户 [!DNL Adobe Admin Console] 以进入 [!DNL Workfront] 必须创建“”[!UICONTROL 个人帐户]”或 [!DNL Adobe] 能够登录的ID帐户。 这会向管理员发送一封电子邮件，以批准或拒绝他们的请求，并且管理员还可以配置该用户具有的访问权限类型。 登录时，他们将转到experience.adobe.com ，输入其电子邮件地址，然后选择 [!UICONTROL 个人帐户]. 从那里，他们将能够访问 [!DNL Workfront].

### 如果我们没有 [!DNL Adobe] 产品(不包括 [!DNL Workfront?]

仍建议贵组织迁移到 [!DNL Adobe Unified Experience]. 您将会收到 [!DNL Adobe] ID以及上面列出的好处。

### 我们的中纳入了外部用户 [!DNL Workfront] 实例。 我们不希望他们有权访问中包含的任何其他产品 [!DNL Adobe]. 我们如何限制他们在控制台中的访问？

[!DNL Admin Console] 可让管理员在很大程度上控制用户可以访问和无法访问的内容。 每当外部用户希望访问时，他们需要创建 [!DNL Adobe] ID，可向管理员发送电子邮件。 然后，管理员可以接受或拒绝对产品的访问权限，并定义他们可以/无法访问该组织所拥有产品的内容。 然后， [!DNL Workfront] 系统管理员可以访问 [!UICONTROL 用户] 面积 [!DNL Workfront] 为外部用户设置更细粒度的权限。

### 组管理员用于在以下位置创建人员： [!DNL Workfront]. 迁移到 [!DNL Experience Cloud]，组管理员是否仍能够创建人员？

是，仍可通过以下方式创建用户 [!DNL Workfront]. 这些用户可添加到 [!DNL Experience Cloud] 自动。 您还可以将组管理员设置为中的产品所有者 [!DNL Admin Console] 以允许他们分配 [!DNL Workfront] 给用户。

### 切换到的截止日期为 [!DNL Experience Cloud]？

目前没有移至的截止日期 [!DNL Adobe Experience Cloud]. 我们正在与客户合作，让他们选择何时可以迁移。

### 我们的支持团队是否需要为此更改执行任何操作？

如果支持团队负责创建新用户，则他们将需要熟悉 [!DNL Admin Console] 用于创建用户和将权利分配给Workfront的界面。 否则，您的内部支持团队可能不会发生重大变化。

### 这对我们通过API功能实现的集成有何影响？

现有的URL路径将继续可用于API流量。 您无需执行任何操作即可更新集成中的端点。 但是，不支持通过用户名和密码直接登录 — 您必须使用API密钥，例外情况是 [!DNL Workfront Fusion] 连接器。

### 那又如何 [!DNL Creative Cloud] 用户？ 迁移对它们有何影响？ 这对他们有什么好处吗？

没有影响 [!DNL Creative Cloud] 迁移到的用户 [!DNL Adobe Unified Experience].

### 登录次数将更改 [!DNL Workfront] 移动用户？

[!DNL Workfront] 移动用户应该不会受到迁移到的影响 [!DNL Adobe Unified Experience].
