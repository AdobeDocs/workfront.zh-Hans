---
title: 删除用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 当用户离开您的组织时，可以从Workfront中删除该用户，但我们建议停用而不是删除这些用户。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 7%
---
# 删除用户

>[!IMPORTANT]
>
>此页面上描述的过程仅适用于尚未载入Admin Console的组织。 由于您的组织已载入到Adobe Admin Console，因此您必须通过Adobe Admin Console执行此操作。
>
>  有关在Adobe Admin Console中删除用户的说明，请参阅[单独管理用户](https://helpx.adobe.com/cn/enterprise/using/manage-users-individually.html)一文中的“永久删除用户”一节，或与Adobe Admin Console管理员联系。

当用户离开您的组织时，您可以从Adobe Workfront中删除该用户。

必须通过Adobe Admin Console执行用户删除操作。 有关说明，请参阅[单独管理用户](https://helpx.adobe.com/cn/enterprise/using/manage-users-individually.html)一文中的“永久删除用户”一节，或联系您的Adobe Admin Console管理员。

>[!IMPORTANT]
>
>从系统中删除用户也会删除与您可能希望保留的用户相关联的信息。 我们建议停用而不是删除用户。 有关详细信息，请参阅[停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须是Adobe Admin Console的管理员。</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除与停用用户

停用用户会导致发生以下情况：

* 如果Workfront组件与您的Workfront Proof帐户关联，则删除用户对Workfront Proof和Workfront的许可证。 有关Workfront Proof的详细信息，请参阅[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
* 不能再为用户分配工作。
* 无法再将该用户添加到更新。
* 无法再向团队或组中添加用户。
* 无法再与用户共享对象。
* 它们与以下对象的关联保持不变：

  * 任务、问题、项目、项目组合
  * 仪表板

    >[!NOTE]
    >
    >如果您停用用户并且无法再查看与用户相关的报告或仪表板，则可能需要更新&#x200B;**使用**&#x200B;的访问权限运行此报告。\
    >要了解更多信息，请参阅[为什么无法访问已停用用户拥有的报告？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) [报告常见问题解答](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)文章的部分。

  * 文档
  * 更新
  * 小时

* 如果用户已签出文档，则当您取消激活这些文档时，它们仍保持签出状态。 只有Workfront管理员才能重新签入这些帐户。 有关签出文档的更多信息，请参阅[签出文档](../../../documents/managing-documents/check-out-documents.md)。

删除用户会导致发生以下情况：

* 如果Workfront组件与您的Workfront Proof帐户关联，请删除用户对Workfront Proof和Workfront的许可证。 有关Workfront Proof的详细信息，请参阅[Workfront Proof：文章索引](../../../workfront-proof/workfront-proof.md)。
* 不能再为用户分配工作。
* 无法再将该用户添加到更新。
* 无法再向团队或组中添加用户。
* 无法再与用户共享对象。
* 删除该用户与以下对象的关联：

  * 任务、问题、项目、项目组合
  * 仪表板

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* 更新
* 小时

  >[!NOTE]
  >
  >这些对象仍保留在Workfront中，但对象的所有者现在为空。

* 如果用户在“全局导航栏”的“文档”区域下上载了任何文档，则也会删除这些文档。
* 如果用户已签出他们拥有的文档，并且文档上载到主文档区域（从主菜单访问），则文档将随用户一起删除。 有关签出文档的更多信息，请参阅[签出文档](../../../documents/managing-documents/check-out-documents.md)。

有关停用用户的详细信息，请参阅[停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
