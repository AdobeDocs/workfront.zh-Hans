---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在 [!DNL Workfront Proof]中配置校对设置
description: 您可以在验证中配置正在创建或编辑的验证。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# 在[!DNL Workfront Proof]中配置校对设置

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

您可以通过以下任意方式配置正在创建或编辑的校样：

>[!NOTE]
>
>您可以为创建的所有新验证配置这些设置。 有关更多信息，请参阅。

## 做出最后决定时锁定验证

您可以将验证状态设置为在最终审批者做出决定时锁定。 如果要确保审阅人无法返回验证并添加其他评论或更改其决策，则此功能非常有用。

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于新校对，在&#x200B;**[!UICONTROL 校对设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 当做出所有必需的决策时锁定校对]**。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 当作出所有决策时锁定校对]**。

有关决策的信息，请参阅[在验证查看者中做出校对决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

## 需要所有查看证明的用户登录

有关[!DNL Workfront Proof]的好处之一是，任何人都可以查看证明，您无需拥有自己的[!DNL Workfront Proof]即可查看证明。 收件人将收到一封电子邮件，其中包含个人URL，可让他们直接转到验证页面，而无需登录[!DNL Workfront Proof]。

但是，如果您的审阅和批准流程需要更高的安全级别，则可以使用需要登录到验证。 这意味着只能将[!DNL Workfront Proof]个用户添加到验证中。 他们必须先输入电子邮件和密码，然后才能访问。

>[!NOTE]
>
>* *为了让某人登录验证（启用需要登录时），必须将他们添加到验证中。*
>* *如果启用“需要登录”，则无法启用订阅。*

要要求查看验证的所有用户登录，请执行以下操作：

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于新校对，在&#x200B;**[!UICONTROL 校对设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 需要登录]**。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 需要登录]**。

## 只需一个决策即可验证

如果您只需要组、部门或公司中的一个人员对验证做出决定，则此设置非常有用。

即使您将审批者或查看者和审批者的角色分配给多个人，一旦某人做出验证决策，验证的状态将更新（根据所做的决策）。 有关校对状态的详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)中查看校对的进度和状态

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于新校对，在&#x200B;**[!UICONTROL 工作流]**&#x200B;下，选择&#x200B;**[!UICONTROL 此阶段]**&#x200B;只需要一个决定。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 仅需要一个决定]**。

有关决策的信息，请参阅[在验证查看者中做出校对决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof)。

## 要求对决策进行电子签名

您可以要求决定提供电子邮件和密码的证明的任何审阅人的电子签名。 当审核者出现决策提示时，会要求他们输入电子邮件和密码并确认其决策。 有关详细信息，请参阅[了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)中的电子签名

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于新校对，在&#x200B;**[!UICONTROL 校对设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 要求以电子方式签署决策]**。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 要求对决策进行电子签名]**。

有关决策的信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md)中配置批准决策选项。

## 不允许用户下载原始文件

您可以阻止校对上的审阅人下载创建校对的原始文件。

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于&#x200B;**[!UICONTROL 校对设置]**&#x200B;下的新校对，取消选择&#x200B;**[!UICONTROL 下载原始文件]**。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 下载原始文件]**。

## 允许其他用户订阅验证

订阅是一个高级设置，可与验证URL和迷你验证配合使用。

默认情况下，未专门添加到验证并使用Proof URL或迷你验证访问它的人只能以只读模式查看验证。 已是验证查看者的用户可以使用其电子邮件地址登录。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校对角色

启用验证订阅允许尚未明确添加到验证的用户订阅验证（即，将自己添加到验证）。 然后，将为他们分配您在订阅设置中为他们选择的角色和电子邮件警报。

如果对验证启用了订阅，则以下字段将变为活动状态：

* **[!UICONTROL 需要订阅者验证]** — 订阅者必须单击电子邮件中的链接才能访问验证\
   选择此选项意味着订阅者将无法立即访问验证，但会通过电子邮件获得指向验证的链接。 订阅者验证的目的是确保用户输入的电子邮件地址正确无误。

* **[!UICONTROL 新订阅者的默认角色]** — 这是将分配给订阅了验证的所有审阅人的默认验证角色。
* **[!UICONTROL 新订阅者的默认电子邮件警报]** — 这是将分配给所有订阅了验证的审阅人的默认电子邮件警报。

另请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)中订阅验证

允许其他用户订阅验证：

1. 按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的说明创建新验证。\
   或\
   打开现有校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。

1. 对于&#x200B;**[!UICONTROL 验证设置]**&#x200B;下的新验证，请取消选择&#x200B;**[!UICONTROL 通过公共URL或嵌入代码订阅验证]**。\
   或\
   对于现有校对，在&#x200B;**[!UICONTROL 设置]**&#x200B;下，选择&#x200B;**[!UICONTROL 订阅]**。
