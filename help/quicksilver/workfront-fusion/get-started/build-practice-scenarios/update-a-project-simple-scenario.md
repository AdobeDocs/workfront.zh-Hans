---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将触发器模块添加到基本场景
description: 了解如何添加触发器模块，以允许方案定期查找新请求并将它们转化为项目。
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 在中使用函数更新简单方案中的项目 [!DNL Adobe Workfront Fusion]

更新Workfront工作项是Workfront Fusion的常见用例。 在此示例中，您将使用函数将项目名称更改为大写字母。

Fusion包括多种类型的函数，可用于转换数据并对数据执行条件逻辑。 有关使用函数的更多信息，请参见 [在Adobe Workfront Fusion中将信息从一个模块映射到另一个模块](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

此示例修改了中创建的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 先决条件

您必须创建中所述的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) ，然后再执行该过程。

## 使用函数更新项目

### 将“更新记录”模块添加到方案

1. 在方案编辑器中打开方案。
1. 将鼠标悬停在模块右侧的部分圆上，然后单击 **[!UICONTROL 添加另一个模块]**.
1. 选择 [!DNL Adobe Workfront] 从应用程序列表中，选择模块 **[!UICONTROL 更新记录]**.
1. 在ID字段中，选择转换对象模块下的ID块。 这是该模块输出的项目的ID。

   ![转换对象中的ID](assets/id-convert-object.png)

1. 在“记录类型”字段中，选择“项目”，因为要更新的对象是项目。
1. 在“选择要映射的字段”区域，选择“名称”。

   将会打开“名称”字段。

### 映射函数以进行名称更新

当此方案将请求转换为项目时，项目的名称与请求相同。 此函数会采用此名称并将其中的所有字母转换为大写。

1. 单击 **名称** 字段。

   将打开映射面板。
1. 在映射面板中，单击 **文本和二进制函数** 图标。 ![“文本函数”图标](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. 选择函数 **upper**.

   函数将显示在“名称”字段中，包括预期输入的格式。

   此示例的输入是项目转换来源问题的名称。

1. 将光标在括号之间移动，因为这是输入将移动的位置。
1. 在映射面板中，单击 **模块输出** 图标。 ![模块输出图标](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. 选择第一个模块输出的名称块。

   名称块显示在函数中。

   ![在函数中命名块](assets/map-name.png)

1. 单击确定以保存模块设置。

### 测试和激活

1. 通过单击测试方案 **运行一次** 屏幕左下角的。
1. 检查输出以确保方案按预期运行。
1. 如果您对方案按预期工作感到满意，请单击 **正在计划** 在屏幕左下角切换到 **开启**.

   这将激活方案。 活动场景根据触发器模块中设置的计划运行。
1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** 左下角附近，保存场景的进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 资源：

* [使用中的函数映射项目 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
