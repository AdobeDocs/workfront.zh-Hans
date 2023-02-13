---
product-area: projects
navigation-topic: manage-issues
title: 自动将问题状态从“等待反馈”更新为“正在进行”
description: 当问题的主要联系人通过更新字段（包括自定义字段）或添加评论来更新问题时，问题状态会自动更新为“进行中”。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 自动将问题状态从“等待反馈”更新为“正在进行”

当问题的主要联系人通过更新字段（包括自定义字段）或添加评论来更新问题时，问题状态会自动更新为“进行中”。

为了进行此自动状态更改，需要满足以下条件：

* 必须通过请求队列输入问题。

   有关创建请求队列的信息，请参阅 [创建和管理请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) 中。 有关创建请求的信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 请求队列中的队列详细信息必须具有以下设置：
   * **当某人提出请求时，自动授予** 设置为 **Contribute访问**
   * **更改状态** 在“高级设置”下选择

   ![“队列详细信息”为Contribute提供访问权限，并且已选中“更改状态”。](assets/queuedetails-contributeaccess-changestatus.png)

   有关“队列详细信息”的详细信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* 问题必须处于“正在等待反馈”状态。
* 系统级别上的问题必须具有等待反馈(AWF)状态。

   有关系统级别状态的更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
