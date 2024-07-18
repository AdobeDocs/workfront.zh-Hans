---
title: 22.3管理员增强功能
description: 22.3管理员增强功能
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 22.3管理员增强功能

本页介绍了在22.3版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能在2022年7月11日这一周提供。 有关22.3版本的所有可用更改列表，请参阅[22.3版本概述](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。

## 将Adobe Workfront与JumpSeat集成

您现在可以将JumpSeat与Workfront集成，为用户创建自定义的产品内指南。 您必须拥有Adobe Workfront企业许可证和有效的JumpSeat订阅才能启用集成。

有关详细信息，请参阅[配置JumpSeat集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)。

## 已将验证默认设置移动到Workfront

您现在可以在Workfront设置区域中编辑以下验证设置：

* 校对默认设置

* 验证决策设置

有关详细信息，请参阅[配置默认校对设置](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)。

## 在审批流程中使用解锁状态

**注意：**&#x200B;已从22.3生产版本中删除。 此功能计划于2022年9月15日发布到生产环境。

为了让您更好地控制系统中的审批流程和状态，我们让您能够根据已解锁的系统状态创建审批流程。 此外，您现在可以解锁已在审批流程中使用的任何状态。

以前，必须锁定审批流程中使用的系统状态。 这使得它可供所有组使用（无需删除或重新命名），因此组管理员无法简化其组的状态列表以满足其特定需求。

有关更多信息，请参阅以下文章：

* [创建工作项的审批流程](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [创建或编辑状态](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [锁定和未锁定的系统级别状态](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 将PDF文件添加到自定义表单

我们将继续帮助您通过可添加的新资产小组件（如图像和视频）使自定义表单更可视化、信息化。 现在，您可以将指向PDF文件的链接添加到自定义表单。 将表单附加到对象后，使用该对象的用户可以从表单中查看该PDF并与之交互。

有关详细信息，请参阅[在自定义表单中添加或编辑图像或其他资源小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

## 自定义表单字段计算编辑器显示错误信息

>[!NOTE]
>
>此功能暂时不可用。 当该功能可用时，将更新此页面。

现在，编辑自定义字段的计算更加容易，并可在计算中直接指示有用的错误信息。 在自定义表单中创建计算字段时，错误将以粉红色突出显示。 将鼠标悬停在突出显示的部分上时，将显示工具提示以描述问题所在。

有关详细信息，请参阅[将计算的数据添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

## 项目标题自定义

作为Workfront或组管理员，您现在可以自定义在您使用布局模板时项目标题中显示的字段。

此更新包括以下增强功能：

* 从项目标题中删除现有字段。

* 添加新的不可编辑项目概述字段。 您无法添加可编辑的自定义字段或字段。 当前位于项目标题上的可编辑字段可以保留在标题上。

* 对象标题最多可包含五个字段。


在此版本之前，无法自定义对象标题中的字段。

有关详细信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

## 控制创建空白项目

作为系统或组管理员，您现在可以控制用户是否可以在不使用模板的情况下创建空白项目。 我们在“设置”的“项目首选项”区域引入了一个新设置，允许您在下列区域禁用创建空白项目：

* 通过项目列表中的“新建项目”选项

* 从问题页面将问题转化为项目时


新设置是“允许用户在不使用模板的情况下创建项目”，默认情况下启用该设置。

**注意：**&#x200B;用户仍然可以将任务转换为空白项目。

有关详细信息，请参阅[配置系统范围的项目首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 从组页面取消激活组

最近，我们添加了取消激活和重新激活组的功能。 为了更快、更轻松地执行该操作，我们将其添加到组的页面。 现在，在单击组名以转到其页面后，您可以选择组名旁边的更多菜单![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png)，然后选择停用或重新激活。

以前，只能使用群组“详细信息”页面上的“处于活动状态”复选框来停用或重新激活群组。

有关详细信息，请参阅[停用或重新激活组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

## 将视频添加到自定义表单

现在，您可以通过添加视频为自定义表单提供信息、视觉趣味和创意的新模式。 当表单附加到对象时，使用该对象的用户可以随时播放视频。

以前，您只能将基于文本的字段和图像添加到自定义表单。

有关详细信息，请参阅[在自定义表单中添加或编辑图像或视频资源小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

