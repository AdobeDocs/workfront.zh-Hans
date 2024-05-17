---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 新验证电子邮件
description: 使本文更适合PiW。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 新验证电子邮件

>[!IMPORTANT]
>
>本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

创建新验证或新版本的验证、将新人员添加到验证或向验证添加工作流时，您可以决定是否要向查看者发送电子邮件，如以下文章中所述：

* [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [在中生成验证 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

收件人收到的电子邮件称作 [!UICONTROL 新校对] 电子邮件。 只有校对创建者和有权将审阅者添加到校对的用户才能控制此电子邮件。 收件人无法禁用它。

新验证电子邮件包含：

* 您的个人消息（如果您选择包括一条消息）
* 如果始终向审阅人发送相同的自定义消息，则最好将其保存在您的页面中 [!UICONTROL 个人设置] 在 [!UICONTROL 校对默认值] 选项卡。 有关更多信息，请参阅。
* 证明的个人链接
* **[!UICONTROL 查看详细信息]** 链接会将您转到关联的 [!DNL Workfront] 对象（如项目、任务或问题）
* 验证图像的缩略图
* 以下证明详细信息：

   * 校样名称
   * 版本号
   * 查看者列表及其在验证中的进度
   * 用于与其他人共享证明的链接

     这允许您共享原始文件的校对URL和/或下载链接。 这不允许您将审阅人明确添加到验证中，您将只共享公共验证URL，并且收件人将获得对验证的只读访问权限。

     请参阅 [在中共享验证 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) 以了解更多信息。

     如果您不希望此链接显示在收件人的电子邮件中，则可以禁用 [!UICONTROL 公共共享] 验证设置

     （下载原始文件和公共URL）。 请参阅 [在中管理校对详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以了解更多信息。

## 活动日志

发送 [!UICONTROL 新校对] 发送给审核者的电子邮件会登录至 [!UICONTROL 活动] 部分 [!UICONTROL 校对详细信息] 页面。 请参阅  [管理[!UICONTROL  校对详细信息] 在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) 以了解更多信息。 您可以检查 [!UICONTROL 新校对] 在创建验证时启用了电子邮件。

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 如果验证的创建者或所有者拥有 [!UICONTROL 已制作校对] 默认情况下，电子邮件处于禁用状态（在其个人设置中），用户不会收到任何电子邮件 [!UICONTROL 校对已制作] 或 [!UICONTROL 新校对] 电子邮件，即使 [!UICONTROL 通过电子邮件通知用户] 复选框。 有关更多信息，请参阅。
>* 如果电子邮件通知在中被禁用为默认设置 [!UICONTROL 帐户设置] 验证的创建者/所有者将不会收到任何 [!UICONTROL 校对已制作] 或 [!UICONTROL 新校对] 即使在其个人设置和 [!UICONTROL 通知] 在新验证页面上，按电子邮件显示人员复选框处于选中状态。 有关详细信息， [此 [!UICONTROL 已制作校对] 电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 并请参阅。
>



## 启用 [!UICONTROL 新校对] 发送电子邮件并包含自定义消息

您可以指定在创建验证时还是在向验证添加某人时，是否向验证查看者发送电子邮件警报。

* [在创建验证时](#when-you-create-a-proof)
* [当您将查看者添加到验证时](#when-you-add-a-reviewer-to-a-proof)

### 在创建验证时 {#when-you-create-a-proof}

当您在中创建新验证时 [!UICONTROL 新校对] 页面，在 **[!UICONTROL 共享]** 部分，您可以选择是否发送电子邮件警报：

* 您可以在此决定是否要 [!UICONTROL 通过电子邮件通知用户] (1)。 如果取消选择此选项，则审阅人不会收到一封电子邮件，告知他们验证已准备好进行审阅。
* 您还可以在电子邮件通知(2)中包含自定义消息。
* 如果您决定添加自己的自定义消息，则可以在电子邮件的正文部分加入自定义主题行(3)和消息(4)。
* 要丢弃自定义消息，只需单击链接(5)。

  >[!NOTE]
  >
  >如果您始终向审阅人发送相同的自定义消息，则最好将其保存在以下的“个人”设置中 [!UICONTROL 校对默认值] 选项卡。 有关更多信息，请参阅。

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 当您将查看者添加到验证时 {#when-you-add-a-reviewer-to-a-proof}

您可以选择是否通知添加到现有验证的新查看者该验证（类似于上文）。

* 首先，通过单击 **[!UICONTROL 共享此版本]** 上的按钮 **[!UICONTROL 校对详细信息]** 第(1)页。

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 将出现一个框，可在其中添加新审阅者。 然后，您可以决定是否要通过电子邮件通知他们(2)，并选择向电子邮件(3)添加自定义消息。

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* 如果选择添加自定义消息，该框将展开，您将能够在电子邮件正文中输入自定义主题行(4)和自定义文本(5)。 您也可以通过单击链接(6)来放弃自定义消息。

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
