---
title: 2026年第四季度报表改进
description: 2026年第四季度报表改进
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1dd8ab20d11b2b4471308ac5402b31e20359a04c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 2026年第四季度报表改进

本页介绍了在2026年第四季度发行的“预览”环境中所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第四季度发布周期中此时可用的所有更改列表，请参阅[2026年第四季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

## 列表和报告有本机引用字段可用

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

您现在可以向Workfront中的列表和报告添加本机引用字段。

本机引用字段是自定义字段。 当字段位于附加到对象的自定义表单上时，字段从对象数据中填充。 例如，如果字段引用了描述字段并且它位于附加到项目的自定义表单上，则会拉入项目描述。 （如果没有可用数据，则字段可能显示“不适用”。）

有关创建本机引用字段的信息，包括支持的本机字段列表，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
有关向报表添加字段的信息，请参阅[创建自定义报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 旧版列表和报告中的多选字段值的一致排序

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

现在，您可以在旧版列表和报告上以一致、可预测的顺序看到多选自定义字段的选定选项。 字段顺序由字段在自定义表单中的排列方式决定。

![自定义表单字段顺序与列表或报表中所选值的顺序匹配](assets/new-field-order-multi-select.png)

以前，选定的选项会以您选择它们的顺序显示，或者以不一致的顺序显示，这会使行更难以扫描和比较。

注：如果字段使用文本模式，则新排序不适用。
