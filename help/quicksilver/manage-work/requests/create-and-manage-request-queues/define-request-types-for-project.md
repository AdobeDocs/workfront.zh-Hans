---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定义项目的请求类型
description: 您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 7%

---

# 定义项目的请求类型

<!-- Audited: 6/2025 -->

您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。 这对于报告相关原因以及帮助用户了解在项目存留期内可能会发生何种意外工作非常有用。

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
   <td>
    <p>标准</p>
    <p>规划</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，必须执行以下操作：

* 拥有或创建项目。

  有关创建项目的信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

## 有关请求类型的注意事项

* 在为项目配置队列详细信息区域时，您可以指定可在项目中记录的问题或请求类型。
* 您无需使项目成为请求队列即可为项目定义请求类型。 为项目记录的任何问题都可以标记为不同的请求类型。
* 如果您将队列主题添加到项目中，则必须在每个队列主题上定义请求类型，以便在添加新问题或请求时显示它。 有关详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

## 定义项目的问题或请求类型

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 在左侧面板中，单击&#x200B;**队列详细信息**。
1. 在&#x200B;**队列属性**&#x200B;部分中，为项目选择所需的&#x200B;**请求类型**：
   * 错误报告
   * 更改顺序
   * 问题
   * 请求

   >[!NOTE]
   >
   >* 您必须至少选择一个请求类型。 您可以选择多种类型。
   >* 您的Workfront管理员可能已重命名其中一些选项。 有关信息，请参阅[配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 单击 **Save**。 在任务或项目上输入新问题时，或在向项目提交新请求时（如果项目已作为请求队列启用），您指定的请求类型将可供选择。
