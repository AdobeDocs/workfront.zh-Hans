---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 将 [!DNL Workfront Proof] 与 [!DNL Basecamp]集成
description: 如果您使用 [!DNL Basecamp] 进行项目管理，则可以使用 [!DNL Workfront Proof]为项目团队提供更丰富的审核和批准工具。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# 将[!DNL Workfront Proof]与[!DNL Basecamp]集成

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果您将[!DNL Basecamp]用于项目管理，则可以使用[!DNL Workfront Proof]为项目团队提供更丰富的审阅和批准工具。

## 了解[!DNL Basecamp]与[!DNL Workfront]的集成

与[!DNL Basecamp]集成允许用户在[!DNL Basecamp]内查看、审阅和批准所有验证。 用户可以向您的[!DNL Workfront Proof]帐户提交验证，并将其与您的[!DNL Basecamp]项目连接。 您的审阅人可以使用Basecamp邮件中嵌入的小型校对，通过[!DNL Basecamp]进行评论和决策。

与[!DNL Workfront Proof]集成后，[!DNL Basecamp]具有以下校对功能：

* 用户可以在[!DNL Basecamp Classic]内查看和批准验证。
* 用户可以随时使用审阅工具。
* 项目审阅团队在[!DNL Basecamp]中收到一封邮件，其中包含用于审阅和批准的小型校对。
* 用户可以切换到整页验证以供审阅和审批。
* 用户可以在小型和全尺寸校样中添加注释和标记。

  >[!NOTE]
  >
  >评论回复后，便无法编辑或删除。

* 审阅人可以对其他审阅人所做的和标记做出响应。
* 当有新版本的验证可用时，用户会收到警报。
* 非[!DNL Workfront Proof]用户的用户可以在[!DNL Basecamp]中处理验证。

[!DNL Workfront Proof]与[!DNL Basecamp]的集成必须在两个级别上设置：

* 在[帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中配置[!DNL Basecamp]这将启用整个组织的Basecamp集成。 有关详细信息，请参阅[启用Basecamp与 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof)的集成。

* 在[个人设置](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)中配置[!DNL Basecamp]：这使验证创建者和所有者能够连接到其个人Basecamp帐户并授权[!DNL Workfront Proof]访问权限。 有关详细信息，请参阅[配置个人设置](#configuring-personal-settings)。

您可以将[!DNL Workfront]与[!DNL Basecamp]或[!DNL Basecamp Classic]集成。 [!DNL Basecamp]的每个版本使用不同的API，因此需要不同的配置过程。

有关配置[!DNL Basecamp Classic]的信息，请参阅[集成 [!DNL Workfront Proof] 与 [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## 正在启用[!DNL Basecamp]与[!DNL Workfront Proof]的集成

作为 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[验证权限配置文件或 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的验证权限配置文件，您可以在[帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)中为整个帐户设置[!DNL Basecamp]集成。

1. 在[!UICONTROL Basecamp]中，收集以下信息：

   * [!DNL Basecamp]帐户的URL
   * 在“[!UICONTROL 我的信息]”部分中找到的URL

1. 注销[!DNL Basecamp]。
1. 单击右上角附近的&#x200B;**[!UICONTROL 帐户设置]**。
1. 单击&#x200B;**[!UICONTROL 集成]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL [!DNL Basecamp]集成]**&#x200B;右侧的&#x200B;**[!UICONTROL [!DNL Basecamp]]**&#x200B;部分中，单击&#x200B;**[!UICONTROL 启用]**。

1. 在&#x200B;**[!UICONTROL [!DNL Basecamp]版本]**&#x200B;旁边，验证&#x200B;**[!UICONTROL Classic版本]**&#x200B;是您与之集成的版本。

1. （视情况而定）如果未显示[!DNL Basecamp] URL，请单击&#x200B;**[!UICONTROL 编辑]**，键入您的[!DNL Basecamp]帐户的URL(不包括“http://”)，然后单击&#x200B;**[!UICONTROL 保存]**。

1. 单击窗口右上角的&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**。

1. 单击&#x200B;**[!UICONTROL 集成]**&#x200B;选项卡。
1. 在&#x200B;**[!DNL Basecamp]**&#x200B;下，单击&#x200B;**[!UICONTROL Basecamp集成]**&#x200B;右侧的&#x200B;**[!UICONTROL 启用]**。

1. 在显示的选项中，**[!UICONTROL [!DNL Basecamp]API令牌]**&#x200B;的右侧，单击&#x200B;**[!UICONTROL 编辑]**。

1. 在出现的框中，键入[!DNL Basecamp]中“[!UICONTROL 我的信息]”部分中找到的URL，然后单击&#x200B;**[!UICONTROL 保存]**。\
   将[!DNL Workfront Proof]与[!DNL Basecamp]集成后，您的用户可以配置其个人设置。 有关设置个人设置的信息，请参阅[配置个人设置](#configuring-personal-settings)

1. 如果无法启用[!DNL Basecamp]集成，则[!DNL Workfront Proof]帐户ID可能与您在[!DNL Basecamp]中使用的帐户ID不同。
1. 将[!DNL Workfront Proof]与[!DNL Basecamp]集成后，您的用户可以配置其个人设置。 有关设置个人设置的信息，请参阅[配置个人设置](#configuring-personal-settings)。

## 配置个人设置

在为贵组织设置[帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)后，创建/提交验证的每位作者都应设置其[个人设置。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. 转到&#x200B;**[!UICONTROL 个人**&#x200B;**设置]**。

1. 打开&#x200B;**[!UICONTROL 集成]**&#x200B;选项卡(1)。
1. 要启用[!DNL Basecamp]集成，请单击&#x200B;**[!UICONTROL 启用]** (2)。
1. 单击&#x200B;**[!UICONTROL 连接到您的[!DNL Basecamp]帐户]** (3)。\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. 登录到您的[!DNL Basecamp]帐户(1)。\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. 单击&#x200B;**[!UICONTROL 是，我将允许访问]**&#x200B;以授权[!DNL Workfront Proof]访问您的帐户(2)。\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. （可选）当您的个人集成处于活动状态(3)时，您可以轻松地在[!DNL Basecamp]帐户之间切换。

   1. 单击&#x200B;**[!UICONTROL 切换[!DNL Basecamp]帐户]** (4)。\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      [!UICONTROL Switch Basecamp帐户]会将您转到[!UICONTROL 个人设置]页面，您可以在其中选择要与[!DNL Workfront Proof]帐户集成的[!DNL Basecamp]帐户。

   1. 在选择[!DNL Basecamp]帐户之前，单击&#x200B;**[!UICONTROL 与[!DNL Basecamp]]** (5)重新集成\

      这将刷新[!UICONTROL 个人设置]页面，并显示您的[!DNL Basecamp]帐户的最新列表。

   1. 单击&#x200B;**[!UICONTROL 与此帐户集成]**&#x200B;以将其与[!DNL Workfront Proof]连接。\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      您现在可以向[!DNL Basecamp]项目添加验证。
