---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 自动化工作流阶段概述
description: 校样阶段是不同用户查看校样的时间段。 当校样从一个阶段移动到下一个阶段时，Adobe Workfront会通知审阅人在需要处理它时通知他们。
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 自动化工作流阶段概述

校样阶段是不同用户查看校样的时间段。 当校样从一个阶段移动到下一个阶段时，Adobe Workfront会通知审阅人在需要处理它时通知他们。

![stages_diagram.png](assets/stages-diagram-350x63.png)

阶段分为两个不同的情况：

* [使用自动工作流创建校样](#create-a-proof-with-an-automated-workflow)
* [为校样的不同审阅人指定截止时间](#assign-deadlines-for-different-reviewers-on-a-proof)

## 使用自动工作流创建校样 {#create-a-proof-with-an-automated-workflow}

向校样添加自动工作流时，您可以设置要进行的审阅工作的阶段。

使用自动工作流为校样设置阶段时：

* 您可以将阶段配置为连续运行或同时运行。
* 您可以将某些阶段配置为仅在上一个阶段完成后才处于活动状态。
* 你可以将某些阶段设为私有。 例如，对于在与客户共享证据之前对证据进行审查，并且不希望客户看到由此产生的评论的代理而言，这非常有用。

有关使用自动工作流创建校样的阶段的说明，请参阅 [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>如果用户未包含在任何阶段中，但有权访问文档并打开校样，则系统将创建一个名为 *Workfront*.
>
>为打开校样的用户分配了在设置>审阅和批准>角色中为打开文档校样的非收件人指定的角色。

## 为校样的不同审阅人指定截止时间 {#assign-deadlines-for-different-reviewers-on-a-proof}

当您为校样的审阅人指定不同的校样截止日期时，系统会为每个截止日期创建一个阶段，并在相应的阶段为每个截止日期对审阅人进行分组。 

**示例：** 例如，如果您创建一个由四位审阅人进行的校样：

* 对于Olivia和Tony的评论者，你指定了14:00的截止时间。
* 对亚伦和艾米来说，你指定几天后17:00的最后期限。
* 你没有为自己指定期限。

系统为以下三个“组”审阅人创建一个阶段：

![stages.png](assets/stages-350x239.png)

如果您与其他审阅人共享校样，但没有指定截止日期，则Workfront会将用户添加到没有截止日期的阶段3。 
