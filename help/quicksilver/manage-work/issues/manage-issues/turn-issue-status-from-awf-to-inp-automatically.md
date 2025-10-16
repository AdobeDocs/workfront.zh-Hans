---
product-area: projects
navigation-topic: manage-issues
title: 自动将问题状态从等待反馈更新为进行中
description: 当问题的主要联系人通过更新字段（包括自定义字段）或添加评论来更新问题时，问题状态会自动更新为进行中。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '281'
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
