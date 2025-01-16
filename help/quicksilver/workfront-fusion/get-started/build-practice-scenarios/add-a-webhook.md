---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将webhook添加到基本场景
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中将webhook添加到基本方案

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [将webhook添加到基本方案](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

Webhook（也称为即时触发器）是一种特定的触发器模块，它可以在每次进行更改时启动一个场景，而不是按给定的计划启动。

在本例中，您将添加一个webhook ，以便在将任何请求提交到特定队列后立即启动方案。 然后，场景将这些请求转换为项目。

此示例修改在[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中创建的方案。

## 先决条件

在执行此过程之前，您必须先创建[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中所述的方案。

## 添加和配置webhook

1. 打开转换对象模块。
1. 在问题ID字段中，删除黑色ID块。 该块为黑色，因为映射该块的模块不再可用。
1. 选择第一个模块(Watch Events)下的ID块以将其映射到第二个模块。
1. 单击&#x200B;**确定**。

### 添加webhook模块

1. 在方案编辑器中打开方案。
1. 右键单击第一个模块，然后选择&#x200B;**删除模块**。

   模块被删除，留空占位符。

1. 单击空白模块，然后从应用程序列表中选择&#x200B;**Adobe Workfront**。
1. 选择&#x200B;**观看活动**。
1. 单击Webhook字段旁边的&#x200B;**添加**。
1. 在“记录类型”字段中，选择&#x200B;**问题**，以便模块会触发问题的更改。
1. 在“状态”字段中，选择&#x200B;**新建状态**。 这是用于筛选器的必填字段，本示例未涵盖该字段。
1. 在“记录来源”字段中，选择&#x200B;**仅新建记录**。 这允许场景在添加问题时触发，而不是在更新或删除问题时触发。
1. 单击&#x200B;**保存**&#x200B;以保存模块配置。
