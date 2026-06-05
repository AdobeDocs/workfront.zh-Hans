---
title: 授予对资源管理的访问权限
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中资源管理的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
TQID: https://experienceleague.adobe.com/K-SveIsDCsH7eskte0y96MwUlPoQ2FANImBY3RxshKo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: d3382524-5489-431b-bde9-271ab257bc37
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 8%

---

# 授予对资源管理的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对资源管理的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自定义访问级别配置用户对资源管理工具的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击资源管理右侧&#x200B;**查看**&#x200B;或&#x200B;**编辑**&#x200B;按钮上的齿轮图标![](assets/gear-icon-settings.png)，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在“规划者”中编辑优先级和预算小时数</td> 
      <td> <p>允许拥有此许可证的用户执行以下操作：</p> <p>在资源规划者中排定项目的优先级。</p> <p>资源计划工具中资源的预算分配（项目业务案例中的“资源计划者”和“资源预算”部分）。</p> <p>此选项默认处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理资源池</td> 
      <td> <p>允许拥有此许可证的用户创建、编辑和删除资源池。 默认禁用此选项。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">在工作负载均衡器<span>更新计划的小时数</span> </td> 
      <td> <p>允许具有此许可证的用户在工作负载均衡器更新用户分配时更新工作项的计划小时数。 分配小时总数将成为工作项的计划小时数。</p> <p>默认禁用此选项。</p> <p> 有关详细信息，请参阅<a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载均衡器</a>中管理用户分配。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 按许可证类型访问资源管理

有关每个访问级别中的用户可以执行哪些资源管理操作的信息，请参阅适用于每个对象类型[&#128279;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)的功能一文中的[资源管理](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource)部分。

## 访问共享的问题

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

当您与其他用户共享对象时，收件人在其上预算或查看资源分配的权限由3个因素共同决定：

* 收件人的资源管理访问级别设置
* 用户对财务数据的访问权限，如[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)中所述
* 共享者授予对象的财务数据的任何权限

有关用户在共享对象时可授予对象财务数据的权限的信息，请参阅[共享对象的财务权限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)。
