---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中配置校样设置 [!DNL Workfront Proof]
description: 您可以通过以下任一方式配置要创建或编辑的校样 — 编辑我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 1%

---

# 在中配置校样设置 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

您可以通过以下任一方式配置要创建或编辑的校样：

>[!NOTE]
>
>您可以为创建的所有新校样配置这些设置。 有关更多信息，请参阅。

## 在做出最后决定时锁定验证

您可以设置校样状态，以在最终审批者做出决策时将其锁定。 如果您希望确保审阅人无法返回到校样并添加其他注释或更改其决策，则此功能非常有用。

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 校样设置]**，选择 **[!UICONTROL 在做出所有必需的决策时锁定验证]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 在做出所有决定时锁定证据]**.

有关决策的信息，请参阅 [在校对查看器中对校样做出决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## 需要对查看校样的所有用户进行登录

关于 [!DNL Workfront Proof] 任何人都可以查证，你不需要拥有自己的证据 [!DNL Workfront Proof] 这样做。 收件人会收到一封包含个人URL的电子邮件，该URL会将他们直接转到校样页面，而无需他们登录 [!DNL Workfront Proof].

但是，如果您在审核和批准过程中需要更高级别的安全性，则可以使用要求登录校样。 这只意味着 [!DNL Workfront Proof] 可以将用户添加到校样中。 他们必须输入电子邮件和密码才能访问。

>[!NOTE]
>
>* *为了让某人登录到校样（在启用了“需要登录”的情况下），必须将他们添加到校样中。*
>* *如果启用了“需要登录”，则无法启用“订阅”。*


要要求查看校样的所有用户都登录，请执行以下操作：

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 校样设置]**，选择 **[!UICONTROL 需要登录]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 需要登录]**.

## 只需要一项证明决定

当您只需要组、部门或公司中的一个人来决定校样时，此设置非常有用。

即使您将“审批者”或“审核者”和“审批者”角色分配给多人，一旦一个人对校样做出决策，校样的状态将会更新（根据做出的决策）。 有关校样状态的更多信息，请参阅 [在中查看校样的进度和状态 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 工作流]**，选择 **[!UICONTROL 此阶段只需要一个决策]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 只需要一个决定]**.

有关决策的信息，请参阅 [在校对查看器中对校样做出决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## 要求以电子方式签署决定

您可以要求对校样做出决策的任何审阅人的电子签名来提供其电子邮件和密码。 当审阅人做出决策提示时，会要求他们输入其电子邮件和密码并确认其决策。 有关更多信息，请参阅 [了解 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 校样设置]**，选择 **[!UICONTROL 要求以电子方式签署决定]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 要求以电子方式签署决定]**.

有关决策的信息，请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## 不允许用户下载原始文件

您可以让审阅人不要下载从中创建校样的原始文件。

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 校样设置]**&#x200B;取消选择 **[!UICONTROL 下载原始文件]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 下载原始文件]**.

## 允许其他用户订阅校样

订阅是一种适用于校样URL和Mini校样的高级设置。

默认情况下，尚未专门添加到校样并使用校样URL或Mini校样访问校样的人员只能在只读模式下查看校样。 已经是校样审阅人的用户可以使用其电子邮件地址登录。 有关更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

启用校样订阅功能后，尚未明确添加到校样的用户便可以订阅校样（即将自己添加到校样中）。 然后，会为他们分配您在订阅设置中为其选择的角色和电子邮件警报。

如果校样已启用订阅，则以下字段将变为活动字段：

* **[!UICONTROL 需要订阅者验证]**  — 订阅者必须单击电子邮件中的链接才能访问校样\
   选择此选项意味着订阅者无法立即访问校样，但会在电子邮件中获得指向校样的链接。 订阅者验证的目的是确保用户输入了他们有权访问的正确电子邮件地址。

* **[!UICONTROL 新订阅者的默认角色]**  — 这是默认的校样角色，将分配给所有订阅校样的审阅人。
* **[!UICONTROL 新订阅者的默认电子邮件警报]**  — 这是默认的电子邮件警报，将分配给所有订阅校样的审阅人。

另请参阅 [在中订阅校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

要允许其他用户订阅校样，请执行以下操作：

1. 创建新校样，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).\
   或\
   打开现有校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

1. 为了找新证据， **[!UICONTROL 校样设置]**&#x200B;取消选择 **[!UICONTROL 通过公共URL或嵌入代码订阅校样]**.\
   或\
   对于现有证据，在 **[!UICONTROL 设置]**，选择 **[!UICONTROL 订阅]**.
