---
title: 表单设计器概述
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以设计一个自定义表单，以便用户将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。
author: Courtney / Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# 表单设计器概述

您可以使用新的表单设计器来设计自定义表单，以便用户可以将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。

新的表单设计器具有新的画布样式工作区，该工作区允许您同时查看字段、画布和字段设置。 它还允许您在设计表单时拖放部分中的字段。

<!-- add screenshot when field settings empty state is ready -->

## 如何访问新的表单设计器

新表单设计器和旧表单生成器的顶部均有一个新按钮。 您可以使用此按钮在旧版生成器和新设计器之间切换。

![切换到新的窗体设计器](assets/switch-views.png)

## 表单设计器提供的新功能

通过新的表单设计器，我们添加了

* **复制字段**：您现在可以通过直接在画布中单击字段上的复制图标来复制现有字段。

* **更改描述性文本的大小**：您现在可以为“描述性文本”字段分配小型、中型或大型。 您还可以在同一行与其他字段一起使用它们。

* **使用默认部分**：如果表单创建者未在表单顶部添加分区，则画布中现在将显示默认分区，以便用户能够调整未分配自定义分区的字段的权限。

  >[!NOTE]
  >
  >将表单附加到对象后，默认部分在对象中不可见。

## 功能即将推出

以下内容目前在表单设计器中不可用，但很快将会添加：

* 显示/跳过逻辑

* 筛选预输入字段

>[!IMPORTANT]
>
>使用新表单设计器时，逻辑和预输入筛选器的现有配置不会受到影响。

### 显示/跳过逻辑

虽然在设计新的自定义表单时您尚无法添加显示/跳过逻辑，但您可以查看在旧版表单生成器中创建的表单上的现有显示/跳过逻辑。

表单设计器中字段上的图标指示逻辑应用于该字段。

此 ![目标字段的显示逻辑](assets/display-logic-bottom-left.png) 左下方的图标表示该字段是用于显示逻辑的目标字段（如果在表单上进行了特定选择，则会显示此字段）。 此 ![定义显示逻辑图标](assets/display-logic-bottom-right.png) 图标位于右下角表示该字段用于定义显示逻辑（此字段上的特定选择或值将显示目标字段）。

此 ![目标字段的跳过逻辑](assets/skip-logic-bottom-left.png) 左下方的图标表示该字段是用于跳过逻辑的目标字段（如果对表单进行了特定选择，则表单会向前跳过该字段）。 此 ![定义跳过逻辑图标](assets/skip-logic-bottom-right.png) 图标位于右下角表示该字段用于定义跳过逻辑（此字段上的特定选择或值将跳过其他字段并直接转到目标字段）。

![逻辑图标](assets/logic-icons-3.png)

选择应用了逻辑的字段会显示字段设置中的现有逻辑规则。

![逻辑规则](assets/form-designer-view-only-logic.png)

## 从表单设计器中移除的功能

我们从表单设计器内部删除了以下功能：


* 表单设置、表单共享、字段共享选项卡

   * 表单设置现在位于画布顶部

   * 表单共享主选项卡和字段共享子选项卡

  >[!NOTE]
  >
  >您可以通过设置>自定义Forms > Forms或字段选项卡控制表单和字段共享。

* 在更新提要中跟踪字段变化
  >[!NOTE]
  >
  >您可以在设置>界面>更新馈送中找到此链接
