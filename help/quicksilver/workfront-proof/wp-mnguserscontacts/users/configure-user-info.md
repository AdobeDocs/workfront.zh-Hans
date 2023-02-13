---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 使用配置用户信息 [!DNL Workfront Proof]
description: 使用配置用户信息 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 使用配置用户信息 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

1. 按照 [使用创建用户 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 指定以下信息：

   * 在 **[!UICONTROL 个人详细信息]** 部分：

      * **电子邮件地址：** 用户的电子邮件地址。
      * **名字：** 用户的名字。
      * **姓氏：** 用户的姓氏。
      * **位置：** 用户在公司中的位置。
      * **权限配置文件：** 用户对校样帐户的权限。
      * **语言：** 用户的主要语言。
      * **时区：** 选择用户的时区。
      * **日期格式：** 选择用户首选的日期格式。
      * **选择加入 — 产品和营销电子邮件：** 选择是否为产品和营销电子邮件选择用户加入。
      * **仅限API:** 允许用户仅通过API登录。
   * 在 **[!UICONTROL 用户详细信息]** 部分，键入用户的联系信息，如街道地址和电话号码。
   * 在 **[!UICONTROL 默认校样设置]** ，请配置影响用户创建或处理校样的方式的设置。

      * **默认校样角色：** 为用户选择默认的校样角色。 角色选项包括 **[!UICONTROL 只读]**, **[!UICONTROL 审阅人]**, **[!UICONTROL 审批者]**, **[!UICONTROL 审核者和审批者]**, **[!UICONTROL 作者]**&#x200B;或 **[!UICONTROL 审核者]**.

         有关校样角色的更多信息，请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **在做出所有决定后锁定证明：** 在对校样做出所有决策后，会自动锁定校样以阻止进一步更改。
      * **需要登录。 校样只能与其他用户共享：** 仅对具有 [!DNL Workfront Proof] 登录凭据。
      * **只需要一个决定：** 只需要一个证据决定。
      * **下载原始文件：** 允许用户下载原始文件进行校样。 默认情况下，此选项处于启用状态。

         有关下载原始文件的更多信息，请参阅 [下载存储在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **订阅. 用户可以通过公共URL或嵌入代码注册校样：** 允许组织外部的审阅人通过公共URL或嵌入代码注册校样。

         选择此选项后， **订阅者必须单击电子邮件中的链接才能访问校样** 中，此变量将被删除。 选择此选项可要求外部审阅人单击电子邮件中的链接以访问校样。
如果 **公共共享** 选项。

      * **新来宾审阅人的默认角色：** 为来宾审阅人选择默认校样角色。 选项与 **默认校样角色。**
   * 在 **[!UICONTROL 默认电子邮件警报设置]** 部分：

      * **默认电子邮件警报：** 选择用户收到电子邮件更新的频率。 选择 **所有活动、对我的评论的回复、决策、最终决策、每小时摘要、每日摘要、** 或 **已禁用**.

         有关默认电子邮件警报选项的更多信息，请参阅 [在中配置电子邮件通知设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **新来宾审阅人的默认电子邮件警报：** 选择来宾审阅人接收电子邮件更新的频率。 选项与 **默认电子邮件警报。**

      * **在校样准备就绪时发送电子邮件确认：** 选择以在校样准备就绪时自动向用户发送确认电子邮件。
      * **发送给此用户的电子邮件格式：** 选择 **[!UICONTROL HTML]** 或 **[!UICONTROL 纯文本]** 作为发送给用户的电子邮件的默认格式。
   * 在 **[!UICONTROL 自定义消息设置]** 部分：为校样模板创建设置。

      有关模板的更多信息，请参阅：

      * **校样主题模板：** 为校样主题创建模板。
      * **校样消息模板：** 为校样消息及其格式创建模板。
