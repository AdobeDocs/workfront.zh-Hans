---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 标记用户以共享校样
description: 当您在校样查看器中对校样进行注释时，可以标记其他用户以通过电子邮件引起他们对您的评论的注意，并将他们添加到校样的工作流中。
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 标记用户以共享校样

当您在校样查看器中对校样进行注释时，可以标记其他用户以通过电子邮件引起他们对您的评论的注意，并将他们添加到校样的工作流中。

在校样的注释中标记用户时，您能够标记的用户可能会因各种因素而异，例如单个用户权限和您组织中的成员资格：

* 如果您是校样创建者、所有者或启用了特定权限，则可以在校样工作流之外标记用户，并与他们共享校样。
* 如果您作为外部用户添加到校样，并且您是另一个具有不同校样帐户的环境的成员，则只能从原始环境中标记这些用户。 <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 访问要求 {#access-requirements}

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校样角色</td> 
   <td>作者、审核者</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>主管或管理员</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 标记用户以共享校样

在 [访问要求](#access-requirements) 默认情况下，上面的部分可以标记用户以共享校样。 如果您是校样所有者或创建者，则还可以为用户添加标记以共享校样，而不考虑“校样权限配置文件”或“校样”角色。 您可以允许具有较低“校样权限配置文件”或“校样”角色的用户在创建校样时标记用户以共享校样。 有关更多信息，请参阅 [配置工作流并添加审阅人](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) 部分 [使用基本工作流创建高级校样](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 文章。

>[!NOTE]
>
>仅当满足以下任一条件时，才可使用外部协作者的电子邮件地址标记外部协作者：>
>* 您组织的Workfront帐户中的用户已将该协作者的电子邮件地址添加到以前的校样中。
>* 该协作者以前使用电子邮件地址在贵组织的Workfront帐户中订阅校样。
>


要标记某个人并在评论中共享校样，请执行以下操作：

1. 在对校样发表评论时，请键入@符号(@)，后跟人员的姓名或电子邮件地址。 开始键入时，可用名称会显示在下拉列表中。
1. 当您在下拉列表中看到该人员时，请选择该人员的姓名。

   >[!TIP]
   >
   >如果要在不选择任何人的情况下关闭下拉列表，可以按 **Esc** 键或单击列表外的任意位置。

1. 对要在评论中标记的任何其他用户重复步骤1-2。
1. 完成注释，然后单击 **帖子**.
1. （视情况而定）如果您标记了尚未添加到校样的任何人，请指定 **校样角色** 和 **电子邮件警报** 为显示的框中列出的每个用户设置，然后单击 **添加人员和帖子评论**.

   ![](assets/add-people-to-proof-350x220.png)

   有关校样角色的信息，请参阅。 有关校样电子邮件警报的信息，请参阅文章中的部分 [在Workfront校样中配置电子邮件通知设置](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   如果校样具有自动工作流，则您标记的用户将会添加到您所在的舞台。 有关更多信息，请参阅 [自动化工作流概述](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   您标记的任何人都会收到有关您的校样评论的通知电子邮件，无论他们使用的是何种校样电子邮件警报设置：

   * 如果用户收到每日摘要或每小时的摘要电子邮件，则Workfront会单独发送通知，并在摘要电子邮件中包含有关您的校样评论的信息。
   * 如果用户收到所有活动或对其评论的回复的警报，则通知将替换有关这些评论和回复的通知。

有关将用户添加到校样的其他方法的信息，请参阅 [在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
