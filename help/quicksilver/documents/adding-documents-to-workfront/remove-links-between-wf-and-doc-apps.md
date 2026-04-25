---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 删除Adobe Workfront和外部文档存储提供商之间的链接
description: When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# 删除Adobe Workfront和外部文档存储提供商之间的链接

When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.

For information about linking external document services to Workfront, see [Linking Documents from External Applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Since the document service is the one allowing permission to link to Workfront, it is not possible for Workfront to remove the permission granted by the document service. You must remove the permission from within the document service application or you must call our Support Team to remove this link from our servers.

>[!NOTE]
>
>This functionality is not available in the new documents area.<br>
>If your organization uses enterprise storage, you will see the new documents area when you access documents in Workfront. For more information about enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   <p>参与者或更高版本</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>Edit access to Documents</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Remove the link between Workfront and Dropbox

1. Log in to Dropbox.
1. Click your profile picture in the upper right corner, then click **Settings**.
1. Click the **Connected apps** tab, then scroll down to **Linked apps**.

1. Click the **X** next to Workfront.

## Remove the link between Workfront and Box

1. Log in to your Box account.
1. 单击右上角的配置文件图片。
1. 单击&#x200B;**帐户设置**，然后单击&#x200B;**安全性**&#x200B;选项卡。

1. 找到&#x200B;**MyWorkfront**&#x200B;并单击“忘记应用程序”下的&#x200B;**X**。

## 删除Workfront和Google驱动器之间的链接

1. 登录到您的Google Drive。
1. 单击右上角的齿轮图标，然后单击&#x200B;**设置**。
1. 单击左侧的&#x200B;**管理应用程序**，并在列表中找到&#x200B;**Workfront**。

1. 在“选项”下拉菜单下，单击&#x200B;**断开与驱动器的连接**。

## 删除Workfront和其他文档存储提供商之间的链接

要从Workfront断开Microsoft One Drive或WebDAM的连接，您必须致电我们的支持团队。

有关联系我们的支持团队的信息，请参阅[联系客户支持](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。
