---
title: 2026年第三季度管理员增强功能
description: 2026年第三季度管理员增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 7%

---

# 2026年第三季度管理员增强功能

本页介绍了管理员在2026年第三季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 用于统一审阅和批准的更改跟踪

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

Workfront中的“更改历史记录”页面现在可以跨统一的审核和批准工作流捕获活动，为管理员提供完整的审核和文档生命周期事件治理追踪。

现在可跟踪批准、暂存和参与者操作。 这些操作可能包括：

* 在Frame.io查看器中作出批准决定
* 创建或删除审批
* 更新文档，如重命名、移动或删除文档

每个条目都包含标准跟踪字段：日期和时间、操作、用户名（或“系统生成”）和对象名称。 不包括Frame.io查看器注释。

此更改跟踪阶段不包括MCP事件。 这些内容将成为未来版本的一部分。

有关详细信息，请参阅[查看和管理更改历史记录](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)。

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

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
