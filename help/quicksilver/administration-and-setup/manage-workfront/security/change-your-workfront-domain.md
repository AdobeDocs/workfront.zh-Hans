---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 更改Adobe Workfront域
description: 作为Adobe Workfront管理员和经授权的Workfront支持联系人，您可以向Workfront支持团队请求帮助，以更改贵组织的Workfront域。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
TQID: https://experienceleague.adobe.com/g9H5AYcIdsVccGIU9U97QPa37J9Y3pXziZRQR7pvjpQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 11%

---

# 更改Adobe Workfront域

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>此页面上描述的过程仅适用于尚未载入Admin Console的组织。 由于所有组织现在都已登记到Adobe Admin Console，**无法更改您的Workfront域**。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[Adobe Workfront与Adobe业务平台之间的管理差异](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
>
>本文将于近期移除。

作为Adobe Workfront管理员和经授权的Workfront支持联系人，您可以向Workfront支持团队请求帮助，以更改贵组织的Workfront域。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 请求域更改

1. 开始在Experience League上创建支持工单。
1. 在&#x200B;**描述**&#x200B;框中，包含所需的新域，以及希望新域上线的时间范围。
1. 完成填写支持案例的框，然后单击&#x200B;**提交**。

您还可以致电Workfront支持，获取有关更改域的帮助。

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
