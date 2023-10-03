---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 配置用户信息，使用 [!DNL Workfront Proof]
description: 配置用户信息，使用 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 配置用户信息，使用 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).

1. 按照中的说明开始创建或编辑用户 [创建用户，使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 指定以下信息：

   * 在 **[!UICONTROL 个人详细信息]** 部分：

      * **电子邮件地址：** 用户的电子邮件地址。
      * **名字：** 用户的名字。
      * **姓氏：** 用户的姓氏。
      * **位置：** 用户在公司中的职位。
      * **权限配置文件：** 用户对验证帐户的权限。
      * **语言：** 用户的主要语言。
      * **时区：** 选择用户的时区。
      * **日期格式：** 选择用户首选的日期格式。
      * **选择加入 — 产品和营销电子邮件：** 选择是否选择让用户加入产品和营销电子邮件。
      * **仅限API：** 允许用户仅通过API登录。

   * 在 **[!UICONTROL 用户详细信息]** 部分，键入用户的联系信息，如街道地址和电话号码。
   * 在 **[!UICONTROL 默认验证设置]** 部分，配置影响用户创建或处理验证方式的设置。

      * **默认验证角色：** 为用户选择默认验证角色。 角色选项包括 **[!UICONTROL 只读]**， **[!UICONTROL 查看者]**， **[!UICONTROL 审批者]**， **[!UICONTROL 审阅者和批准者]**， **[!UICONTROL 作者]**，或 **[!UICONTROL 审查方]**.

        有关校对角色的更多信息，请参阅 [在中管理验证角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **作出所有决策时锁定验证：** 在对验证做出所有决定后，自动锁定验证以防止进一步更改。
      * **需要登录。 该验证只能与其他用户共享：** 使验证仅对具有以下权限的用户可用 [!DNL Workfront Proof] 登录凭据。
      * **只需一个决策：** 只需对验证做出一个决定。
      * **下载原始文件：** 允许用户下载原始文件以进行验证。 此选项默认处于启用状态。

        有关下载原始文件的详细信息，请参阅 [下载存储在中的文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **订阅. 用户可以通过公共URL或嵌入代码注册验证：** 允许组织外部的审阅人通过公共URL或嵌入代码注册验证。

        如果选择该选项， **订阅者必须单击电子邮件中的链接才能访问验证** 也可用。 选择此选项可要求外部查看者单击电子邮件中的链接以访问验证。
如果符合以下条件，则默认启用此选项 **公开共享** 已选中选项。

      * **新来宾审阅人的默认角色：** 为访客审阅人选择默认验证角色。 选项与中的相同 **默认验证角色**，但审查方和作者除外。

   * 在 **[!UICONTROL 默认电子邮件警报设置]** 部分：

      * **默认电子邮件警报：** 选择用户接收电子邮件更新的频率。 选择 **所有活动、回复我的意见、决策、最终决策、每小时摘要、每日摘要、** 或 **已禁用**.

        有关默认电子邮件警报选项的详细信息，请参阅 [在中配置电子邮件通知设置 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **新访客审阅人的默认电子邮件警报：** 选择来宾审阅人接收电子邮件更新的频率。 选项与的相同 **默认电子邮件警报。**

      * **验证就绪后发送电子邮件确认：** 选择以在验证就绪时自动向用户发送确认电子邮件。
      * **发送到此用户的电子邮件格式：** 选择 **[!UICONTROL HTML]** 或 **[!UICONTROL 纯文本]** 作为发送给用户的电子邮件的默认格式。

   * 在 **[!UICONTROL 自定义消息设置]** 部分：为验证模板创建设置。

     有关模板的更多信息，请参阅：

      * **验证主题模板：** 为验证主题创建模板。
      * **校对消息模板：** 为验证消息及其格式创建模板。
