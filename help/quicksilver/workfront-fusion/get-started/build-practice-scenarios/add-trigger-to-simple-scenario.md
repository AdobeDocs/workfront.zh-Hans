---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将触发器模块添加到基本场景
description: 了解如何添加触发器模块，以允许方案定期查找新请求并将它们转化为项目。
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 将触发器模块添加到基本场景

触发器模块位于方案的开头。 当给定服务发生更改时，这些模块在特定标准下开始执行场景。 更改可以是创建新记录、删除记录、更新记录等。

轮询模块在设定的时间间隔检查服务，并返回有关在该时间间隔内发生更改的信息。 如果没有任何更改，则触发器不会执行场景。

在此示例中，您将添加一个每15分钟运行一次的触发器模块，如果有任何请求已提交到特定队列，则会启动一个方案。 然后，场景将这些请求转换为项目。

此示例修改在[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中创建的方案。

## 先决条件

在执行此过程之前，您必须先创建[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中所述的方案。

## 添加并配置触发器模块

### 添加触发器模块

1. 在方案编辑器中打开方案。
1. 右键单击第一个（搜索）模块并选择&#x200B;**删除模块**。

   模块被删除，留空占位符。

1. 单击空白模块，然后从应用程序列表中选择&#x200B;**Adobe Workfront**。
1. 选择&#x200B;**监视记录**。
1. 确保模块使用与场景中其余模块相同的连接。
1. 在筛选器字段中，选择&#x200B;**仅新记录**。
1. 在记录类型字段中，选择&#x200B;**问题**。
1. 在输出框中，选择`ID`、`Name`和`Project ID`。
1. 单击&#x200B;**确定**&#x200B;以保存模块设置。

   出现“Choose where to start（选择开始位置）”窗口。

1. 从&#x200B;**开始选择**。

### 计划触发器模块

1. 单击Watch Records模块的时钟。

   将打开“计划”设置窗口。

1. 在“运行方案”字段中，选择&#x200B;**定期**。

1. 单击&#x200B;**确定**。

### 更新第二个模块

由于第一个模块已被替换，因此第二个模块必须映射到新的第一个模块。

1. 打开转换对象模块。
1. 在问题ID字段中，删除黑色ID块。 该块为黑色，因为映射该块的模块不再可用。
1. 选择第一个模块（观察记录）下的ID块，以将其映射到第二个模块。
1. 单击&#x200B;**确定**。

### 测试和激活

1. 转到Fusion所连接的Workfront环境并添加问题。
1. 在方案编辑器的左下角单击&#x200B;**[!UICONTROL 运行一次]**。
1. 检查输出以确保方案按预期运行。
1. 如果您满意方案按预期工作，请单击屏幕左下角的&#x200B;**计划**&#x200B;切换开关至&#x200B;**开启**。

   这将激活方案。
1. 在[!DNL Workfront Fusion]中，单击左下角附近的&#x200B;**[!UICONTROL 保存]**&#x200B;以保存方案进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 资源

* 有关webhook的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即时触发器(webhook)。
