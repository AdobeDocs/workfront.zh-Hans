---
title: 表单设计器概述
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以设计一个自定义表单，用户可以将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# 表单设计器概述

您可以使用新的表单设计器来设计一个自定义表单，用户可以将其附加到Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。

新的表单设计器具有新的画布样式工作区，允许您同时查看字段、画布和字段设置。 它还允许您在设计表单时拖放部分中的字段。

<!-- add screenshot when field settings empty state is ready -->

## 如何访问新的表单设计器

新表单设计器和旧表单生成器的顶部都有一个新按钮。 您可以使用此按钮在旧版生成器和新设计器之间切换。

![](assets/switch-views.png)

## 表单设计器提供的新功能

通过使用新的表单设计器，我们在

* **复制字段**:现在，您可以通过直接从画布中单击字段上的复制图标来复制现有字段。

* **更改描述性文本的大小**:现在，您可以为描述性文本字段指定小、中或大大小。 您还可以在同一行上将它们与其他字段一起使用。

* **使用默认部分**:如果表单创建者未在表单顶部添加部分，则画布中现在会显示“默认”部分，以便用户可以调整未分配自定义部分的字段的权限。

   >[!NOTE]
   >
   >将表单附加到对象后，对象中不显示默认部分。

## 即将推出功能

表单设计器当前不提供以下内容，但不久将添加以下内容：

* 调整描述性文本的大小

* 显示/跳过逻辑

* 筛选提前类型字段

>[!IMPORTANT]
>
>使用新的表单设计器时，逻辑和Typeahead过滤器的现有配置不会受到影响。

## 从表单设计器中删除的功能

我们从表单设计器内部删除了以下功能：


* 表单设置、表单共享、字段共享选项卡

   * 表单设置现在在画布顶部可用

   * 表单共享主选项卡和字段共享子选项卡
   >[!NOTE]
   >
   >您可以通过设置>自定义Forms > Forms或字段选项卡控制表单和字段共享。

* 在更新提要中跟踪字段变化
   >[!NOTE]
   >
   >您可以在设置>界面>更新信息源中找到此信息
