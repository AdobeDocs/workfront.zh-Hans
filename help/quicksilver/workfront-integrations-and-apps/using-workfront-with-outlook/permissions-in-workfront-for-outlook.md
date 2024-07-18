---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 适用于Outlook的 [!DNL Workfront] 的权限级别
description: ' [!DNL Workfront for Outlook] 加载项需要读/写邮箱访问权限。  [!DNL Workfront for Outlook] 集成需要最高级别的权限，因为它具有从Outlook Exchange Server下载电子邮件附件并将附件上载到 [!DNL Workfront]的功能（当用户从具有附件的电子邮件提交请求时）。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!DNL Workfront for Outlook]的权限级别

[!DNL Workfront for Outlook]需要[!DNL Outlook]加载项中允许的四级权限中的最高级别。

有关[!DNL Outlook]加载项中权限的详细信息，请参阅[!DNL Microsoft]文档中的[ [!DNL Outlook] 加载项的隐私、权限和安全性](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)。

[!DNL Workfront for Outlook]加载项需要读取/写入邮箱访问权限(`ReadWriteMailbox`)，这是最高权限范围。
[!DNL Workfront for Outlook]集成需要最高级别的权限，因为它具有从[!DNL Outlook] Exchange服务器下载电子邮件附件并将它们上载到[!DNL Workfront]的功能（当用户提交具有附件的电子邮件中的请求时）。 为使此功能正常工作，[!DNL Workfront for Outlook]使用来自[!DNL Office]外接程序JavaScript API的功能`mailbox.getCallbackTokenAsync()`获取令牌并使用该令牌从Exchange服务器下载电子邮件附件。 唯一允许使用该函数的权限是`ReadWriteMailbox`。 有关详细信息，请参阅Microsoft文档中的[Outlook加载项的隐私、权限和安全性](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)。

[!DNL Workfront for Outlook]加载项还需要`ReadWriteItem`权限（包含在`ReadWriteMailbox`中），该权限用于读取电子邮件正文和读取/更新电子邮件元数据：

* 阅读电子邮件正文：

  当用户提交请求或将电子邮件正文作为更新发送到[!DNL Adobe Workfront]对象时，[!DNL Workfront for Outlook]会读取电子邮件正文。
* 读取/更新电子邮件元数据：

  当用户通过电子邮件提交请求时，[!DNL Workfront for Outlook]会更新电子邮件标头。 此操作是为了存储有关已提交的[!DNL Adobe Workfront]对象的信息，因此下次用户打开同一电子邮件的加载项时，将显示有关该电子邮件中先前操作的信息。

[!DNL Workfront for Outlook]仅在用户在该加载项中执行操作时访问用户的邮箱。 它没有任何背景功能。 Workfront for Outlook仅在以下情况下访问用户的邮箱：

* 用户尝试从[!DNL Workfront for Outlook]提交请求、创建任务或发送电子邮件作为更新（打开加载项并选择操作）
   * [!DNL Workfront for Outlook]读取要填充到加载项内表单中的电子邮件正文。
   * [!DNL Workfront for Outlook]读取电子邮件元数据，以便在加载项上显示与同一电子邮件在该加载项中执行的先前操作有关的信息。
* 当用户提交请求、创建任务或从[!DNL Workfront for Outlook]发送电子邮件作为更新时（单击加载项上的[!UICONTROL submit]按钮）：
   * [!DNL Workfront for Outlook]读取电子邮件正文以将其作为请求描述或注释发送到Workfront。
   * [!DNL Workfront for Outlook]更新电子邮件元数据以存储有关已提交的请求或已更新对象的信息。
   * [!DNL Workfront for Outlook]从exchange服务器下载电子邮件附件，以上载到已提交的请求、已创建的任务或已更新的对象。
