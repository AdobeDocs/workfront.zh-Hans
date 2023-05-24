---
title: 表单设计器概述
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以设计一个自定义表单，用户可将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 061d1a08a8c99b2770491ce2fcea63a9dad7a63f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 1%

---

# 表单设计器概述

>[!IMPORTANT]
>
>2023年5月24日，窗体设计人员被暂时禁用。 您可以使用旧版表单生成器创建和编辑自定义表单。 参见 [使用旧版表单生成器创建或编辑自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/use-the-custom-form-builder.md).

您可以使用新的表单设计器来设计自定义表单，以便用户可以将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。

新的表单设计器具有新的画布样式工作区，该工作区允许您同时查看字段、画布和字段设置。 它还允许您在设计表单时拖放部分中的字段。

<!-- add screenshot when field settings empty state is ready -->

## 如何访问新的表单设计器

新表单设计器和旧表单生成器的顶部都有一个新按钮。 您可以使用此按钮在旧版生成器和新设计器之间切换。

![](assets/switch-views.png)

## 表单设计器提供的新功能

通过新的表单设计器，我们添加了

* **复制字段**：您现在可以通过直接在画布中单击字段上的复制图标来复制现有字段。

* **更改描述性文本的大小**：您现在可以为描述性文本字段分配小尺寸、中尺寸或大尺寸。 您也可以将它们与其他字段在同一行上使用。

* **使用默认部分**：如果表单创建者尚未在表单顶部添加分区，则画布中现在将显示默认分区，以便用户能够调整未分配自定义分区的字段的权限。

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

## 从表单设计器中移除的功能

我们已从窗体设计器中删除了以下功能：


* 表单设置、表单共享、字段共享选项卡

   * 表单设置现在位于画布顶部

   * 表单共享主选项卡和字段共享子选项卡
   >[!NOTE]
   >
   >您可以通过设置>自定义Forms > Forms或字段选项卡控制表单和字段共享。

* 在更新提要中跟踪字段变化
   >[!NOTE]
   >
   >您可以在设置>界面>更新馈送中找到此项
