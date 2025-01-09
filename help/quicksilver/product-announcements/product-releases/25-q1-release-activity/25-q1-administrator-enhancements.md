---
title: 2025年第一季度管理员增强功能
description: 2025年第一季度管理员增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: d2e3379e9390f2b419bb2d78b1999c8c2dd7d0d3
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 2025年第一季度管理员增强功能

本页介绍了在2025年第一季度版本中对“预览”环境所做的所有管理员增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第一季度发布周期中此时可用的所有更改列表，请参阅[ 2025年第一季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)。

## 在环境之间比较对象以进行环境升级

>[!NOTE]
>
>预览版本： 2024年1月6日；适用于所有客户的生产版本：带有25.1版本（2025年1月）

为了更便于确定环境升级包中应包含哪个对象，我们添加了跨环境比较对象的功能。 现在，您可以选择对象类型和环境。 Workfront会生成该类型对象的列表，包括这些对象是否存在于目标环境中，以及该对象在源环境与目标环境之间是否有差异。 然后，可以直接从此列表将对象添加到资源包。

以前，如果用户希望比较环境之间的对象，则必须手动检查这些对象。

有关详细信息，请参阅[比较环境之间的对象](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md)。

## 更多可用于环境升级的对象

>[!NOTE]
>
>预览版本： 2024年1月6日；适用于所有客户的生产版本：带有25.1版本（2025年1月）

为了扩展环境升级功能的功能，我们添加了更多对象。 现在，可以将以下对象添加到环境升级包中：

* 位置
* 费率卡
* 任务

以前，这些对象不可用于环境升级。

有关可用于环境升级对象的详细信息，请参阅环境升级概述一文中的[环境升级支持的对象](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)。

## 在记录小时数时阻止移动任务

>[!NOTE]
>
>预览版本： 2024年12月19日；适用于所有客户的生产版本：适用于25.1版本（2025年1月16日）

由于移动记录小时数的任务或问题有时会导致合规性或审核问题，因此我们在“设置”的“任务和问题首选项”区域中添加了一个首选项，该首选项允许您阻止用户在记录小时数的情况下移动任务和问题。 在此增强功能之前，用户可以将任务和问题移动到其他项目，即使在这些项目上记录了小时数。

有关信息，请参阅[配置系统范围的任务和问题首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 用于单次分配任务的项目或用户计划的首选项

>[!NOTE]
>
>预览版本： 2024年11月21日；用于快速发布的生产：用于24.12版（2024年12月12日）；用于季度发布的生产：用于25.1版（2025年1月16日）

作为系统或组管理员，您现在有了一个新的首选项，当您为任务分配一个用户，并且项目和用户都关联到时间表时，指示Workfront是否应使用项目或用户的时间表计算项目的时间表。 在此增强功能之前，此设置存在于多用户分配中。 该设置现在可用于单用户任务分配。

有关详细信息，请参阅[配置系统范围的项目首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 业务规则现在支持超链接

>[!NOTE]
>
>预览版本： 2024年11月21日；用于快速发布的生产：用于24.12版（2024年12月12日）；用于季度发布的生产：用于25.1版（2025年1月16日）

现在，您可以在业务规则的自定义错误消息中包含超链接，以指导用户如何在规则的限制内修改其操作。 静态URL可以链接到对用户有益的文档或其他页面。

有关信息，请参阅[创建和编辑业务规则](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)。

## 现在可对本机预输入字段进行筛选

>[!NOTE]
>
>预览版本： 2024年11月21日；用于快速发布的生产：用于24.12版（2024年12月12日）；用于季度发布的生产：用于25.1版（2025年1月16日）

当您将本地字段引用添加到自定义表单并且它引用预输入字段(例如Portfolio、公司或所有者)时，筛选器选项现在可用。 该过滤器允许您限制用户在使用该字段时可以选择的对象。 此自定义筛选器的工作方式与自定义预输入字段上的筛选器的工作方式相同，使用文本模式定义筛选器。

有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 已将“移至”图标添加到自定义字段

>[!NOTE]
>
>预览版本： 2024年10月29日；用于快速发布的生产：用于24.11版（2024年11月14日）；用于季度发布的生产：用于25.1版（2025年1月16日）

当自定义表单包含多个具有许多字段的分区时，可能很难通过拖放方式将字段从一个分区移动到另一个分区。 每个字段都添加了“移至”图标，允许您选择字段所在的部分。

有关详细信息，请参阅[组织和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。
