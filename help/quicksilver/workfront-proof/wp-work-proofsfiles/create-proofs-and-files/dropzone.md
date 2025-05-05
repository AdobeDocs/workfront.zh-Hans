---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: 拖放区域
description: 如果您拥有企业计划，则可以使用拖放区域向您的帐户提交新验证和新版本验证，而无需登录到您的帐户。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# 拖放区域

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果您拥有企业计划，则可以使用拖放区域向您的帐户提交新验证和新版本验证，而无需登录到您的帐户。

当您通过Dropzone提交验证时，它将显示在您[!DNL Workfront Proof]帐户的Dropzone页面中。 从那里，您可以将其路由到您的工作流中。

## 通过Dropzone URL提交新验证

1. 在浏览器中，转到唯一的拖放区域URL，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中配置拖放区域中所述
1. 输入您的电子邮件地址。
1. 单击&#x200B;**[!UICONTROL 选择文件]**&#x200B;或&#x200B;**[!UICONTROL 捕获网页]**，然后选择要上载的文件或网页。

1. 输入安全代码，然后单击&#x200B;**[!UICONTROL 下一步]**。\
   进度条会显示上传的进度。\
   在下一个屏幕中，您将能够添加校样详细信息。\
   请注意，此部分仅在“拖放区域”设置中启用时显示。

1. 填写详细信息后，单击&#x200B;**[!UICONTROL 下一步]**。
1. 添加到验证的任何审阅人，将仅在激活验证（见下文）时收到其通知电子邮件。
1. 在您将证明提交到Dropzone后，该证明将经历以下状态：

   * 首次将文件上传到拖放区域时，验证会在那里显示为草稿。
   * 完成提交后，证明将在您的拖放区域显示为已提交。
   * 激活并解锁验证后，它在您的拖放区域中显示为活动。
   * 如果验证已锁定，则在拖放区域中显示为“已锁定”。

## 通过拖放区域URL提交现有验证的新版本

1. 在浏览器中，转到唯一的拖放区域URL，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中配置拖放区域中所述
1. 输入您的电子邮件地址。
1. 选中该复选框可指示您正在上载现有校对的新版本。\
   有关创建新版本的验证的信息，请参阅。
1. 单击&#x200B;**[!UICONTROL 选择文件]**&#x200B;或&#x200B;**[!UICONTROL 捕获网页]**，然后选择要上载的文件或网页。

1. 输入安全代码，然后单击&#x200B;**[!UICONTROL 下一步]**。\
   进度条会显示上传的进度。\
   Workfront Proof会向您发送一封验证电子邮件。

1. 单击电子邮件中的链接。\
   电子邮件会在您的浏览器中打开Dropzone窗口。 电子邮件通知中的链接有效期为24小时。
1. 选择校对的先前版本（仅显示您创建/提交的校对）。\
   在下一个屏幕中，您将能够添加校样详细信息。\
   仅当在“拖放区域”设置中启用此分区时，它才会显示。

1. 键入详细信息，然后单击&#x200B;**[!UICONTROL 下一步]**。

   >[!NOTE]
   >
   >添加到验证的任何审阅人，将仅在激活验证（见下文）时收到其通知电子邮件。

   在您将证明提交到Dropzone后，该证明将经历以下状态：

   * 首次将文件上传到拖放区域时，验证会在那里显示为草稿。
   * 完成提交后，证明将在您的拖放区域显示为已提交。
   * 激活并解锁验证后，它在您的拖放区域中显示为活动。
   * 如果验证已锁定，则在拖放区域中显示为“已锁定”。

## 通过电子邮件将证明发送到拖放区域

>[!NOTE]
>
>不再支持通过电子邮件将验证发送到拖放区域。


## 正在完成您的提交

Workfront会向您（提交者）发送一封完整的提交电子邮件，要求您确认文件是新验证还是新版本。 电子邮件通知中的链接有效期为24小时。

1. 单击链接并按照上述步骤操作，具体取决于它是新验证还是现有验证的新版本。

## 激活验证

拖放区域所有者会收到一封通知电子邮件，告知已向Dropzone提交新验证：

* 验证会显示在您帐户的拖放区域页面中（要访问拖放区域页面，请单击左侧导航侧边栏中的链接）。
* 拖放区域所有者（或至少拥有主管配置文件的用户）可访问该验证。 可以在拖放区域设置中更改所有者（只有帐单管理员或管理员可以执行此操作）。
* 必须先由Dropzone所有者激活/解锁验证，然后才能处理验证（具有至少主管配置文件的用户也可以执行此操作）。 在激活/解锁之前，验证状态显示为“已提交”。

要激活验证，请执行以下操作：

1. 转到校样右侧的下拉菜单，然后单击&#x200B;**[!UICONTROL 激活]**。
1. 激活/解锁验证后：

   * 验证状态更改为活动。
   * 添加到验证的任何人都将收到通知电子邮件，告知他们要审阅的新验证。 （在激活/解锁验证之前，不会发送电子邮件。）
   * 这个证据可以正常使用
   * 如果提交者还明确将自己添加到验证，则不会收到New proof电子邮件。 有关详细信息，请参阅[新验证电子邮件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

## 管理您的拖放区域

通过Dropzone页面，可以轻松管理提交到Dropzone的操作。 您的拖放区域页面包含以下选项和功能：

* 页面布局(1)
* 选择在视图中包括/排除存档的验证(2)
* 操作按钮(3)
* 排序(4)
* 筛选器(5)
* 验证操作菜单(6)
* 将验证取消存档(7)
* 展开/折叠验证摘要(8)
* 选择验证(9)

页面布局、排序和筛选选项与[!DNL Views]列表中的选项相同。 有关详细信息，请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中查看页面上的管理项目。

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
