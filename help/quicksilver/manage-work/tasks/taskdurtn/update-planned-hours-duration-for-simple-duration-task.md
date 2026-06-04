---
product-area: projects
navigation-topic: task-duration
title: 使用简单持续时间类型更新任务的已计划小时数和持续时间
description: 默认情况下，Adobe Workfront会根据已计划小时数计算具有简单持续时间类型的任务的持续时间。 但是，您还可以在Workfront的某些区域中手动编辑简单持续时间任务的规划小时数和持续时间。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SLemiOnFj-dOnWtXjH6gNzHZdVaXfp47qB0xzVJkRck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 450
ht-degree: 6%

---

# 使用简单持续时间类型更新任务的已计划小时数和持续时间

默认情况下，Adobe Workfront会根据已计划小时数计算具有简单持续时间类型的任务的持续时间。 但是，您还可以在Workfront的某些区域中手动编辑简单持续时间任务的规划小时数和持续时间。

您可以在任务层的“分配”区域内联或任务层编辑具有“简单持续时间类型”的任务的已计划小时数和持续时间。

有关内联编辑信息的详细信息，请参阅[在Adobe Workfront的列表中内联编辑项](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)。

本文介绍如何在任务级别的“工作总揽”区域使用“简单持续时间类型”更新任务的已计划小时数和持续时间。

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准或更高版本</p> 
   <p>工作版或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p> <p>编辑任务访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对任务的访问 </p></td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 使用简单持续时间类型更新任务的已计划小时数和持续时间

>[!IMPORTANT]
>
>手动更新简单持续时间任务的持续时间后，Workfront将停止根据计划小时数计算持续时间。

要在高级工作分配框中编辑具有简单持续时间类型的任务的已计划小时数和持续时间，请执行以下操作：

1. 在任务列表中，单击要更改持续时间类型的任务的名称。
1. 执行下列操作之一：

   * 单击任务名称旁边对象![&#128279;](assets/qs-more-icon-on-an-object.png)上的&#x200B;**更多**&#x200B;图标更多，单击&#x200B;**编辑**，然后单击&#x200B;**分配**。
   * 单击任务标题的“工作总揽”区域中的&#x200B;**分配给**&#x200B;或工作总揽的名称，然后单击&#x200B;**高级**。

1. 为所有分配输入&#x200B;**计划小时数**&#x200B;的总值，例如10小时。 计划小时数总数在分配给任务的所有资源之间平均分配。
1. （可选）手动调整分配给任务的每个资源的计划小时数。 任务更新的计划小时数总数，以反映单独分配给资源的新小时数。
1. 输入任务&#x200B;**持续时间**&#x200B;的值，例如2天。

   ![高级工作分配简单持续时间多个资源](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 单击&#x200B;**保存**。
