---
product-area: projects
navigation-topic: approvals
title: 连接Workfront和Frame.io
description: Workfront在审核和批准流程中使用Frame.io来会见希望工作的人。 项目管理和批准流程在Workfront中进行管理，审查流程在Frame.io中完成。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: f50d102eb9c44abb9780c378c41c108b124077c4
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# 连接Workfront和Frame.io

Workfront在审核和批准流程中使用Frame.io来会见希望工作的人。 项目管理和批准流程在Workfront中进行管理，审查流程在Frame.io中完成。 您必须完成以下所有部分才能成功设置集成：

* [将Workfront组连接到Frame.io组](#connect-a-workfront-group-to-a-frameio-team)
* [创建Workfront项目并添加连接的组](#create-a-workfront-project-and-add-a-connected-group)

>[!IMPORTANT]
>
>本文内容介绍更新的文档审批功能，该功能仅适用于特定帐户。 有关标准审批流程的信息，请参阅中列出的文章 [工作审批](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## 访问要求

* 您的组织必须手动载入才能使用本文中描述的功能。 有关更多信息，请参阅 [Adobe Workfront和Frame.io本机集成alpha：概述](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


## 将Workfront组连接到Frame.io组

我们正在积极改进这项功能，以便在5月全面推出。

### 先决条件

* 创建一个Frame.io团队以映射到Workfront组。
* 查找团队的API开发人员令牌。 有关更多信息，请参阅 [开发人员令牌](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) 在Frame.io开发人员网站上。

### 将Workfront组连接到Frame.io组

{{step-1-to-setup}}

1. 在左侧面板中，单击 **组**.
1. 选择现有组，或单击 **创建组**.
1. 在左侧面板中，单击 **连接到Frame.io**.
   ![](assets/connect-frame-group.png)
1. 输入API开发人员令牌。
1. 单击 **启动连接**.
1. （视情况而定）选择一个Frame.io帐户。

## 创建Workfront项目并添加连接的组

将Workfront组连接到Frame.io团队后，必须使用该连接的组创建项目。

### 先决条件

* 必须将Workfront组连接到Frame.io团队，如上一节所述。

### 创建Workfront项目并添加连接的组

{{step1-to-projects}}

1. 从头开始创建新项目或模板。 有关如何创建项目的信息，请参阅 [创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. 在左侧面板中，查找 **项目详细信息**.

1. 查找 **组** 字段，并删除默认组。

1. 在下拉菜单中，找到所需的组。 与Frame.io连接的组将显示Frame.io图标。
   ![](assets/add-frame-group.png)

1. 进行任何其他项目配置更改。

1. 单击 **保存更改**.

1. 继续下一部分。

### 添加任务并将集成状态设置为“活动”

>[!NOTE]
>
>当前不支持子任务。


1. 创建需要在Frame.io中填充的任务

1. 选择所需的任务，然后单击 **编辑**.

1. 滚动到 **自定义Forms** 部分，并查找Frame.io集成表单。

   >[!IMPORTANT]
   >
   >必须添加Frame.io连接的组才能在任务中查看此自定义表单。

1. 启用该复选框，然后选择 **活动**.
   ![](assets/frame-custom-form.png)

1. 单击 **保存更改**. 项目名称旁边会显示一个Frame.io图标。

1. 将用户或团队分配给任务。

   >[!NOTE]
   >
   >添加到任务中的用户或团队也会添加到Frame.io项目中。

1. 在项目文档区域上传任何文档或创意摘要。

项目仍未连接，您必须继续到下一部分以完成集成。

### 在Frame.io中启用项目

1. 更改状态，从 **规划** 到 **当前** 或等于当前值的自定义状态。 这样即可完成集成，并在Frame.io中生成项目、任务和任何文档。

项目名称旁边的Frame.io图标变为紫色，表示集成成功。 用户将收到一封邀请他们加入Frame.io项目的电子邮件。