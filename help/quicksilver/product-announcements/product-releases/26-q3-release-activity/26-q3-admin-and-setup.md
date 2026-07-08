---
title: 2026年第三季度管理员增强功能
description: 2026年第三季度管理员增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a9688886f32cd41dd7d53dbf0a918f25fdd04a0b
workflow-type: tm+mt
source-wordcount: '1328'
ht-degree: 4%

---

# 2026年第三季度管理员增强功能

本页介绍了管理员在2026年第三季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## 内部查找字段替换预输入字段类型

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

自定义表单中新的&#x200B;**内部查找**&#x200B;字段类型提供了动态筛选。 它与“预输入”字段类型类似，允许用户通过键入部分名称来搜索和选择现有Workfront对象。 内部查找上的筛选器可以引用表单上其他字段中的值，而使用Typeaheads无法执行此操作。

内部查找支持多选，此字段类型还为大型数据集提供了改进的性能。 内部查找支持以下本机Workfront对象：项目、公司、组、工作角色、Portfolio、项目、团队、模板、用户、任务、问题、文档和位置。

Internal lookup字段类型正在替换Typeahead字段类型。 您可以通过单击右侧字段选项中的按钮，快速将现有的预输入字段转换为内部查找。 转换时，历史数据将保留在字段中，并在报表中以相同的方式使用。

>[!IMPORTANT]
>
>外部集成（如Workfront Fusion场景或基于API的自动化）可能会引用旧版字段结构，并且需要在转换后进行更新。 在将预输入字段转换为内部查找字段之前，您应该验证任何集成。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 本机引用字段支持的默认值逻辑

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日
>
>此功能仅适用于Workflow Prime或Ultimate包中的组织。

在自定义表单中，现在可使用本机引用字段添加默认值逻辑。

本机引用字段上的此逻辑类型仅在用户界面中可用，在Workfront API中不可用。

有关信息，请参阅[将逻辑规则添加到自定义表单和字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)一文中的[将默认值逻辑添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form)。

## 更新了自定义表单中的本机字段筛选

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

本机字段上存在的系统筛选器现在应用于自定义表单中的字段，并且管理员可见。

添加应用了系统过滤器的本机引用字段时，可以将相同的过滤器应用于自定义表单中的字段，并根据需要在文本模式框中修改过滤器。

将您自己的自定义筛选器添加到字段会覆盖字段的系统筛选器。 如果不输入自定义筛选器，则默认应用系统筛选器。

此外，动态筛选现在可用于本机引用字段。 动态筛选器允许您根据另一个字段的值缩小项目列表。

例如，当您在项目字段筛选器中使用`?portfolioID={portfolio}.{ID}`，并且自定义表单上有Portfolio本机字段时，项目字段仅显示选定项目组合中的项目。 如果Portfolio字段留空，则所有项目在项目字段中均可用。

有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 保护字段名称不被意外重命名

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

为了保护集成和数据完整性，我们更新了在自定义表单的字段设置面板中编辑字段名称的方式。

字段设置面板中的字段名称现在默认为只读。 您仍然可以编辑字段名称，但重命名需要明确的确认步骤。 以前名为&#x200B;**名称**&#x200B;的字段也已更新为&#x200B;**API名称**，以更好地反映其技术重要性。 **标签**&#x200B;字段保持可编辑状态。

有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels)。

## 查看Workfront对象的更改历史记录

>[!NOTE]
>
>预览：2026年6月11日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

为了让您更轻松地查看在一个中心列表中发生的更改，我们创建了“更改历史记录列表”。 此列表显示诸如对象、操作和更改源（如用户或Workfront系统）等信息。

以前，审核日志可用，但不包含对象。

有关详细信息，请参阅[查看和管理更改历史记录](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)。

## 用于将旧版存储产品组合转换为Adobe云存储的新系统首选项

>[!NOTE]
>
>预览：2026年6月11日适用于所有人的生产： 2026年6月11日

Workfront管理员现在可以直接从“系统首选项”将旧版存储产品组合转换为Adobe云存储。 要转换项目组合，请在新的选择要转换为企业存储的项目组合中选择项目组合，并保存页面。

当产品组合转换为Adobe云存储时：

* 您就无法再将使用旧版 Workfront 存储的项目移动到这个项目组合中
* 这个项目组合中创建的所有新项目都使用 Adobe 云存储
* Frame.io是使用Adobe云存储的文档的查看器
* 使用旧版Workfront存储的子对象将保留在旧版存储中

以前，将Adobe云存储项目添加到旧版存储产品组合会自动将该产品组合转换为Adobe云存储。

有关详细信息，请参阅[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## 富文本将取代“带格式文本”字段类型

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

自定义表单中的新&#x200B;**富文本**&#x200B;字段类型是一个强大的文本编辑器，除了粗体、斜体、下划线、项目符号、编号、超链接和块引号等传统选项外，还具有格式选项，如上标和下标、标题和表格。 字符限制仍为15,000。

富文本字段类型正在将文本替换为格式字段类型。 您可以通过单击右侧字段选项中的按钮，快速将带格式字段的现有文本转换为富文本。 转换时，历史数据将保留在字段中，并在报表中以相同的方式使用。

>[!IMPORTANT]
>
>外部集成（如Workfront Fusion场景或基于API的自动化）可能会引用旧版字段结构，并且需要在转换后进行更新。 在将字段转换为富文本之前，您应该验证任何集成。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 自定义表单现已支持原生财务字段

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

您现在可以在自定义表单中包含Workfront本机金融字段。 以前，不支持财务字段。

可引用的可用财务字段取决于表单类型。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)。

## 自定义表单可在整个系统范围内共享，并授予附加权限

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

自定义表单中新增了“系统中的每个人都可以查看和附加”共享选项。 选择此选项后，系统范围内的所有用户都可以将表单附加到其他对象。

在系统范围内共享可消除在添加新组时跨组或代理手动共享表单和更新权限的需要。

有关详细信息，请参阅[共享自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。

## 新增系统首选项，可在批量编辑时强制要求填写必填字段

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

目前，批量编辑对象时，仅在用户修改必填字段时强制执行该字段。 如果未修改字段，则会将其视为可选字段，且不会验证该字段。

新的系统首选项现在允许您强制批量编辑中的必填字段。 要不允许保存批量编辑的对象，除非所有必填字段都有值，请在“设置”>“系统”>“首选项”页面上选择选项&#x200B;**“始终强制批量编辑必填字段**”。

有关详细信息，请参阅[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。
