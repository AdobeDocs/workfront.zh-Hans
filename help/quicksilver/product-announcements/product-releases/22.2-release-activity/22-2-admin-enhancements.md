---
title: 22.2管理员增强功能
description: 22.2管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# 22.2管理员增强功能

本页介绍在“预览”环境的22.2版本中对管理员所做的所有增强。 这些增强功能将在生产环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。 有关2.2版本中可用的所有更改的列表，请参阅 [22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 配置自定义表单以处理多个对象类型

现在，您可以配置新的或现有的自定义表单以处理多个对象类型，从而使表单更加广泛地有用。 用户将能够在您为其配置的所有类型的对象上附加并填写表单。

以前，您可以将自定义表单配置为仅用于一种对象类型。

此功能可与之前在Workfront系统中创建的所有自定义表单配合使用。 例如，如果您已经为任务对象类型创建了自定义表单，则您现在可以将表单配置为与其他对象类型（如项目和问题）一起使用。

有关更多信息，请参阅 [开始创建自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) 在文章中 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* 在我们初次预览此功能时，我们暂时禁用了复制多对象自定义表单的功能。 该功能于3月24日启用。 有关复制自定义表单的信息，请参阅 [复制自定义表单以创建新表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* 在计算的自定义字段中，您引用的某些字段可能与为表单配置的对象类型不兼容。 我们的解决方案是一种通配符，它允许计算输出不同的值，具体取决于表单所附加到的对象。 3月24日，我们增加了通配符。 有关如何使用该插件的信息，请参阅 [多对象自定义表单中的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) 在文章中 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* 对于自定义表单中的分节，我们创建了一组通用的查看和编辑权限，这些权限适用于您可以为表单配置的所有对象类型。 在一种情况下，我们发现其中一个权限（“有限编辑”）可能会导致表单出错。 已在3月24日修复此问题。 有关分段的更多信息，请参阅 [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>


## Blueprint目录可供所有用户使用，并且管理员可以允许请求

所有Adobe Workfront用户现在都可以浏览可用蓝图目录。 有关更多信息，请参阅 [浏览蓝图目录并请求安装蓝图](../../../administration-and-setup/blueprints/browse-catalog.md).

此外，系统管理员还允许用户请求安装Blueprint。 为请求分配一个请求队列以存储请求，使用户能够从Blueprint目录中发出请求。 有关更多信息，请参阅 [配置对Blueprint的访问权限](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## 将图像添加到自定义表单

在您创建或编辑的自定义表单中，您现在可以添加图像，并包含一个信息性或指导性工具提示，当用户将鼠标悬停在该工具提示上时，可以阅读该工具提示。

例如，这可能有助于显示新产品的品牌策略，或提供填写表单时需要的可视信息。

以前，自定义表单完全基于文本。

>[!NOTE]
>
>在新的Adobe Workfront体验区域（尚未现代化）中，例如批量编辑项目时显示的框，自定义表单图像不会显示。 在我们继续更新这些区域时，它们将显示。

有关更多信息，请参阅 [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 新的默认访问级别配置

为了更好地满足创建新访问级别的大多数管理员的需求，我们更改了下面列出的“优化设置”选项的默认配置。 在您单击齿轮图标时，将显示这些图标 ![](assets/gear-icon-in-access-levels.png) 按钮。

所有这些更改都会禁用以前默认启用的选项。 如果这不符合您组织的需求，您可以在设置新访问级别时或以后的任何时间启用它们。

>[!IMPORTANT]
>
>此默认配置更改仅影响您从现在开始创建的访问级别，而不会影响您之前创建的任何访问级别。

* 在具有计划许可证类型的新访问级别中：

   * 现在，对于项目、任务、问题、项目组合、项目群、报告、过滤器、文档和模板，共享全系统已禁用。
   * 对于报表，也会禁用查看内置报表和公开共享报表。
   * 对于文档，公开共享文档也会被禁用。

* 在具有工作许可证类型的新访问级别中：

   * 现在，对于过滤器和文档，共享系统范围内的内容处于禁用状态。
   * 对于文档，公开共享文档也会被禁用。

* 在具有请求或查看许可证类型的新访问级别中：

   * 现在，对于过滤器，共享系统范围的内容处于禁用状态。

## 停用群组

随着内部组织的更改，您可能需要停止在Workfront中使用某些组并创建新组。 为了帮助解决此问题，我们添加了在不丢失组历史数据的情况下停用组的功能。 对于不需要查看的常规用户，会从“组类型提前”字段中清除不活动的组。

您仍然可以查找和配置您管理的非活动组的选项、首选项和对象关联。 取消激活组不会更改与该组所附加到的对象有关的任何内容。

以前，无法停用组。

有关更多信息，请参阅 [停用或重新激活群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Blueprint安装历史增强功能

现在，在安装Blueprint时，将显示一条消息，显示已成功与Blueprint一起安装的特定对象（如角色、团队或组）以及任何未能安装的对象。 您还可以通过单击安装历史记录表中特定安装旁边的查看详细信息，在“Blueprint详细信息”(Blueprint Details)页面上查看已安装对象的列表。

有关更多信息，请参阅 [安装Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## 现在，在生产中安装仅预览蓝图时会显示警告

某些蓝图仅可用于在“预览”环境中安装以进行测试。

如果您在生产环境、沙盒1或沙盒2中访问仅预览内容，则安装按钮不活动，您可能会看到一条警告消息。

有关更多信息，请参阅 [安装Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
