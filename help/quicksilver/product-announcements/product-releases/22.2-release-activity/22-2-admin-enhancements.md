---
title: 22.2管理员增强功能
description: 22.2管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# 22.2管理员增强功能

本页介绍了在22.2版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。 有关22.2版本的所有可用更改列表，请参阅[22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)。

## 配置自定义表单以使用多个对象类型

现在，您可以配置新的或现有的自定义表单以与多个对象类型一起使用，从而使表单具有更广泛的用途。 用户将能够在您为其配置表单的所有类型的对象上附加和填写表单。

以前，您可以将自定义表单配置为仅使用一个对象类型。

此功能适用于之前在Workfront系统中创建的所有自定义表单。 例如，如果您已经拥有为Task对象类型创建的自定义表单，则现在可以将表单配置为同时使用其他对象类型，如“项目”和“问题”。

>[!NOTE]
>
>* 在首次预览发布此功能时，我们暂时禁用了复制多对象自定义表单的功能。 该功能已于3月24日启用。
>* 在计算自定义字段中，您引用的某些字段可能与为表单配置的对象类型不兼容。 我们的解决方案是一个通配符，允许计算根据表单附加到的对象输出不同的值。 我们在3月24日添加了通配符。
>* 对于自定义表单中的分区界限，我们已创建了一组通用的查看和编辑权限，这些权限适用于可为表单配置的所有对象类型。 在一个方案中，我们发现这些权限之一“有限编辑”可能会导致表单上出现错误。 此问题已于3月24日修复。
>

## Blueprint目录可供所有用户使用，管理员可以允许请求

所有Adobe Workfront用户现在都可以浏览可用Blueprint的目录。 有关详细信息，请参阅[浏览Blueprint目录并请求安装Blueprint](../../../administration-and-setup/blueprints/browse-catalog.md)。

此外，系统管理员可以为用户启用访问权限，以请求安装Blueprint。 通过分配请求队列来存储请求，用户可以从Blueprint目录发出请求。 有关详细信息，请参阅[配置对Blueprint的访问权限](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md)。

## 将图像添加到自定义表单

在您创建或编辑的自定义表单中，您现在可以添加图像并包含信息性或说明性工具提示，用户将鼠标悬停在该图像上时可以阅读这些工具提示。

例如，这对于显示新产品的品牌或提供用户在填写表单时所需的视觉信息可能很有帮助。

以前，自定义表单完全基于文本。

>[!NOTE]
>
>在新的Adobe Workfront体验区域（如批量编辑项目时显示的框）中，尚未进行现代化，自定义表单图像无法显示。 它们将在我们继续更新这些区域时显示。


## 新的默认访问级别配置

为了更好地满足大多数创建新访问级别的管理员的需求，我们更改了下面列出的“微调您的设置”选项的默认配置。 当您单击“编辑”按钮上的齿轮图标![访问级别齿轮图标](assets/gear-icon-in-access-levels.png)时，将显示这些图标。

所有这些更改都会禁用以前默认启用的选项。 如果这不符合贵组织的需求，则可以在设置新访问级别时或稍后随时启用它们。

>[!IMPORTANT]
>
>此默认配置更改仅影响您从现在创建的访问级别，而不影响您之前创建的任何访问级别。

* 在具有“计划”许可证类型的新访问级别中：

   * 现在已为项目、任务、问题、项目组合、程序、报告、筛选器、文档和模板禁用共享系统范围。
   * 对于报表，还禁用“查看内置报表”和“公开共享报表” 。
   * 对于文档，也会禁用公开共享文档。

* 在具有“工作”许可证类型的新访问级别中：

   * 现在已为筛选器和文档禁用共享系统范围。
   * 对于文档，也会禁用公开共享文档。

* 在具有“请求”或“审阅”许可证类型的新访问级别中：

   * 已为筛选器禁用共享系统范围。

## 停用组

随着内部组织的变化，您可能需要停止使用Workfront中的某些组并创建新组。 为了帮助解决此问题，我们添加了取消激活组的功能，而不会丢失其历史数据。 对于不需要查看的非活动用户，将从组预输入字段中清除非活动组。

您仍然可以查找和配置您管理的非活动组的选项、首选项和对象关联。 而且，停用组不会更改与该组连接的对象有关的任何内容。

以前，无法停用组。

有关详细信息，请参阅[停用或重新激活组](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

## Blueprint安装历史记录增强

安装Blueprint时，现在会显示一条消息，其中显示已成功与Blueprint一起安装的特定对象（例如角色、团队或组）以及任何无法安装的对象。 您还可以通过单击安装历史记录表中特定安装旁边的查看详细信息，查看“Blueprint详细信息”页面上的已安装对象列表。

有关详细信息，请参阅[安装Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md)。

![Blueprint安装历史记录](assets/blueprints-installation-history-350x95.png)

## 在生产环境中安装仅预览的Blueprint时，现在会显示警告

某些Blueprint仅可用于在“预览”环境中安装以进行测试。

如果您在生产环境、沙盒1或沙盒2中访问仅预览内容，则安装按钮无效，您可能会看到一条警告消息。

有关详细信息，请参阅[安装Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md)。
