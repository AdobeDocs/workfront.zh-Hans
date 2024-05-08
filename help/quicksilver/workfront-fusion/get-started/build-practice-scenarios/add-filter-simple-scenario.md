---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 将筛选器添加到基本方案
description: 通过过滤器，您可以确保场景仅在满足某些条件时推进。
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# 将过滤器添加到中的基本方案 [!DNL Adobe Workfront Fusion]

通过过滤器，您可以确保场景仅在满足某些条件时推进。

在此示例中，您将向场景添加一个过滤器，该过滤器允许仅当请求已提交到特定请求队列时，才从请求创建新项目。

此示例修改了中创建的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront触发器模块包括过滤器，这些过滤器允许仅在满足某些条件时才启动方案。 但是，由于模块间过滤器用于每个非触发器和非Workfront用例，因此了解如何在模块之间使用过滤器非常重要。 此示例将模块间过滤器用于可能与模块内过滤器相符的功能。

## 先决条件

您必须创建中所述的方案 [创建基本方案](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) ，然后再执行该过程。

## 添加筛选器

### 准备添加过滤器

1. 打开第一个方案。
1. 在 **输出** 区域，选择 `Project`.
您现在应该拥有 `ID`， `Name`、和 `Project` 已选定。
1. 单击确定以保存模块设置。
1. 打开Workfront。
1. 在Workfront中，找到表示Fusion场景将使用的请求队列的项目。

   此项目必须位于为Fusion连接设置的Workfront帐户中。

1. 在URL中记下项目ID。

   示例： https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### 添加并配置过滤器

1. 在方案编辑器中打开方案。
1. 单击扳手图标 ![“扳手”图标](assets/wrench-icon.png) 在第一模块和第二模块之间，并选择 **设置过滤器**.
1. 在标签字段中，输入此过滤器的标签，如“过滤请求队列”。
1. 在 **条件** 区域，在顶部字段中，映射 `projectID` 第一个模块中的。

   ![映射项目ID](assets/map-proj-id.png)
1. 离开 **条件** 运算符为Equal to。
1. 在 **条件** 区域中，粘贴您从项目URL中记录的项目ID [准备添加过滤器](#prepare-to-add-the-filter).
1. 单击 **确定** 以保存过滤器设置。

### 测试和激活

1. 转到Fusion所连接到的Workfront环境，并将问题添加到您在筛选器中指定的项目。 将另一个问题添加到其他项目。
1. 单击 **[!UICONTROL 运行一次]** 位于场景编辑器的左下角。
1. 检查输出以确保方案按预期运行。

   这两个问题都应该显示在第一个方案的输出中，但只有指定项目中的问题应该显示为第二个方案的输入，
1. 如果您对方案按预期工作感到满意，请单击 **正在计划** 在屏幕左下角切换到 **开启**.

   这将激活方案。
1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** 左下角附近，保存场景的进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 资源

* 有关筛选器的更多信息，请参阅 [将过滤器添加到方案](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

