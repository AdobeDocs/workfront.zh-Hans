---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将webhook添加到基本场景
description: Webhook（也称为即时触发器）是一种特定的触发器模块，它可以在每次进行更改时启动一个场景，而不是按给定的计划启动。
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 将webhook添加到中的基本方案 [!DNL Adobe Workfront Fusion]

Webhook（也称为即时触发器）是一种特定的触发器模块，它可以在每次进行更改时启动一个场景，而不是按给定的计划启动。

在本例中，您将添加一个webhook ，以便在将任何请求提交到特定队列后立即启动方案。 然后，场景将这些请求转换为项目。

此示例修改了中创建的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 先决条件

您必须创建中所述的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) ，然后再执行该过程。

## 添加和配置webhook

1. 打开转换对象模块。
1. 在问题ID字段中，删除黑色ID块。 该块为黑色，因为映射该块的模块不再可用。
1. 选择第一个模块(Watch Events)下的ID块以将其映射到第二个模块。
1. 单击 **确定**.

### 添加webhook模块

1. 在方案编辑器中打开方案。
1. 右键单击第一个模块并选择 **删除模块**.

   模块被删除，留空占位符。

1. 单击空白模块，然后选择 **Adobe Workfront** 从应用程序列表中。
1. 选择 **观看活动**.
1. 单击 **添加** 在Webhook字段旁边。
1. 在记录类型字段中，选择 **问题**，因此模块会触发问题的更改。
1. 在State字段中，选择 **新建状态**. 这是用于筛选器的必填字段，本示例未涵盖该字段。
1. 在记录来源字段中，选择 **仅新记录**. 这允许场景在添加问题时触发，而不是在更新或删除问题时触发。
1. 单击 **保存** 以保存模块配置。


