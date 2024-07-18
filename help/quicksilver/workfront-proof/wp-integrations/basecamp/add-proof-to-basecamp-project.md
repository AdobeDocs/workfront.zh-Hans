---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: 将验证添加到基础模板项目
description: 设置 [!DNL Basecamp] 集成后，您可以开始向 [!DNL Basecamp] 帐户中的项目添加验证。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: fd62db43-bc45-4ede-b1ef-a198323793ca
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# 将验证添加到基础模板项目

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

设置[!DNL Basecamp]集成后，您可以开始向[!DNL Basecamp]帐户中的项目添加验证。

验证上的查看者随后将在其[!DNL Basecamp]帐户中收到嵌入了[!DNL Workfront Proof]小型验证的消息。 打开邮件后，他们将能够在其[!DNL Basecamp]帐户内对验证进行评论和决策。 有关详细信息，请参阅[在 [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/review-proof-basecamp.md)中查看校对。

作为校对创建者，您需要确保已启用您的[!DNL Basecamp]集成，并在[!UICONTROL 个人设置]中选择了相关的[!DNL Basecamp]帐户（因为您可以与多个[!DNL Basecamp]帐户集成）。

将验证添加到[!DNL Basecamp]项目后，审阅人将收到电子邮件通知，其中将包含在[!DNL Workfront Proof]中查看验证的链接以及在其[!DNL Basecamp]帐户中打开邮件的链接。

## 向[!DNL Basecamp]项目添加新验证

1. 创建校对，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成校对中所述。
1. 如果要通过电子邮件通知审阅人，请确保已启用&#x200B;**[!UICONTROL 通过电子邮件通知联系人]**。\
   请注意，您的[!DNL Basecamp]审阅人将收到其他[!DNL Basecamp]消息。

1. 在&#x200B;**[!UICONTROL 组织]**&#x200B;部分中，单击&#x200B;**[!UICONTROL 将校对添加到[!DNL Basecamp]项目]**。

1. 在出现的&#x200B;**[!UICONTROL 添加到Basecamp]**&#x200B;框中，单击&#x200B;**[!UICONTROL 刷新数据]**&#x200B;以与Basecamp同步。

1. 选择您的Basecamp项目。
1. 在&#x200B;**[!UICONTROL 项目人员]**&#x200B;下，选中要添加到验证的[!DNL Basecamp] Classic帐户中审阅人的复选框。\
   选定的审阅人将在[!DNL Basecamp]中收到此校对的邮件以及来自[!DNL Workfront Proof]的电子邮件通知。

1. 单击&#x200B;**[!UICONTROL 确定]**。
1. 应用校样所需的任何其他设置（正常情况下），然后单击&#x200B;**[!UICONTROL 保存]**&#x200B;以提交校样。

>[!NOTE]
>
>如果已更改审阅者默认值，则必须刷新[!DNL Basecamp]数据，然后才能使用新的默认值。 要刷新[!DNL Basecamp]数据，请单击[!DNL Workfront Proof]中Basecamp弹出窗口上的[!UICONTROL 刷新]链接。 如果您还想在[!DNL Basecamp]中接收消息，请包含您自己的姓名。
>
>使用其他校对设置完成[!UICONTROL 添加到Basecamp]弹出窗口后，单击[!UICONTROL 保存]提交校对。
>
>如果您没有在另一个浏览器窗口中打开[!UICONTROL Basecamp]会话，则必须登录到您的[!DNL Basecamp]帐户，然后才能在[!DNL Basecamp]中看到该消息。

## 将现有验证添加到[!DNL Basecamp]项目

1. 在[!DNL Workfront Proof]中，转到[!UICONTROL 校对详细信息]页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息中所述。
1. 在&#x200B;**[!UICONTROL 工作流]**&#x200B;部分中，打开&#x200B;**[!UICONTROL 更多共享选项]**&#x200B;部分。

1. 确保&#x200B;**[!UICONTROL 校对URL]**&#x200B;和&#x200B;**[!UICONTROL 嵌入代码]**&#x200B;设置为&#x200B;**[!UICONTROL 启用]**。

1. 单击&#x200B;**[!UICONTROL 将校对添加到Basecamp项目]**。
1. 在出现的[!UICONTROL 添加到Basecamp]框中，执行以下操作：

   1. 单击&#x200B;**[!UICONTROL 刷新数据]**&#x200B;以与Basecamp Classic同步，然后再继续。
   1. 选择您的Basecamp项目。
   1. 在&#x200B;**[!UICONTROL 项目人员]**&#x200B;下，选中要添加到验证的[!DNL Basecamp] Classic帐户中审阅人的复选框。
   1. 查看者会出现在默认角色/电子邮件警报中。 所选审阅人在Basecamp中收到此校对的消息，还收到来自[!DNL Workfront Proof]的电子邮件通知。
   1. 如果已更改审阅者默认值，则必须刷新Basecamp数据，然后才能使用新的默认值。 要刷新Basecamp数据，请单击Workfront Proof中Basecamp弹出窗口中的“刷新”链接。 如果您还希望在Basecamp中接收消息，请包含您的个人姓名

1. 单击&#x200B;**[!UICONTROL 确定]**。

将验证添加到[!DNL Basecamp Classic]项目后，您会看到其他选项显示在“验证详细信息”页面的[!UICONTROL 更多共享选项]部分中（有关此页面的信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理验证详细信息）。 您将能够：

* 编辑[!DNL Basecamp Classic]项目详细信息。
* 通过单击框底部的项目URL （该URL包含此验证的标识符）转到[!DNL Basecamp Classic]中的消息。

>[!NOTE]
>
>如果您没有在另一个浏览器窗口中打开[!DNL Basecamp]会话，则必须登录到您的[!DNL Basecamp]帐户，然后才能在[!DNL Basecamp]中看到该消息。

另请参阅[在 [!DNL Basecamp] Classic](../../../workfront-proof/wp-integrations/basecamp-classic/review-proof-basecamp-classic.md)中查看校对。
