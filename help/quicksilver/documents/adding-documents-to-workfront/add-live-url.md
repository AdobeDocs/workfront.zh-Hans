---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 将Web链接添加为文档
description: 您可以将网站作为Web链接添加到Adobe Workfront中并请求获得批准。
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 05f148f2c28555e37fb415f606e314a5df564047
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 4%
---
# 将Web链接添加为文档

您可以从新的“文档”区域将网站作为Web链接添加到Adobe Workfront。 添加后，您可以像请求审批已上传文件一样请求审批实时网页。

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>使用旧版Workfront存储管理文档的任何Workfront软件包</p>
<p>用于使用Adobe云存储管理文档的任意工作流包</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>旧版Workfront Storage：编辑对文档的访问权限</p> 
   <p>Adobe云存储：默认情况下会启用对文档的编辑访问权限，无法对其进行更改</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将Web链接添加为文档

您可以将html网页作为Web链接上传到Workfront。 添加后，您可以像请求审批已上传文件一样请求审批实时网页。 有关Frame.io如何处理Web链接的更多信息，请参阅[HTML Review for Frame.io](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links)。


>[!IMPORTANT]
>
>* 如果网站允许嵌入iFrame，则支持URL。
>* 支持专用Web URL，但某些身份验证流程可能因服务器配置而不起作用。
>* 当前不支持Youtube和Figma URL。<br>
>有关详细信息，请参阅[HTML对Frame.io的审查](https://help.frame.io/en/articles/12893213-html-review-for-frame-io)。


要添加Web链接，请执行以下操作：

1. 转到要添加网站的项目、任务或问题，然后在左侧面板中选择&#x200B;**文档**。
1. 单击&#x200B;**新建**，然后选择&#x200B;**Web链接**。
1. 在&#x200B;**文档名称**&#x200B;字段中输入名称，然后在&#x200B;**URL**&#x200B;字段中输入网站的地址。
1. 单击&#x200B;**添加**。
   ![将Web链接添加为文档](assets/web-url.png)

若要请求审批Web链接，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

## 已知限制

* 在Frame.io中创建的Web链接文档存在临时问题。 如果您在Frame.io中创建Web链接，然后在Workfront中对其创建批准，则文档不会在Frame.io中打开。 在Workfront中创建的Web链接不会受到影响。 在解决此问题之前，请先在Workfront中创建Web链接文档，然后再开始审批。
* 当前无法在Frame.io中创建Web链接文档的新版本。 如果您需要创建Web链接文档的新版本，请在Workfront中创建新版本。