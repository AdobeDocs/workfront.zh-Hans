---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 权限级别 [!DNL Workfront] for Outlook
description: 的 [!DNL Workfront for Outlook] 外接程序需要读/写邮箱访问权限。 的 [!DNL Workfront for Outlook] 集成需要最高级别的权限，因为它具有从Outlook exchange服务器下载电子邮件附件并将其上传到的功能 [!DNL Workfront]，用户从具有附件的电子邮件提交请求时。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 权限级别 [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] 需要中允许的四个级别中的最高权限 [!DNL Outlook] 加载项。

有关 [!DNL Outlook] 加载项，请参阅 [隐私、权限和安全性 [!DNL Outlook] 加载项](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) 在 [!DNL Microsoft] 文档。

的 [!DNL Workfront for Outlook] 加载项需要读/写邮箱访问(`ReadWriteMailbox`)，这是权限范围最高的值。
的 [!DNL Workfront for Outlook] 集成需要最高级别的权限，因为它能够从 [!DNL Outlook] exchange服务器，并将其上传到 [!DNL Workfront]，用户从具有附件的电子邮件提交请求时。 要使此功能正常工作， [!DNL Workfront for Outlook] 使用函数 `mailbox.getCallbackTokenAsync()` 从 [!DNL Office] 插件JavaScript API以获取令牌，并使用该令牌从exchange服务器下载电子邮件附件。 允许使用该函数的唯一权限是 `ReadWriteMailbox`. 有关更多信息，请参阅 [Outlook加载项的隐私、权限和安全性](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) (在Microsoft文档中)。

的 [!DNL Workfront for Outlook] 此外， `ReadWriteItem` 权限(包括 `ReadWriteMailbox`)，用于读取电子邮件正文和读取/更新电子邮件元数据：

* 阅读电子邮件正文：

   [!DNL Workfront for Outlook] 在用户提交请求时读取电子邮件正文，或将电子邮件正文作为更新发送到 [!DNL Adobe Workfront] 对象。
* 读取/更新电子邮件元数据：

   [!DNL Workfront for Outlook] 当用户提交来自电子邮件的请求时，会更新电子邮件标题。 这样做是为了存储有关已提交 [!DNL Adobe Workfront] 对象，因此下次用户为同一电子邮件打开加载项时，将显示有关该电子邮件先前操作的信息。

[!DNL Workfront for Outlook] 仅当用户在加载项中执行操作时，才会访问用户的邮箱。 它没有任何后台功能。 Workfront for Outlook仅在以下情况下访问用户邮箱：

* 用户尝试提交请求、创建任务或发送电子邮件作为 [!DNL Workfront for Outlook] （打开加载项并选择操作）
   * [!DNL Workfront for Outlook] 读取要在加载项内的表单中填充的电子邮件正文。
   * [!DNL Workfront for Outlook] 读取电子邮件元数据，以显示有关加载项的信息，以了解有关在加载项中通过同一电子邮件执行的操作的先前操作。
* 当用户提交请求、创建任务或发送电子邮件作为 [!DNL Workfront for Outlook] (单击 [!UICONTROL 提交] 按钮):
   * [!DNL Workfront for Outlook] 读取电子邮件正文，以请求描述或评论的形式将其发送到Workfront。
   * [!DNL Workfront for Outlook] 更新电子邮件元数据，以存储有关已提交请求或已更新对象的信息。
   * [!DNL Workfront for Outlook] 从exchange服务器下载电子邮件附件以上载到已提交的请求、已创建的任务或已更新的对象。
