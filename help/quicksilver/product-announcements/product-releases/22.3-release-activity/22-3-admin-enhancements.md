---
title: 22.3管理员增强功能
description: 22.3管理员增强功能
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 22.3管理员增强功能

本页介绍在“预览”环境的22.3版本中对管理员所做的所有增强。 这些增强功能于2022年7月11日这一周发布。 有关22.3版本中可用的所有更改的列表，请参阅 [22.3版本概述](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 将Adobe Workfront与JumpSeat集成

您现在可以将JumpSeat与Workfront集成，以为用户创建自定义的产品内指南。 您必须拥有Adobe Workfront企业许可证和有效的JumpSeat订阅才能启用集成。

有关更多信息，请参阅 [配置JumpSeat集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## 校样默认设置已移至Workfront

您现在可以在Workfront设置区域内编辑以下校样设置：

* 校样默认设置

* 校样决策设置

有关更多信息，请参阅 [配置默认校样设置](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## 在批准流程中使用已解锁状态

**注意：** 已从22.3生产版本中删除。 此功能计划于2022年9月15日发布到生产环境。

为了让您更好地控制系统中的审批流程和状态，我们允许您基于已解锁的系统状态创建审批流程。 此外，您现在可以解锁批准流程中已使用的任何状态。

以前，审批流程中使用的系统状态必须被锁定。 这样，组管理员就无法简化组的状态列表以满足其特定需求，而且所有组都可以使用该状态，而且无法删除或重命名该状态。

有关更多信息，请参阅以下文章：

* [为工作项创建审批流程](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [创建或编辑状态](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [锁定和解锁的系统级别状态](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 将PDF文件添加到自定义表单

我们将继续帮助您使用可添加的新资产小组件（如图像和视频），使自定义表单更加直观和信息丰富。 现在，您可以向自定义表单添加指向PDF文件的链接。 将表单附加到对象后，使用该对象的用户可以从表单内查看该PDF并与其交互。

有关更多信息，请参阅 [在自定义表单中添加或编辑图像或其他资产小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 自定义表单字段计算编辑器显示错误信息

>[!NOTE]
>
>此功能暂时不可用。 当该功能可用时，将更新此页面。

现在，编辑自定义字段的计算更为简单，计算中会直接显示有用的错误信息。 在自定义表单中创建计算字段时，错误将以粉红色突出显示。 将鼠标悬停在突出显示的部分上时，会显示工具提示，以描述问题所在。

有关更多信息，请参阅 [将计算数据添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 项目标题自定义

作为Workfront或组管理员，您现在可以在使用布局模板时自定义项目标题中显示的字段。

此更新包括以下增强功能：

* 从项目标题中删除现有字段。

* 添加新的不可编辑项目概述字段。 您无法添加可编辑的自定义字段或字段。 当前位于项目标题中的可编辑字段可保留在标题中。

* 对象标头最多可包含五个字段。


在此版本之前，无法自定义对象标题中的字段。

有关更多信息，请参阅 [使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## 控制创建空白项目

作为系统或组管理员，您现在可以控制用户是否可以创建空白项目，而无需使用模板。 我们在“设置”的“项目首选项”区域中引入了一个新设置，允许您在以下区域中禁用创建空白项目：

* 从项目列表中的新建项目选项

* 将问题从问题页面转换为项目时


新设置为“允许用户在不使用模板的情况下创建项目”，默认情况下处于启用状态。

**注意：** 用户仍可以将任务转换为空白项目。

有关更多信息，请参阅 [配置系统范围的项目首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 从“群组”页面中停用群组

最近，我们添加了停用和重新激活群组的功能。 为了更快、更轻松地执行该操作，我们已将其添加到群组页面。 现在，在单击某个群组的名称以转到其页面后，您可以选择“更多”菜单 ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) 在群组名称旁边，选择停用或重新激活。

以前，只能使用群组详细信息页面上的活动复选框来停用或重新激活群组。

有关更多信息，请参阅 [停用或重新激活群组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## 将视频添加到自定义表单

现在，您可以通过添加视频为自定义表单提供新的信息、视觉兴趣和创意模式。 将表单附加到对象后，使用该对象的用户可以随时播放视频。

以前，您只能向自定义表单中添加基于文本的字段和图像。

有关更多信息，请参阅 [在自定义表单中添加或编辑图像或视频资产小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

