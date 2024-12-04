---
content-type: release-notes
title: Adobe Workfront 25.1版的规划发行活动
description: 这是Adobe Workfront计划产品2025年第一季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 0%

---

# Adobe Workfront Planning 2025年第一季度发布活动

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>本文中的信息介绍Adobe Workfront Planning，它是Adobe Workfront的新产品。
>
>除了Workfront计划之外，您必须购买Workfront计划才能访问和使用Workfront计划功能。
>
>有关访问Workfront Planning的完整要求列表，请参阅[访问概述](/help/quicksilver/planning/access/access-overview.md)。
>有关Workfront规划的概述，请参阅[Adobe Workfront规划概述](/help/quicksilver/planning/general/planning-overview.md)。

本文介绍了在2025年第一季度版本中为Workfront Planning发布的功能。

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

有关2024年8月28日正式发布后为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。


## 将现有Workfront字段导入Workfront Planning记录类型

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

现在，将字段添加到记录类型时，您可以选择导入现有的Workfront自定义或本机字段，并将其与您选择的记录类型相关联。 导入现有字段会在Workfront Planning中创建Workfront字段的副本。 复制的字段与其原始版本无关。

在此增强功能之前，您必须手动创建所有字段并将它们与记录类型相关联。

目前不支持计算字段。

有关信息，请参阅[从Adobe Workfront导入字段](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## 通过导入CSV或Excel文件创建记录类型、记录和字段

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

您现在可以通过导入CSV或Excel文件来导入新记录类型。

将导入以下信息：

* 工作表或文件的名称作为记录类型名称导入。

* 每列的第一行作为新字段导入。 每个导入的工作表中最多可以有500个字段。

* 每行都作为新记录导入。 每张纸最多可以有10,000条记录。

有关详细信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

## 避免在公式中使用循环引用

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

在编辑或创建公式字段（该字段可能会创建对自身或共享字段的循环引用）时，我们引入了警告消息。 不能保存引用自身或引用计算中所引用项的公式字段。

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 将“连接”视图页添加到记录的页，以在表视图中显示连接的记录

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

您可以将页面添加到记录的详细信息区域，以在表格视图中显示连接的记录。 您可以为每个连接的记录添加一个页面。

添加的页面为只读。

有关信息，请参阅[管理记录页布局](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 在请求区域的已提交部分中新增了Workfront和Planning选项卡

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

您现在可以在Workfront请求区域的已提交部分找到Workfront规划请求。 “已提交”部分现在显示以下选项卡：

* Workfront：显示在Workfront中提交的请求。
* 计划：显示使用Workfront Planning请求表单提交的请求。

您必须使用请求表单的链接才能将请求添加到Workfront Planning记录类型。 稍后可以从Workfront的“请求”区域提交Workfront计划请求。

您的组织必须先购买Workfront Planning程序包，然后您才能在“请求”区域使用“计划”选项卡。

有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 请求表单现在支持其他字段类型

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

现在，您可以在Workfront Planning中将以下字段类型添加到记录类型请求表单：

* 人员
* Workfront连接

在此增强功能之前，无法将这些类型的字段添加到Workfront Planning中的请求表单。

有关信息，请参阅在Adobe Workfront Planning中创建和管理申请表单(/help/quicksilver/planning/requests/create-request-form.md)。

## 限制公开共享包含特定字段类型的请求表单

>[!NOTE]
>
>预览版本： 2024年11月27日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

如果请求表单包含以下任何字段类型，则不能再公开共享该表单：

* 公式
* Workfront和AEM Assets连接
* 查找字段
* 人员

有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。


## 按周显示日历视图中的记录

>[!NOTE]
>
>预览版本： 2024年11月26日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

现在，您可以在日历视图中按周显示记录。 在此增强功能之前，您只能按月显示日历视图。

有关信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

## 恢复已删除的记录

>[!NOTE]
>
>预览版本： 2024年11月22日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

删除记录后，这些记录现在会暂时移到“最近删除”的收件箱中30天。 您可以从记录类型页面访问最近删除的框，它仅包含特定类型的记录。

Workspace管理员可以在删除记录后，从垃圾桶中恢复长达30天的记录。 连接的记录及其字段信息也会恢复。

在此增强功能之前，无法恢复已删除的记录。

有关详细信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/records-information.md)。

## 可在记录详细信息区域找到的Adobe人工智能助手

>[!NOTE]
>
>预览版本： 2024年11月21日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

为了让您更轻松地完成工作，我们将Adobe人工智能助手添加到记录的详细信息预览或记录页面。 您可以在记录页面内部使用AI助手来更新有关记录的信息。

有关信息，请参阅[Adobe Workfront Planning AI助手概述](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)。

## 向记录页面添加缩略图和封面图像时的新体验

>[!NOTE]
>
>预览版本： 2024年11月20日；用于快速发布的生产：用于24.12版（2024年12月）；用于季度发布的生产：用于25.1版（2025年1月）

当您打开记录的预览或页面并且记录没有缩略图或封面图像时，您必须将鼠标悬停在标题中记录名称上方的区域上，才能查看将封面和缩略图图像添加到记录的选项。 在此增强功能之前，在记录名称上方显示的缩略图和封面的占位符图像为空。

有关更多信息，请参阅以下文章：

* [将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [将缩略图图像添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## 表格视图中百分比类型字段的新显示类型

>[!NOTE]
>
>预览版本： 2024年11月7日；用于快速发布的生产版本：用于24.12版本（2024年12月）；用于季度发布的生产版本：用于25.1版本（2025年1月）

为了使数字在表格视图中更容易阅读，您现在可以从以下选项中进行选择，以更改百分比类型字段在表格视图中的显示方式：

* 数字
* 条形图
* 圆形

此显示类型仅在表格视图中受支持。

在此增强功能之前，您只能将百分比值显示为数字。

有关详细信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 请求表单中现在支持连接字段

>[!NOTE]
>
>预览版本： 2024年10月31日；用于快速发布的生产：用于24.11版（2024年11月14日）；用于季度发布的生产：用于25.1版（2025年1月）

您现在可以将Workfront Planning记录的已连接字段添加到记录类型请求表单中。

您无法在请求表单中为Workfront对象添加连接查找字段或连接字段。

在此增强功能之前，无法将这些类型的字段添加到Workfront Planning中的请求表单。

有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

## 连接已链接到其他记录的记录时出现连接警告

>[!NOTE]
>
>预览版本： 2024年10月31日；用于快速发布的生产：用于24.11版（2024年11月14日）；用于季度发布的生产：用于25.1版（2025年1月）

当尝试连接已在其他位置连接的记录，并且这些记录属于通过“一对多”或“一对一”连接类型连接的记录类型时，您现在会收到一条警告，指出这些记录已连接。 如果确认要继续连接，则将从原始记录中删除所选记录，并将其添加到当前编辑的记录中。

有关连接类型的信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## 带有记录详细信息页面中字段描述的新信息图标

>[!NOTE]
>
>预览版本： 2024年10月30日；用于快速发布的生产：用于24.11版（2024年11月14日）；用于季度发布的生产：用于25.1版（2025年1月）

我们在记录页面中的字段名称的右侧添加了一个信息图标。 当存在描述时，单击信息图标将显示字段的说明。 在此增强功能之前，将鼠标悬停在字段名称上时显示的字段描述。

有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

## 适用于Planning连接的新Workfront字段类型

>[!NOTE]
>
>预览版本： 2024年10月24日；用于快速发布的生产：用于24.11版（2024年11月14日）；用于季度发布的生产：用于25.1版（2025年1月）

为了继续将Workfront对象桥接到Workfront Planning记录，我们在Workfront自定义表单中添加了一个名为Planning连接的新字段类型。 现在，通过在Workfront自定义表单上添加此字段类型，并最终在Workfront对象上添加此字段类型，您可以执行以下操作：

* 在自定义表单中显示连接到Workfront对象的记录。

* 从Workfront对象连接和断开Workfront Planning记录。

您可以将新字段添加到所有对象类型的表单中。 但是，您只能从附加到以下Workfront对象的表单编辑字段中的信息，这些对象可以从Workfront Planning记录类型连接：Portfolio、项目、公司、组。

现在尚无法为Workfront对象批量编辑Planning连接字段。

有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3435633/){target=_blank}
