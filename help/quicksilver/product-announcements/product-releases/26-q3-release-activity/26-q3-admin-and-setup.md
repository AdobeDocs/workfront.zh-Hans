---
title: 2026年第三季度管理员增强功能
description: 2026年第三季度管理员增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a88a468901cc7a28139315ab820fc612f1c31736
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 2026年第三季度管理员增强功能

本页介绍了管理员在2026年第三季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 富文本使用格式字段类型替换文本

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

自定义表单中的新&#x200B;**富文本**&#x200B;字段类型是一个强大的文本编辑器，除了粗体、斜体、下划线、项目符号、编号、超链接和块引号等传统选项外，还具有格式选项，如上标和下标、标题和表格。 字符限制仍为15,000。

富文本字段类型正在将文本替换为格式字段类型。 您可以通过单击右侧字段选项中的按钮，快速将带格式字段的现有文本转换为富文本。 转换时，历史数据将保留在字段中，并在报表中以相同的方式使用。

>[!IMPORTANT]
>
>外部集成（如Workfront Fusion场景或基于API的自动化）可能会引用旧版字段结构，并且需要在转换后进行更新。 在将字段转换为富文本之前，您应该验证任何集成。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 自定义表单中支持的本机财务字段

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

您现在可以在自定义表单中包含Workfront本机金融字段。 以前，不支持财务字段。

可引用的可用财务字段取决于表单类型。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)。

## 可以在系统范围内共享自定义表单并有权附加

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

自定义表单中新增了“系统中的每个人都可以查看和附加”共享选项。 选择此选项后，系统范围内的所有用户都可以将表单附加到其他对象。

在系统范围内共享可消除在添加新组时跨组或代理手动共享表单和更新权限的需要。

有关详细信息，请参阅[共享自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。

## 新系统偏好设置可强制批量编辑中的必填字段

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

目前，批量编辑对象时，仅在用户修改必填字段时强制执行该字段。 如果未修改字段，则会将其视为可选字段，且不会验证该字段。

新的系统首选项现在允许您强制批量编辑中的必填字段。 要不允许保存批量编辑的对象，除非所有必填字段都有值，请在“设置”>“系统”>“首选项”页面上选择选项&#x200B;**“始终强制批量编辑必填字段**”。

