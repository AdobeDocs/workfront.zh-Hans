---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 集成 [!DNL Workfront Proof] with [!DNL Basecamp]
description: 如果您使用 [!DNL Basecamp] 对于项目管理，您可以使用 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# 集成 [!DNL Workfront Proof] with [!DNL Basecamp]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您使用 [!DNL Basecamp] 对于项目管理，您可以使用 [!DNL Workfront Proof].

## 了解 [!DNL Basecamp] 与集成 [!DNL Workfront]

集成 [!DNL Basecamp] 允许用户在 [!DNL Basecamp]. 用户可以向 [!DNL Workfront Proof] 帐户，并将其与 [!DNL Basecamp] 项目。 您的审阅人可以通过 [!DNL Basecamp]，使用Basecamp消息中嵌入的mini校样。

与集成后 [!DNL Workfront Proof], [!DNL Basecamp] 具有以下校对功能：

* 用户可以在 [!DNL Basecamp Classic].
* 用户可随时查看可用的工具。
* 项目审阅团队会在 [!DNL Basecamp] 以小小的证据供审阅和批准。
* 用户可以切换到全页校样以进行审阅和批准。
* 用户可以向小型校样和全尺寸校样添加注释和标记。

   >[!NOTE]
   >
   >评论被回复后，便无法编辑或删除。

* 审阅人可以对其他审阅人创建的和标记做出响应。
* 当有新版本的校样可用时，用户会收到警报。
* 非 [!DNL Workfront Proof] 用户可以在中处理校样 [!DNL Basecamp].

集成 [!DNL Workfront Proof] with [!DNL Basecamp] 必须在两个级别上设置：

* 配置 [!DNL Basecamp] in [帐户设置：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 这可为您的整个组织启用Basecamp集成。 有关更多信息，请参阅 [启用Basecamp与 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* 配置 [!DNL Basecamp] in [个人设置](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):这样，校样创建者和所有者就可以连接到其个人Basecamp帐户并进行授权 [!DNL Workfront Proof] 访问权限。 有关更多信息，请参阅 [配置个人设置](#configuring-personal-settings).

您可以集成 [!DNL Workfront] 使用 [!DNL Basecamp] 或 [!DNL Basecamp Classic]. 每个版本 [!DNL Basecamp] 会使用不同的API，因此需要不同的配置过程。

有关配置的信息 [!DNL Basecamp Classic]，请参阅 [集成 [!DNL Workfront Proof] with [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## 启用 [!DNL Basecamp] 与集成 [!DNL Workfront Proof]

As a [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 或 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)，您可以设置 [!DNL Basecamp] 集成 [帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. 在 [!UICONTROL 巴塞坎普]，收集以下信息：

   * 您的URL [!DNL Basecamp] 帐户
   * 在“[!UICONTROL 我的信息]“ ”部分

1. 注销 [!DNL Basecamp].
1. 单击 **[!UICONTROL 帐户设置]** 在右上角附近。
1. 单击 **[!UICONTROL 集成]** 选项卡。
1. 在 **[!UICONTROL [!DNL Basecamp]]** 的 **[!UICONTROL [!DNL Basecamp]集成]**，单击 **[!UICONTROL 启用]**.

1. 旁边 **[!UICONTROL [!DNL Basecamp]版本]**，验证 **[!UICONTROL 经典版本]** 是您集成的版本。

1. （视情况而定）如果否 [!DNL Basecamp] 显示URL，单击 **[!UICONTROL 编辑]**，请键入 [!DNL Basecamp] 帐户(不含“http://”)，然后单击 **[!UICONTROL 保存]**.

1. 在窗口的右上角，单击 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**.

1. 单击 **[!UICONTROL 集成]** 选项卡。
1. 在 **[!DNL Basecamp]**，在 **[!UICONTROL Basecamp集成]**，单击 **[!UICONTROL 启用]**.

1. 在显示的选项右侧 **[!UICONTROL [!DNL Basecamp]API令牌]**，单击 **[!UICONTROL 编辑]**.

1. 在显示的框中，键入“[!UICONTROL 我的信息]“ ”部分 [!DNL Basecamp]，然后单击 **[!UICONTROL 保存]**.\
   集成后 [!DNL Workfront Proof] with [!DNL Basecamp]，则用户可以配置其个人设置。 有关设置个人设置的信息，请参阅 [配置个人设置](#configuring-personal-settings)

1. 如果无法启用 [!DNL Basecamp] 集成，您的 [!DNL Workfront Proof] 帐户ID可能与您在 [!DNL Basecamp].
1. 集成后 [!DNL Workfront Proof] with [!DNL Basecamp]，则用户可以配置其个人设置。 有关设置个人设置的信息，请参阅 [配置个人设置](#configuring-personal-settings).

## 配置个人设置

设置后 [帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 对于贵组织，创建/提交验证的每个作者都应设置  [个人设置。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. 转到 **[!UICONTROL 个人** &#x200B; **设置]**.

1. 打开 **[!UICONTROL 集成]** 选项卡(1)。
1. 启用 [!DNL Basecamp] 集成，单击 **[!UICONTROL 启用]** (2)。
1. 单击 **[!UICONTROL 连接到 [!DNL Basecamp] 帐户]** (3)。\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. 登录到 [!DNL Basecamp] 账号(1)。\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. 单击 **[!UICONTROL 是的，我允许访问]** 授权 [!DNL Workfront Proof] 访问您的帐户(2)。\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. （可选）当您的个人集成处于活动状态时(3)，您可以轻松地在 [!DNL Basecamp] 帐户。

   1. 单击 **[!UICONTROL 交换机 [!DNL Basecamp] 帐户]** (4)。\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      的 [!UICONTROL 交换机Basecamp帐户] 带你去 [!UICONTROL 个人设置] 页面，您可以在其中选择 [!DNL Basecamp] 要与您的 [!DNL Workfront Proof] 帐户。

   1. 单击 **[!UICONTROL 与[!DNL Basecamp]]** （五）在选择前 [!DNL Basecamp] 帐户\

      这会刷新 [!UICONTROL 个人设置] 页面，并显示您的最新列表 [!DNL Basecamp] 帐户。

   1. 单击 **[!UICONTROL 与此帐户集成]** 将其连接到 [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      您现在可以向 [!DNL Basecamp] 项目。
