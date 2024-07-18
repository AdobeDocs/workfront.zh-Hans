---
title: 22.4管理员增强功能
description: 22.4管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4管理员增强功能

本页介绍了在22.4版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在2022年10月3日这一周提供。

有关22.4版本的所有可用更改列表，请参阅[22.4版本概述](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)。

## 在审批流程中使用解锁状态

>[!NOTE]
>
>此功能在22.3版本发布时间范围内首次引入到“预览”环境中。 它将于2022年9月15日发布到生产环境。

为了让您更好地控制系统中的审批流程和状态，我们让您能够根据已解锁的系统状态创建审批流程。 此外，您现在可以解锁已在审批流程中使用的任何状态。 以前，必须锁定审批流程中使用的系统状态。 这使得它可供所有组使用（无需删除或重新命名），因此组管理员无法简化其组的状态列表以满足其特定需求。

## 主菜单上的Blueprint图标现在通过布局模板进行控制

系统管理员现在可以通过布局模板配置在主菜单上添加或删除Blueprint图标。 这样可以更好地控制谁可以浏览Blueprint目录。

出现以下情况时，主菜单中会显示Blueprint图标：

* 用户未分配布局模板

* 用户的布局模板在“活动项目”列表中具有Blueprint选项

* 用户的布局模板在可用项列表中具有Blueprint选项，图标未出现在主菜单中。

现有布局模板自动包含Blueprint图标，管理员可以从布局模板中删除该图标以限制Blueprint目录的可见性。 在22.4版本之后创建的新布局模板将在“活动项目”列表中包含Blueprint图标。

有关详细信息，请参阅[配置对Blueprint的访问权限](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 问题标头自定义

作为Workfront或组管理员，您现在可以自定义在您使用版面模板时问题标题中显示的字段。

此更新包括以下增强功能：

* 从问题标题中删除或重新排列现有字段。

* 添加新的不可编辑问题概述字段。 您无法添加可编辑的自定义字段或字段。 您还可以显示问题标题上当前的可编辑字段（例如，状态或完成百分比）。

* 问题标题最多可包含五个字段。

* 您现在可以将“解决者”字段添加到问题标题。 当解析对象与问题相关联时，“解析者”字段将更改为“解析问题”、“解析任务”或“解析项目”，具体取决于与问题关联的对象类型。

在此版本之前，只能自定义项目和任务标题。



有关详细信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 任务标题自定义

作为Workfront或组管理员，您现在可以自定义在您使用布局模板时任务标题中显示的字段。

此更新包括以下增强功能：

* 从任务标题中删除或重新排列现有字段。

* 添加新的不可编辑任务概述字段。 您无法添加可编辑的自定义字段或字段。 您还可以显示当前位于任务标题上的可编辑字段（例如，“状态”或“完成百分比”）。

* 任务标题最多可包含五个字段。

在此版本之前，只能自定义项目标头。

有关详细信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 展示板上最新功能的早期功能选择加入

我们很高兴能推出新的展示板功能，以便尽早选择加入功能。 此可选工具适用于所有组织。

只有Workfront管理员可以选择启用早期功能。 当管理员选择启用早期功能时，组织中的所有用户都选择启用，并且您的生产Workfront环境中启用了附加功能。

有关详细信息，请参阅[Adobe Workfront展示板的早期功能加入](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 自定义表单字段计算编辑器显示错误信息

>[!NOTE]
>
>此功能在22.3版本发布时间范围内首次引入到“预览”环境中。 它会随22.4版一起发布到生产环境。

现在，编辑自定义字段的计算更加容易，并可在计算中直接指示有用的错误信息。 在自定义表单中创建计算字段时，错误将以粉红色突出显示。 将鼠标悬停在突出显示的部分上时，将显示工具提示以描述问题所在。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412387/){target=_blank}

## 迁移到AdobeUnified Experience

注意：此迁移已推迟到2023年第1季度至第2季度。 届时将通知所有受影响的客户。

如果您的组织已载入到Adobe Admin Console，则您的Workfront实例将迁移到Adobe22.4版的Unified Experience。

AdobeUnified Experience包括：

* 通过Adobe Experience Cloud对所有Adobe应用程序进行单点登录

* 用于在Workfront组织和环境之间切换的“组织切换器”

* 包含Workfront页面、Adobe Experience Cloud首选项和Workfront配置文件的选项导航

有关详细信息，请参阅[AdobeWorkfront的Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412388/){target=_blank}
