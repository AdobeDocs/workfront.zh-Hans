---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 新校样电子邮件
description: 使本文在PiW中更好地工作。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 新校样电子邮件

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

创建新校样或新版本校样、向校样添加新人员或向校样添加工作流时，您可以决定是否向审阅人发送电子邮件，如以下文章所述：

* [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

收件人收到的电子邮件称为 [!UICONTROL 新校样] 电子邮件。 只有校样创建者和有权将审阅人添加到校样的用户才能控制此电子邮件。 收件人无法禁用此功能。

新校样电子邮件包含：

* 您的个人邮件（如果您选择包含一个邮件）
* 如果您始终向审阅人发送相同的自定义消息，则最好将其保存在 [!UICONTROL 个人设置] 下 [!UICONTROL 校对默认值] 选项卡。 有关更多信息，请参阅。
* 证明的个人链接
* **[!UICONTROL 查看详细信息]** 链接，可将您引导至关联的 [!DNL Workfront] 对象（如项目、任务或问题）
* 校样图像的缩略图
* 以下校样详细信息：

   * 校对名称
   * 版本号

      有关更多信息，请参阅。

   * 审稿人名单及其举证进度
   * 用于与其他人共享校样的链接

      这允许您共享原始文件的校样URL和/或下载链接。 这不允许您向校样明确添加审阅者，您将只共享公共校样URL，收件人将获得对校样的只读访问权限。

      请参阅 [在中共享校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) 以了解更多信息。

      如果您不希望此链接显示在收件人的电子邮件中，则可以禁用 [!UICONTROL 公共共享] 校样设置

      （下载原始文件和公共URL）。 请参阅 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以了解更多信息。

## 活动日志

发送 [!UICONTROL 新校样] 发送给审阅人的电子邮件已登录 [!UICONTROL 活动] 部分 [!UICONTROL 校样详细信息] 页面。 请参阅  [管理[!UICONTROL  校样详细信息] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以了解更多信息。 您可以检查 [!UICONTROL 新校样] 创建校样时启用了电子邮件。

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 如果校样的创建者或所有者 [!UICONTROL 制作校样] 默认情况下处于禁用状态的电子邮件（在其个人设置中），他们将不会收到任何 [!UICONTROL 制作的证明] 或 [!UICONTROL 新校样] 即使 [!UICONTROL 通过电子邮件通知用户] 框中，选择“New proof”（新建校样）。 有关更多信息，请参阅。
>* 如果在 [!UICONTROL 帐户设置] 校样的创建者/所有者将不会收到任何 [!UICONTROL 制作的证明] 或 [!UICONTROL 新校样] 电子邮件，即使在其个人设置中启用此功能，并且 [!UICONTROL 通知] “New proof”（新建校样）页面上勾选了“people by email”（按电子邮件进行人员）框。 有关更多信息，请 [的 [!UICONTROL 制作校样] 电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 和请参阅。
>




## 启用 [!UICONTROL 新校样] 电子邮件并包含自定义消息

您可以指定是在创建校样时，还是在向校样的审阅人添加人时，向审阅人发送电子邮件警报。

* [创建校样时](#when-you-create-a-proof)
* [在向校样添加审阅者时](#when-you-add-a-reviewer-to-a-proof)

### 创建校样时 {#when-you-create-a-proof}

在 [!UICONTROL 新校样] 页面下 **[!UICONTROL 共享]** ，您可以选择是否发送电子邮件警报：

* 在这里，您可以决定是否要 [!UICONTROL 通过电子邮件通知用户] (1)。 如果取消选择此选项，则审阅人不会收到电子邮件，告知他们校样已准备好供审阅。
* 您还可以在电子邮件通知(2)中包含自定义消息。
* 如果您决定添加自己的自定义消息，则可以在电子邮件正文(4)中放入自定义主题行(3)和消息。
* 要放弃自定义消息，只需单击链接(5)。

   >[!NOTE]
   >
   >如果您始终向审阅人发送相同的自定义消息，则最好在 [!UICONTROL 校对默认值] 选项卡。 有关更多信息，请参阅。

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 在向校样添加审阅者时 {#when-you-add-a-reviewer-to-a-proof}

您可以选择添加到现有校样的新审阅人是否会收到校样的通知（与上面类似）。

* 首先，通过单击 **[!UICONTROL 共享此版本]** 按钮 **[!UICONTROL 校样详细信息]** (1)页。

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 此时会出现一个框，您可以在其中添加新审阅人。 然后，您可以决定是否希望通过电子邮件(2)通知他们，并选择向电子邮件(3)添加自定义消息。

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* 如果选择添加自定义消息，将展开该框，您将能够在电子邮件正文(5)中放入自定义主题行(4)和自定义文本。 您还可以通过单击链接(6)来放弃自定义消息。

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
