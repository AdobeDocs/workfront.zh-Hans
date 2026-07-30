---
title: 2026年第四季度管理员增强功能
description: 2026年第四季度管理员增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1dd8ab20d11b2b4471308ac5402b31e20359a04c
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 2026年第四季度管理员增强功能

本页介绍了管理员在2026年第四季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第四季度发布周期中此时可用的所有更改列表，请参阅[2026年第四季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

## 组管理员可以管理业务配置文件

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

组管理员现在可以为其管理的组创建、编辑和删除业务配置文件，而无需系统管理员访问权限。 这使组织在组级别委派业务配置文件管理方面拥有更大的灵活性。

有关详细信息，请参阅[查看和管理企业档案](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md)。

## 布局模板支持增强列表上的视图

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

现在，系统级别通过布局模板支持增强列表视图。 您可以隐藏现有系统视图，将特定视图指定为默认视图，并将自定义视图添加到系统视图列表中。

布局模板中的增强列表示例为&#x200B;**所有请求**&#x200B;和&#x200B;**高级工作**。 增强型列表在视图旁边有一个“新体验”标签。

有关信息，请参阅[使用布局模板自定义筛选器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 批量编辑外部查找字段

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

批量编辑对话框现在允许编辑外部查找字段。 这在以前是不可能的。

在查找字段从属于另一个查找字段的情况下，无法批量编辑具有依赖关系的字段，除非正在编辑的所有对象的第一个字段相同。

例如，国家/地区列表取决于为区域所做的选择。 如果一个项目的区域是亚洲，而另一个项目的区域是欧洲，并且您批量编辑这两个项目，则国家/地区字段将不可用，因为区域不匹配。 如果您编辑这两个项目中的区域为相同区域，则还可以选择要在两个项目中使用的国家/地区。

有关外部查找字段的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields)。

## 自定义表单设计器预览中支持的高级逻辑

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

自定义表单设计器预览模式现在支持高级逻辑选项，包括高级显示逻辑、默认值逻辑、验证逻辑、格式逻辑和可编辑性逻辑。 您可以在表单预览中测试逻辑公式，并根据需要在逻辑生成器中调整它们。 您还可以选择测试对象（项目、任务、问题等） 以预览具有真实上下文数据的表单。

以前，预览模式仅支持基本显示和跳过逻辑选项。

请注意，这些逻辑类型仅适用于Workflow Prime或Ultimate包中的组织：高级显示、默认值、条件格式和可编辑性。

有关详细信息，请参阅[将逻辑规则添加到自定义表单和字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)和[组织和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。

## 用于统一审阅和批准的更改跟踪

>[!NOTE]
>
>预览： 2026年7月30日>生产快速发布： 2026年8月13日>适用于所有人的生产： 2026年10月15日

Workfront中的“更改历史记录”页面现在可以跨统一的审核和批准工作流捕获活动，为管理员提供完整的审核和文档生命周期事件治理追踪。

现在可跟踪批准、暂存和参与者操作。 这些操作可能包括：

* 在Frame.io查看器中作出批准决定
* 创建或删除审批
* 更新文档，如重命名、移动或删除文档

每个条目都包含标准跟踪字段：日期和时间、操作、用户名（或“系统生成”）和对象名称。 捕获了MCP活动，包括哪个LLM（如Claude）进行了更新。 不包括Frame.io查看器注释。

有关详细信息，请参阅[查看和管理更改历史记录](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)。
