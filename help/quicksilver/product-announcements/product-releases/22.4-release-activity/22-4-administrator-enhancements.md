---
title: 22.4管理员增强功能
description: 22.4管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4管理员增强功能

本页介绍在“预览”环境的22.4版本中对管理员所做的所有增强。 这些增强功能将于2022年10月3日这一周发布。

有关22.4版本中可用的所有更改的列表，请参阅 [22.4版本概述](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 在批准流程中使用已解锁状态

>[!NOTE]
>
>在22.3版本时间范围内，此功能首次在“预览”环境中引入。 它于2022年9月15日发布至生产。

为了让您更好地控制系统中的审批流程和状态，我们允许您基于已解锁的系统状态创建审批流程。 此外，您现在可以解锁批准流程中已使用的任何状态。 以前，审批流程中使用的系统状态必须被锁定。 这样，组管理员就无法简化组的状态列表以满足其特定需求，而且所有组都可以使用该状态，而且无法删除或重命名该状态。

## 主菜单上的Blueprint图标现在可通过布局模板进行控制

现在，系统管理员可以通过布局模板配置来添加或删除主菜单上的Blueprint图标。 这可以更好地控制谁可以浏览Blueprint目录。

当出现以下情况时，“Blueprints”（蓝图）图标会显示在“Main Menu（主菜单）”中：

* 用户未分配布局模板

* 用户的布局模板在“活动物料”列表中具有“Blueprint”选项

* 用户的布局模板在“可用项目”列表中具有“蓝图”选项，该图标不会显示在主菜单中。

现有的布局模板会自动包含Blueprint图标，管理员可以从布局模板中删除该图标以限制Blueprint目录的可见性。 22.4版本之后创建的新布局模板将在“活动项目”列表中包含“Blueprint”图标。

有关更多信息，请参阅 [配置对Blueprint的访问权限](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 问题标题自定义

作为Workfront或组管理员，您现在可以在使用布局模板时自定义在问题标题中显示的字段。

此更新包括以下增强功能：

* 从问题标题中删除或重新排列现有字段。

* 添加新的不可编辑的问题概述字段。 您无法添加可编辑的自定义字段或字段。 您还可以显示问题标题上当前包含的可编辑字段（例如，“状态”或“完成百分比”）。

* 问题标题最多可包含五个字段。

* 现在，您可以将“解决方式”字段添加到问题标题中。 当解决对象与问题关联时，“解决者”字段会根据与问题关联的对象类型更改为“解决问题”、“解决任务”或“解决项目”。

在此版本之前，只能自定义项目和任务标题。



有关更多信息，请参阅 [使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 任务标题自定义

作为Workfront或组管理员，您现在可以在使用布局模板时自定义任务标题中显示的字段。

此更新包括以下增强功能：

* 从任务标题中删除或重新排列现有字段。

* 添加新的、不可编辑的任务概述字段。 您无法添加可编辑的自定义字段或字段。 您还可以显示当前位于任务标题上的可编辑字段（例如，“状态”或“完成百分比”）。

* 任务标题最多可包含五个字段。

在此版本之前，只能自定义项目标题。

有关更多信息，请参阅 [使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 抢先试用展示板上的最新功能

我们很高兴能够为抢先体验功能选择加入打开新的展示板功能。 此可选工具可供所有组织使用。

只有Workfront管理员才能选择使用早期功能。 当管理员选择早期功能时，组织中的所有用户都将选择加入，并且其他功能将在您的生产Workfront环境中启用。

有关更多信息，请参阅 [抢先试用Adobe Workfront展示板的功能选择加入](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 自定义表单字段计算编辑器显示错误信息

>[!NOTE]
>
>在22.3版本时间范围内，此功能首次在“预览”环境中引入。 它随2.4版本发布到生产环境。

现在，编辑自定义字段的计算更为简单，计算中会直接显示有用的错误信息。 在自定义表单中创建计算字段时，错误将以粉红色突出显示。 将鼠标悬停在突出显示的部分上时，会显示工具提示，以描述问题所在。

有关更多信息，请参阅 [将计算数据添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412387/){target=_blank}

## 迁移到Adobe统一体验

注意：这一迁移已推迟到2023年的Q1-Q2次。 届时，任何受影响的客户都将收到通知。

如果贵组织已载入Adobe Admin Console，则Workfront实例将在22.4版本中迁移到Adobe统一体验。

Adobe统一体验包括：

* 通过Adobe Experience Cloud对所有Adobe应用程序进行单次登录

* 在Workfront组织和环境之间移动的“组织切换器”

* 使用Workfront页面、Adobe Experience Cloud首选项和Workfront配置文件的选项进行导航

有关更多信息，请参阅 [Adobe统一的Workfront体验](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412388/){target=_blank}
