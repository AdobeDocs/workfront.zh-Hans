---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 使用 [!DNL Workfront Proof]配置用户信息
description: 使用 [!DNL Workfront Proof]配置用户信息
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 使用[!DNL Workfront Proof]配置用户信息

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

1. 按照[使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md)创建用户中的说明开始创建或编辑用户。
1. 指定以下信息：

   * 在&#x200B;**[!UICONTROL 个人详细信息]**&#x200B;部分中：

      * **电子邮件地址：**&#x200B;用户的电子邮件地址。
      * **名字：**&#x200B;用户的名字。
      * **姓氏：**&#x200B;用户的姓氏。
      * **职位：**&#x200B;用户在公司中的职位。
      * **权限配置文件：**&#x200B;用户对验证帐户的权限。
      * **语言：**&#x200B;用户的主要语言。
      * **时区：**&#x200B;选择用户的时区。
      * **日期格式：**&#x200B;选择用户首选的日期格式。
      * **选择加入 — 产品和营销电子邮件：**&#x200B;选择是否选择用户加入产品和营销电子邮件。
      * **仅限API：**&#x200B;允许用户仅通过API登录。

   * 在&#x200B;**[!UICONTROL 用户详细信息]**&#x200B;部分中，键入用户的联系信息，如街道地址和电话号码。
   * 在&#x200B;**[!UICONTROL 默认验证设置]**&#x200B;部分中，配置影响用户创建或处理验证方式的设置。

      * **默认验证角色：**&#x200B;为用户选择默认验证角色。 角色选项为&#x200B;**[!UICONTROL 只读]**、**[!UICONTROL 审阅者]**、**[!UICONTROL 审批者]**、**[!UICONTROL 审阅者和审批者]**、**[!UICONTROL 作者]**&#x200B;或&#x200B;**[!UICONTROL 审查者]**。

        有关验证角色的更多信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理验证角色。

      * **当所有决策都做出时锁定验证：**&#x200B;当所有决策都做出验证后，自动锁定验证以防止进一步更改。
      * **需要登录。 校对只能与其他用户共享：**&#x200B;使校对仅对具有[!DNL Workfront Proof]登录凭据的用户可用。
      * **只需要一个决定：**&#x200B;只需要一个关于校对的决定。
      * **下载原始文件：**&#x200B;允许用户下载原始文件以进行校对。 此选项默认处于启用状态。

        有关下载原始文件的详细信息，请参阅[下载存储在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)中的文件。

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **订阅。 人们可以通过公共URL或嵌入代码注册验证：**&#x200B;允许组织外部的审阅者通过公共URL或嵌入代码注册验证。

        选择此选项时，**订阅者必须单击电子邮件中的链接才能访问校对**&#x200B;也可用。 选择此选项可要求外部查看者单击电子邮件中的链接以访问验证。
如果选择&#x200B;**公共共享**&#x200B;选项，则默认启用此选项。

      * **新来宾审阅人的默认角色：**&#x200B;为来宾审阅人选择默认验证角色。 选项与&#x200B;**默认验证角色**&#x200B;中的选项相同，但审查方和作者除外。

   * 在&#x200B;**[!UICONTROL 默认电子邮件警报设置]**&#x200B;部分中：

      * **默认电子邮件警报：**&#x200B;选择用户接收电子邮件更新的频率。 选择&#x200B;**所有活动、我的评论回复、决策、最终决策、每小时摘要、每日摘要、**&#x200B;或&#x200B;**已禁用**。

        有关默认电子邮件警报选项的详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中配置电子邮件通知设置

      * **新来宾审阅人的默认电子邮件警报：**&#x200B;选择来宾审阅人接收电子邮件更新的频率。 选项与&#x200B;**默认电子邮件警报**&#x200B;的选项相同。

      * **验证就绪时发送电子邮件确认：**&#x200B;选择此项可在验证就绪时自动向用户发送确认电子邮件。
      * **发送给此用户的电子邮件格式：**&#x200B;选择&#x200B;**[!UICONTROL HTML]**&#x200B;或&#x200B;**[!UICONTROL 纯文本]**&#x200B;作为发送给此用户的电子邮件的默认格式。

   * 在&#x200B;**[!UICONTROL 自定义消息设置]**&#x200B;部分中：创建验证模板的设置。

     有关模板的更多信息，请参阅：

      * **验证主题模板：**&#x200B;为验证主题创建模板。
      * **校对消息模板：**&#x200B;为校对消息及其格式创建模板。
