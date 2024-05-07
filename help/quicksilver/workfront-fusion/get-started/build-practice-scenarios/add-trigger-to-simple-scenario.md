---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将触发器模块添加到基本场景
description: 了解如何添加触发器模块，以允许方案定期查找新请求并将它们转化为项目。
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 将触发器模块添加到基本场景

触发器模块位于方案的开头。 当给定服务发生更改时，这些模块在特定标准下开始执行场景。 更改可以是创建新记录、删除记录、更新记录等。

轮询模块在设定的时间间隔检查服务，并返回有关在该时间间隔内发生更改的信息。 如果没有任何更改，则触发器不会执行场景。

在此示例中，您将添加一个每15分钟运行一次的触发器模块，如果有任何请求已提交到特定队列，则会启动一个方案。 然后，场景将这些请求转换为项目。

此示例修改了中创建的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 先决条件

您必须创建中所述的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) ，然后再执行该过程。

## 添加并配置触发器模块

### 添加触发器模块

1. 在方案编辑器中打开方案。
1. 右键单击第一个（搜索）模块并选择 **删除模块**.

   模块被删除，留空占位符。

1. 单击空白模块，然后选择 **Adobe Workfront** 从应用程序列表中。
1. 选择 **观看记录**.
1. 确保模块使用与场景中其余模块相同的连接。
1. 在筛选器字段中，选择 **仅新记录**.
1. 在输出框中，选择 `ID`， `Name`、和 `Project ID`.
1. 单击 **确定** 以保存模块设置。

   出现“Choose where to start（选择开始位置）”窗口。

1. 选择 **从现在起**.

### 计划触发器模块

1. 单击Watch Records模块的时钟。

   将打开“计划”设置窗口。

1. 在运行方案字段中，选择 **定期发送**.

1. 单击 **确定**.

### 更新第二个模块

由于第一个模块已被替换，因此第二个模块必须映射到新的第一个模块。

1. 打开转换对象模块。
1. 在问题ID字段中，删除黑色ID块。 该块为黑色，因为映射该块的模块不再可用。
1. 选择第一个模块（观察记录）下的ID块，以将其映射到第二个模块。
1. 单击 **确定**.

### 测试和激活

1. 转到Fusion所连接的Workfront环境并添加问题。
1. 单击 **[!UICONTROL 运行一次]** 位于场景编辑器的左下角。
1. 检查输出以确保方案按预期运行。
1. 如果您对方案按预期工作感到满意，请单击 **正在计划** 在屏幕左下角切换到 **开启**.

   这将激活方案。
1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** 左下角附近，保存场景的进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 资源

* 有关Webhook的更多信息，请参阅 [中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
