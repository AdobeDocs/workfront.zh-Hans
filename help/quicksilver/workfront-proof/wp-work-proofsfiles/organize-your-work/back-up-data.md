---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 备份 [!DNL Workfront Proof] 数据
description: 您可以使用备份函数请求备份 [!DNL Workfront Proof] 中的所有数据。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 备份[!DNL Workfront Proof]数据

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

## 备份简介

您可以使用备份函数请求备份[!DNL Workfront Proof]中的所有数据。

备份将以.zip文件的形式提供给您。 它包含所有数据的XML导出（包括所有校对的所有版本的注释和响应）；但是，它不包括您作为校对上传的原始文件。

为您创建的每个要下载的备份.zip文件都有一个唯一的文件名，例如：

9789_05_05_2011_61703.zip

此示例中的文件名提供了以下信息：

* 9789是您的[!DNL Workfront Proof]帐户标识符
* 05_05_2011是创建日期：2011年5月5日
* 61703是随机系统分配的数字

此命名约定使您轻松地将所有备份.zip文件存储在计算机上的单个位置，并了解每个备份的确切创建时间。

[!UICONTROL 备份]函数允许您决定如何使用资源：

* 使您可以释放存储空间，而不会丢失活动或存档的校样。 您可以请求备份，删除校样，然后清空[还原并清空 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)中的垃圾桶。
* 允许您访问最初上载到[!DNL Workfront]验证的任何文件。 您可以在删除校样之前使用[!UICONTROL 下载原始文件]功能下载它们。

>[!NOTE]
>
>使用备份时，请考虑以下事项：
>
>* 备份在企业计划和无限计划上可用。 请联系我们的[销售团队](mailto:sales@proofhq.com)获取报价。
>* 默认情况下，数据编码类型设置为UTF-8，我们建议进行此设置。 这是Internet应用程序最常用的编码类型。
>* 您一次只能请求一个[!DNL backup]。 当处理您的备份.zip文件时，将不会显示“备份”选项卡上的“请求新备份”链接，并且显示的消息保持不变。 有关请求备份的信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md)中请求新的数据备份。
>



## 备份数据

1. 单击[!DNL Workfront Proof]界面右上角的&#x200B;**[!UICONTROL 帐户设置]**。 (1)
1. 单击&#x200B;**[!UICONTROL 备份]**&#x200B;选项卡。 (2)
1. 单击&#x200B;**[!UICONTROL 请求新备份]**&#x200B;链接(3)

当备份就绪时，将发生以下情况：

* 您收到来自[!DNL Workfront Proof]的电子邮件，通知您此问题（“您的[!DNL Workfront Proof]备份已就绪”）。 该电子邮件包含备份数据的下载链接。
* [帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)备份选项卡显示备份数据的下载链接。
* Request new backup （请求新备份）链接(3)重新出现在Backups （备份）选项卡上

您的数据将可以下载为zip文件。 您可以从通知电子邮件或[!UICONTROL 帐户设置]中下载备份.zip文件，如以下部分所述：

* [从电子邮件通知下载备份.zip文件](#downloading-your-backup-zip-file-from-your-email-notification)
* [从帐户设置下载备份.zip文件](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## 从电子邮件通知下载备份.zip文件 {#downloading-your-backup-zip-file-from-your-email-notification}

当您的备份.zip文件已可供下载时，您将收到来自[!DNL Workfront Proof]的电子邮件，其主题行为“您的[!DNL Workfront Proof]备份已准备就绪”。

要从电子邮件下载备用.zip文件，请执行以下操作：

1. 单击电子邮件中的下载链接。\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   如果您当前未登录到[!DNL Workfront Proof]，则会打开一个新的浏览器窗口并显示登录页面。

## 从帐户设置下载备份.zip文件 {#downloading-your-backup-zip-file-from-the-account-settings}

当您的备份.zip文件已可供下载时，[!UICONTROL 备份]选项卡将显示下载链接来指示此情况。 此外，还会再次显示[!UICONTROL 请求新备份]链接。

1. 单击[!DNL Workfront Proof]界面右上角的&#x200B;**[!UICONTROL 帐户设置]**。 (1)
1. 单击&#x200B;**[!UICONTROL 备份]**&#x200B;选项卡。 (2)\
   如果帐户中没有用户请求任何备份，则[!UICONTROL 备份]选项卡指示您没有备份。 如果用户已请求备份，该选项卡将显示上次备份的创建日期和下载链接。

1. 单击&#x200B;**[!UICONTROL 下载备份]**&#x200B;链接。 (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png)出现“File Download（文件下载）”屏幕，询问您是要打开还是保存下载文件。

1. 单击&#x200B;**[!UICONTROL 保存]**，然后在计算机上选择要保存备份.zip文件的位置。\
   在您下次请求备份之前，确定最近备份日期的消息仍显示在[!UICONTROL 备份]页面的底部。 下载备份链接适用于上次备份。 每当显示[!UICONTROL 请求新备份]链接时，您都可以单击该链接以请求另一个备份。

## 了解备份.zip文件中的文件

您的备份.zip文件包含七个CSV（逗号分隔值或逗号分隔）文件，这些文件包含直到备份数据时来自您的活动和存档验证的信息：

* comments.csv — 包含有关校样的评论
* comment_replies.csv — 包括验证回复organization.csv — 包括数字标识符和您的组织名称（您的帐户）
* contacts.csv — 包含每个联系人的数字标识符、姓名和组织
* files.csv — 包含来自“验证详细信息”页面或“文件详细信息”页面的有关验证或上传到[!DNL Workfront Proof]的文件的信息
* recipients.csv — 包括在[!DNL Workfront Proof]上载验证以供审阅时指定为审阅者、审阅者和审批者等每个人的数字标识符、角色和决策
* users.csv — 包含数值标识符和帐户中所有用户的名称

您可以使用任何使用的zip实用程序从备份.zip文件中解压缩这些文件，然后将它们存储在计算机上您选择的位置。 保存zip文件并提取单个CSV文件后，您可以根据需要处理信息以保留内部记录。

根据您的请求创建的每个备份.zip文件都有一个独特的名称，其中包含备份创建日期，但每个备份.zip文件中包含的CSV文件始终具有相同的名称。 您可能希望使用以下方法之一来确保备份文件彼此不同：

* 为每个备份.zip文件以及从中提取的CSV文件创建一个新文件夹。
* 在从zip文件中提取每个CSV文件时，请重命名该文件以包含备份日期。

>[!NOTE]
>
>如果计算机上安装了[!DNL Microsoft Excel]，则提取实用程序可能会将各个CSV文件的文件类型列为[!DNL Microsoft Office Excel]逗号分隔值文件。 您可以使用[!DNL Excel]打开提取的CSV文件，并将文件另存为[!DNL Excel]工作簿(&#42;.xlsx)或某些其他文件类型。
