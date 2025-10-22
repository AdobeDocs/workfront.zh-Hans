---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 标记要共享验证的用户
description: 在验证查看者中评论验证时，您可以标记其他用户以通过电子邮件提请他们注意您的评论，并将他们添加到验证的工作流中。
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 标记要共享验证的用户

在验证查看者中评论验证时，您可以标记其他用户以通过电子邮件提请他们注意您的评论，并将他们添加到验证的工作流中。

在校对的评论中标记用户时，您可以标记的用户可能会因各种因素而异，例如个人用户权限和您在组织中的成员资格：

* 如果您是验证创建者、所有者或启用了特定权限，则可以在验证工作流之外标记用户并与他们共享验证。
* 如果您作为外部用户添加到验证，并且您是另一个具有不同验证帐户环境的成员，则只能标记原始环境中的这些用户。<!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 访问要求 {#access-requirements}

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>任何</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">验证角色</td> 
   <td>作者、审查方</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校样权限配置文件</td> 
   <td>主管或管理员</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 标记要共享验证的用户

默认情况下，具有上面[访问要求](#access-requirements)部分中概述的验证权限配置文件或验证角色的用户可以标记用户以共享验证。 如果您是验证所有者或创建者，则还可以标记用户以共享验证，而不管验证权限配置文件或验证角色如何。 您可以允许具有较低验证权限配置文件或验证角色的用户在创建验证时标记用户以共享验证。 有关详细信息，请参阅[使用基本工作流创建高级校对](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur)文章中的[配置工作流并添加审阅者](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)部分。

>[!NOTE]
>
>仅当满足以下任一条件时，您才可以使用外部协作者的电子邮件地址为其添加标记：
>
>* 您组织的Workfront帐户中的用户之前已将协作者电子邮件地址添加到验证中。
>* 协作者之前使用电子邮件地址订阅了您组织的Workfront帐户中的验证。

要标记某人并在评论中共享验证，请执行以下操作：

1. 对验证进行评论时，请键入at sign (@)，后跟人员的姓名或电子邮件地址。 开始键入时，可用名称将显示在下拉列表中。
1. 在下拉列表中看到人员时，选择人员姓名。

   >[!TIP]
   >
   >如果要关闭下拉列表而不选择任何人，可以按&#x200B;**Esc**&#x200B;键或单击列表之外的任意位置。

1. 对要在注释中标记的任何其他用户重复步骤1-2。
1. 完成评论，然后单击&#x200B;**帖子**。
1. （视情况而定）如果您为尚未添加到验证的任何人添加标签，请为显示的框中列出的每个用户指定&#x200B;**验证角色**&#x200B;和&#x200B;**电子邮件提醒**&#x200B;设置，然后单击&#x200B;**添加联系人并发布评论**。

   ![将人员添加到校对](assets/add-people-to-proof-350x220.png)

   有关验证角色的信息，请参阅。 有关验证电子邮件警报的信息，请参阅[在Workfront Proof中配置电子邮件通知设置](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)一文中的部分。

   如果验证具有自动工作流，则您标记的用户将添加到您所在的阶段。 有关详细信息，请参阅[自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

   您标记的任何人都将收到有关您的验证评论的通知电子邮件，无论他们使用何种验证电子邮件警报设置：

   * 如果用户收到每日摘要或每小时摘要电子邮件，Workfront会单独发送通知，并在摘要电子邮件中包含有关验证评论的信息。
   * 如果用户收到有关所有活动的警报，或收到有关用户评论的回复，则通知将替换有关这些评论和回复的通知。

有关将用户添加到验证的其他方法的信息，请参阅[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。
