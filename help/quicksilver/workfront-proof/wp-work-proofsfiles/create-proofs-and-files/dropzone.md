---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: 拖放区
description: 如果您拥有企业计划，则可以使用拖放区向帐户提交新校样和新版本的校样，而无需登录到您的帐户。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# 拖放区

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您拥有企业计划，则可以使用拖放区向帐户提交新校样和新版本的校样，而无需登录到您的帐户。

当您通过Dropzone提交校样时，该校样会显示在 [!DNL Workfront Proof] 帐户。 从此处，您可以将其路由到工作流中。

## 通过Dropzone URL提交新校样

1. 在您的浏览器中，转到唯一的Dropzone URL，如 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 输入您的电子邮件地址.
1. 单击 **[!UICONTROL 选择文件]** 或 **[!UICONTROL 捕获网页]** 并选择要上传的文件或网页。

1. 输入安全代码，然后单击 **[!UICONTROL 下一个]**.\
   进度栏显示上传的进度。\
   在下一个屏幕中，您将能够添加校样详细信息。\
   请注意，此部分仅在“拖放区”设置中已启用时才显示。

1. 填写详细信息后，单击 **[!UICONTROL 下一个]**.
1. 添加到校样的任何审阅人只有在激活校样时才会收到其通知电子邮件（请参阅下文）。
1. 在将校样提交到拖放区后，它会处于以下状态：

   * 首次将文件上传到拖放区时，校样会显示为草稿。
   * 完成提交后，校样会在您的Dropzone中显示为已提交。
   * 激活并解锁校样后，该校样会在拖放区域中显示为“活动”。
   * 如果校样已锁定，它会在您的拖放区域中显示为已锁定。

## 通过拖放区URL提交现有校样的新版本

1. 在您的浏览器中，转到唯一的Dropzone URL，如 [在中配置拖放区 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 输入您的电子邮件地址.
1. 选中此复选框可指示您正在上传现有校样的新版本。\
   有关创建校样新版本的信息，请参阅。
1. 单击 **[!UICONTROL 选择文件]** 或 **[!UICONTROL 捕获网页]** 并选择要上传的文件或网页。

1. 输入安全代码，然后单击 **[!UICONTROL 下一个]**.\
   进度栏显示上传的进度。\
   Workfront校样会向您发送一封验证电子邮件。

1. 单击电子邮件中的链接。\
   此电子邮件会在您的浏览器中打开Dropzone窗口。 电子邮件通知中的链接有效24小时。
1. 选择校样的先前版本（只显示您创建/提交的校样）。\
   在下一个屏幕中，您将能够添加校样详细信息。\
   此部分仅在“拖放区”设置中已启用时才显示。

1. 键入详细信息，单击 **[!UICONTROL 下一个]**.

   >[!NOTE]
   >
   >添加到校样的任何审阅人只有在激活校样时才会收到其通知电子邮件（请参阅下文）。

   在将校样提交到拖放区后，它会处于以下状态：

   * 首次将文件上传到拖放区时，校样会显示为草稿。
   * 完成提交后，校样会在您的Dropzone中显示为已提交。
   * 激活并解锁校样后，该校样会在拖放区域中显示为“活动”。
   * 如果校样已锁定，它会在您的拖放区域中显示为已锁定。

## 通过电子邮件将校样发送到Dropzone

>[!NOTE]
>
>不再支持通过电子邮件将校样发送到拖放区。


## 完成提交

Workfront会向您（提交者）发送一封填写提交电子邮件，要求您确认文件是新校样还是新版本。 电子邮件通知中的链接有效24小时。

1. 单击链接并按照上述步骤操作，具体取决于它是新校样还是现有校样的新版本。

## 激活校样

拖放区所有者会收到一封通知电子邮件，告知已向拖放区提交了新校样：

* 校样会显示在您帐户的Dropzone页面中（要访问Dropzone页面，请单击左侧导航侧栏中的链接）。
* 校样可由Dropzone所有者（或至少具有Supervisor用户档案的用户）访问。 所有者可以在拖放区设置中进行更改（只有账单管理员或管理员才能执行此操作）。
* 校样在得到处理之前，必须由Dropzone所有者激活/解锁（至少具有主管用户档案的用户也可以激活/解锁）。 在激活/解锁校样之前，校样的状态将显示为已提交。

激活校样：

1. 转到校样右侧的下拉菜单，然后单击 **[!UICONTROL 激活]**.
1. 激活/解锁校样后：

   * 校样状态将变为“活动”。
   * 添加到校样的任何人员都将收到通知电子邮件，建议他们查看新的校样。 （在激活/解锁校样之前，不会发送任何电子邮件。）
   * 证明可以照常进行
   * 如果提交者还将自己明确添加到校样中，则他们将不会收到New校样电子邮件。 有关更多信息，请参阅 [新校样电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## 管理您的Dropzone

通过Dropzone页面，可以轻松管理向Dropzone提交的内容。 您的Dropzone页面包含以下选项和功能：

* 页面布局(1)
* 选择在视图(2)中包含/排除已存档的校样
* 操作按钮(3)
* 排序(4)
* 过滤器(5)
* 校样操作菜单(6)
* 取消存档校样(7)
* 展开/折叠校样摘要(8)
* 选择校样(9)

页面布局以及排序和过滤选项与 [!DNL Views] 列表。 请参阅 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 以了解更多信息。

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
