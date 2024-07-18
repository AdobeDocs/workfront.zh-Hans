---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: 在 [!DNL Workfront Proof]中配置附属帐户
description: 附属帐户是您从自己的 [!DNL Workfront] Proof帐户中配置并管理的付费帐户。 有关详细信息，请参阅“在 [!DNL Workfront] 校对中的附属帐户”。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中配置附属帐户

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

附属帐户是您从自己的[!DNL Workfront Proof]帐户中配置并管理的付费帐户。 有关详细信息，请参阅 [!DNL Workfront] Proof](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md)中的[附属帐户。

任何账单管理员都可以创建附属帐户。 有关计费管理员的信息，请参阅 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[[!UICONTROL 证明权限配置文件]。

>[!NOTE]
>
> 必须在我们的[!UICONTROL Standard]或更高版本计划之一上设置附属帐户。

## 创建附属帐户 {#creating-a-satellite-account}

要创建附属帐户，请执行以下操作：

1. 转到[!UICONTROL 帐单]页面。\
   有关计费页面的详细信息，请参阅[计费 [!DNL Workfront Proof] [!UICONTROL 页面]](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

1. 单击&#x200B;**[!UICONTROL 新建附属帐户]**&#x200B;帐户按钮。 (1)

   此时会出现一个弹出窗口。

   ![New_Satellite_Account.png](assets/new-satellite-account-350x156.png)

1. 输入客户的详细信息，包括任何相关的促销代码。
1. 单击&#x200B;**[!UICONTROL 保存]**。 Satellite帐户会自动显示在[!UICONTROL 帐单]页面顶部的[!UICONTROL 帐户]下拉菜单中。
1. 从下拉菜单中选择新的Satellite帐户。
1. 继续[为您的卫星帐户选择计划](#selecting-a-plan-for-your-satellite-account)以升级您的卫星帐户。

## 为卫星帐户选择计划 {#selecting-a-plan-for-your-satellite-account}

按照[创建附属帐户](#creating-a-satellite-account)中的说明设置附属帐户后，您需要将其升级到所需的计划。

1. 转到[!UICONTROL 帐单]页面。\
   有关计费页面的详细信息，请参阅[计费 [!DNL Workfront Proof] [!UICONTROL 页面]](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

1. 在页面顶部的&#x200B;**[!UICONTROL 您的帐户]**&#x200B;下拉菜单中(1)，选择相关的附属帐户。

   此时将显示Satellite帐户的账单页面，并自动复制您帐户中的账单联系人详细信息。

   ![Satellite_Account_Change_Plan.png](assets/satellite-account-change-plan-350x156.png)

1. 单击页面右上角的&#x200B;**[!UICONTROL 更改计划]**&#x200B;按钮。 (2)\
   或\
   单击当前或下一个计划名称以打开弹出窗口。 (3)

1. 升级或降级您的计划。

## 将用户添加到您的卫星帐户

将Satellite帐户升级到所选计划后，您需要将用户添加到该帐户。

1. 以[!DNL Workfront Proof]管理员身份登录到[!DNL Workfront Proof]。
1. 单击&#x200B;**[!UICONTROL 帐户设置]**。
1. 在页面顶部的下拉菜单中，选择相关的Satellite帐户。 (1)\
   此时将显示Satellite帐户的帐户设置页面。
1. 单击页面右上角的&#x200B;**[!UICONTROL 新用户]**&#x200B;按钮。 (2)\
   此时将显示[!DNL New User]页。

1. 输入用户的详细信息，然后单击&#x200B;**[!UICONTROL 保存]**。\
   用户会收到电子邮件通知，告知他们可访问该帐户。

添加到Satellite帐户的用户在中心帐户的联系人列表中显示为成员。

同样，中心帐户中的用户将显示为Satellite帐户联系人中的成员。

若要查看Satellite帐户中所有用户的完整列表，请单击&#x200B;**[!UICONTROL 用户]**&#x200B;选项卡。

![SA_New_User.png](assets/sa-new-user-350x156.png)

## 将现有的单独帐户关联到您的中心帐户

如果您之前为客户创建了其他单独的帐户，则可以将这些帐户转换为Satellite帐户。

我们通过将他们关联到您的[!DNL Workfront Proof]帐户（使其成为中心帐户）来解决此问题。

您只需向我们提供以下详细信息：

* [!DNL Workfront Proof]帐户的名称和用于设置该帐户的电子邮件地址
* 要链接到帐户的单独帐户的名称以及用于设置单独帐户的电子邮件地址。
