---
title: 2023年第四季度管理员增强功能
description: 2023年第四季度管理员增强功能
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# 2023年第四季度管理员增强功能

本页介绍了在2023年第四季度版本中对“预览”环境所做的所有管理员增强。 这些增强功能将在23.10版本的生产环境中提供。

有关2023年第四季度发布周期中此时可用的所有更改列表，请参阅 [2023年第四季度发行版概述](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## 自定义表单上的计算字段现在可以使用$$USER通配符

此 `$$USER` 通配符现在可用于新表单设计器的计算自定义字段和外部查找字段中。 引用 `$$USER` 在计算中，添加当前用户的ID。 您还可以将通配符与其他字段一起使用。 例如， `$$USER.{name}` 将添加当前用户的名称。

有关计算字段的更多信息，请参阅 [使用表单设计器添加计算字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## 将外部API中的值选项添加到自定义表单

新的字段类型， **外部查找**&#x200B;现在可在自定义表单设计器上使用。 当数据存储在外部系统上时，此字段类型允许您从外部API加载选项，并根据自定义表单中的其他字段值筛选。

将表单添加到对象时，从API返回的值将显示在下拉字段中，用户可以选择一个。

>[!NOTE]
>
>新 **外部查找** 字段类型在旧版表单生成器中不可用。

有关更多信息，请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).