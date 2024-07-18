---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将触发器模块添加到基本场景
description: 了解如何添加触发器模块，以允许方案定期查找新请求并将它们转化为项目。
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 使用函数在[!DNL Adobe Workfront Fusion]中更新简单方案中的项目

更新Workfront工作项是Workfront Fusion的常见用例。 在此示例中，您将使用函数将项目名称更改为大写字母。

Fusion包括多种类型的函数，可用于转换数据并对数据执行条件逻辑。 有关使用函数的更多信息，请参阅[在Adobe Workfront Fusion中将信息从一个模块映射到另一个模块](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)。

此示例修改在[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中创建的方案。

## 先决条件

在执行此过程之前，您必须先创建[创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中所述的方案。

## 使用函数更新项目

### 将“更新记录”模块添加到方案

1. 在方案编辑器中打开方案。
1. 将鼠标悬停在模块右侧的部分圆圈上，然后单击“**[!UICONTROL 添加其他模块]**”。
1. 从应用程序列表中选择[!DNL Adobe Workfront]，然后选择模块&#x200B;**[!UICONTROL 更新记录]**。
1. 在ID字段中，选择转换对象模块下的ID块。 这是该模块输出的项目的ID。

   转换对象中的![ID](assets/id-convert-object.png)

1. 在“记录类型”字段中，选择“项目”，因为要更新的对象是项目。
1. 在“选择要映射的字段”区域，选择“名称”。

   将会打开“名称”字段。

### 映射函数以进行名称更新

当此方案将请求转换为项目时，项目的名称与请求相同。 此函数会采用此名称并将其中的所有字母转换为大写。

1. 单击&#x200B;**名称**&#x200B;字段。

   将打开映射面板。
1. 在映射面板中，单击&#x200B;**文本和二进制函数**&#x200B;图标。 ![文本函数图标](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. 选择函数&#x200B;**upper**。

   函数将显示在“名称”字段中，包括预期输入的格式。

   此示例的输入是项目转换来源问题的名称。

1. 将光标在括号之间移动，因为这是输入将移动的位置。
1. 在映射面板中，单击&#x200B;**模块输出**&#x200B;图标。 ![模块输出图标](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. 选择第一个模块输出的名称块。

   名称块显示在函数中。

   ![函数中的名称块](assets/map-name.png)

1. 单击确定以保存模块设置。

### 测试和激活

1. 单击屏幕左下角的&#x200B;**运行一次**&#x200B;以测试方案。
1. 检查输出以确保方案按预期运行。
1. 如果您满意方案按预期工作，请单击屏幕左下角的&#x200B;**计划**&#x200B;切换开关至&#x200B;**开启**。

   这将激活方案。 活动场景根据触发器模块中设置的计划运行。
1. 在[!DNL Workfront Fusion]中，单击左下角附近的&#x200B;**[!UICONTROL 保存]**&#x200B;以保存方案进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 资源：

* [使用 [!DNL Adobe Workfront Fusion]中的函数映射项](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
