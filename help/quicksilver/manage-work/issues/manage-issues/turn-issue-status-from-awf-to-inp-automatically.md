---
product-area: projects
navigation-topic: manage-issues
title: 自动将问题状态从等待反馈更新为进行中
description: 当问题的主要联系人通过更新字段（包括自定义字段）或添加评论来更新问题时，问题状态会自动更新为进行中。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 0%

---

# 自动将问题状态从等待反馈更新为进行中

<!--Audited: 109/2025-->

当问题的主要联系人通过更新字段（包括自定义字段）或添加评论来更新问题时，问题状态会自动更新为进行中。

为了进行此自动状态更改，需要满足以下条件：

* 必须使用请求队列添加问题。

  有关创建请求队列的信息，请参阅[创建和管理请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md)部分。

  有关将请求提交到请求队列的信息，请参阅[创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

* 请求队列中的“队列详细信息”必须具有以下设置：
   * **当某人发出请求时，自动授予**&#x200B;设置为&#x200B;**参与访问**
   * 已选择&#x200B;**更改状态**

  ![已选择“队列详细信息”授予Contribute访问权限和更改状态。](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  设置请求队列时，您可以定义主要联系人对其提交的问题具有的访问权限。
  >
  >设置请求队列时取消选择更改状态设置时，请记住，系统管理员始终有权更改问题的状态，即使取消选择请求队列设置中的更改状态选项也是如此。

  有关队列详细信息的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

* 问题必须处于“等待反馈”状态。
* 对于系统级别的问题，必须具有“等待反馈(AWF)”状态。

  有关系统级状态的详细信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。
