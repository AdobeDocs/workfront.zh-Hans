---
title: 2026年第四季度报表改进
description: 2026年第四季度报表改进
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 2%
---
# 2026年第四季度报表改进

本页介绍了在2026年第四季度发行的“预览”环境中所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第四季度发布周期中此时可用的所有更改列表，请参阅[2026年第四季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

## Google Cloud Platform和Microsoft Azure上现在提供画布功能板

>[!NOTE]
>
>预览：不适用
>生产快速发布： 2026年10月14日
>适用于所有人的生产： 2026年10月15日

Google Cloud Platform (GCP)和Azure上的Workfront实例现在可以选择使用画布功能板打开测试版。 有关详细信息，请参阅[使用画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

## 注册Snowflake Data Connect的Workfront专用列表

>[!NOTE]
>
>预览：不适用
>生产快速发布： 2026年10月14日
>适用于所有人的生产： 2026年10月15日

您现在可以通过注册个人列表，直接与组织的Snowflake帐户共享Workfront Data Connect数据。 此连接方法使用Snowflake的私有列表功能在组织之间安全地共享数据而不公开披露数据，并且可以跨区域和托管平台工作。

当您要将Workfront数据与企业数据仓库中的其他数据联接时，私有列表非常有用。 由于数据位于您自己的Snowflake帐户中，因此您可以将其与您的其余数据一起查询。

有关详细信息，请参阅[注册Workfront Data Connect的私有列表](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md)。

## 报告MCP工具现在可用于画布仪表板

>[!NOTE]
>
>预览：2026年10月1日
>生产快速发布： 2026年10月14日
>适用于所有人的生产： 2026年10月15日

为了更便于使用画布功能板，我们向Workfront MCP添加了工具。 现在，您可以通过聊天构建和管理画布功能板，并且会使用Workfront数据为您创建功能板和构件。 这适用于Claude和Cursor等MCP客户端。

例如，您可以：

* 通过询问创建报告。 用自然语言描述仪表板或图表，而不是手动构建仪表板。
* 就地编辑。 要求重命名小组件、更改筛选器、交换图表类型或调整大小，这些更改将应用于实时仪表板。
* 重复使用您拥有的资源。 复制现有功能板或构件作为起点，而不是从头重建。

### 支持的功能

**仪表板**

* 创建新仪表板
* 列出您的仪表板（您的仪表板、与您共享的仪表板、所有人仪表板或收藏夹），并按标题进行搜索
* 打开或查看功能板的结构
* 更新标题、描述、货币、筛选器和提示
* 复制仪表板（无论是否包含其小组件、提示和过滤器）
* 删除仪表板

**小组件**

* KPI — 单个合计数字（总和、平均值、计数、最小值、最大值等）
* 图表 — 条形图、柱状图、折线图和饼图；支持简单图、多系列图和栈叠图
* 表 — 具有行分组的多列表
* 查看构件的配置，并更新、复制、调整大小或重新定位，或删除构件

**报告选项**

* 使用条件和AND/OR组过滤数据
* 按任何字段分组和聚合
* 从KPI或图表向下钻取到基础记录
* 自定义列标签、数字、日期和货币格式以及条件单元格样式
* 仪表板级别的提示和过滤器

有关详细信息，请参阅[使用画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

## 在画布功能板之间复制或移动构件

>[!NOTE]
>
>预览：2026年10月1日
>生产快速发布： 2026年10月14日
>适用于所有人的生产： 2026年10月15日

您现在可以将构件复制到同一仪表板、您拥有编辑访问权限的其他仪表板或新仪表板。 您还可以将构件移动到您具有编辑访问权限的其他仪表板或新仪表板。

复制构件时，将打开一个对话框，可在其中选择目标仪表板以及复制还是移动构件。 以前，Report Builder会立即打开。

## 在画布功能板中筛选收藏集关系

>[!NOTE]
>
>预览：2026年10月1日
>生产快速发布： 2026年10月14日
>适用于所有人的生产： 2026年10月15日

在画布功能板中构建过滤器时，您现在可以根据收藏集关系进行过滤，收藏集关系是链接到一组相关记录而不是单个记录的字段。 例如，您可以筛选属于项目的任务状态，以显示具有“新建”状态任务的项目列表。

以前，过滤收藏集关系需要文本模式。

有关详细信息，请参阅[画布功能板的报告筛选器引用](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)。

## 在画布中复制仪表板

>[!NOTE]
>
>预览： 2026年9月3日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

您现在可以使用新的&#x200B;**复制仪表板**&#x200B;操作复制画布仪表板。 此操作适用于其访问级别授予对功能板的编辑或创建权限的任何用户，即使他们仅具有对正在复制的特定功能板的查看访问权限。 没有对功能板进行编辑或创建权限的用户看不到此操作。

复制仪表板时，可以重命名仪表板、更新其描述和货币，以及选择要延续到副本中的小组件、仪表板过滤器和仪表板提示。

只有您是指定用户或系统管理员时，才会保留对构件以用户身份运行配置。 共享首选项将不会复制到新仪表板，并且复制完成后会显示一条确认消息，其中包含指向新仪表板的链接。

以前，无法复制功能板；用户必须从头开始重新构建功能板以创建特定于受众的变体。

## Canvas仪表板中的“审批类型”字段

>[!NOTE]
>
>适用于所有人的生产： 2026年8月28日
>[!BADGE 超出计划]{type=Neutral}

审批实体现在包含&#x200B;**审批类型**&#x200B;字段，该字段允许用户区分验证审批、文档版本审批、接收审批和其他审批类型。

## Canvas仪表板中的审批术语更新

>[!NOTE]
>
>适用于所有人的生产： 2026年8月28日
>[!BADGE 超出计划]{type=Neutral}

为了清楚起见，已重命名画布功能板中用于文档和工作的审批的以下字段名称：

| 上一个名称 | 新名称 |
| --- | --- |
| 文档审批 | 审批 |
| 文档审批阶段 | 审批阶段 |
| 文档审批阶段参与者 | 审批阶段参与者 |
| 审批流程 | 工作审批流程 |
| 审批阶段 | 工作审批阶段 |
| 审批者状态 | 工作审批状态 |
| 等待审批 | 等待工作审批 |

此更改不会影响当前报表的运行方式。

## 画布仪表板中的数据透视表报表

>[!NOTE]
>
>预览： 2026年8月27日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

画布仪表板中新的数据透视表类型使用准确、完整的汇总来聚合数据。 您可以直接在功能板上构建计数、总和和平均等量度，然后深入查看任何总计的基础记录。

有关详细信息，请参阅[在画布功能板中生成数据透视表](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md)。

## 强制计划报表的结束日期

>[!NOTE]
>
>预览： 2026年8月13日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

计划报表现在需要结束日期以防止无限期交付。 超过其结束日期的计划将自动停用。

现有计划已更新了结束日期，以提高可靠性并减少不必要的系统使用。 Workfront还提供了可视性和警告，以帮助您在报表计划生命周期接近其结束日期时对其进行管理。

有关详细信息，请参阅[计划自动报告交付](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

## 列表和报告有本机引用字段可用

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

您现在可以向Workfront中的列表和报告添加本机引用字段。

本机引用字段是自定义字段。 当字段位于附加到对象的自定义表单上时，字段从对象数据中填充。 例如，如果字段引用了描述字段并且它位于附加到项目的自定义表单上，则会拉入项目描述。 （如果没有可用数据，则字段可能显示“不适用”。）

有关创建本机引用字段的信息，包括支持的本机字段列表，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
有关向报表添加字段的信息，请参阅[创建自定义报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 旧版列表和报告中的多选字段值的一致排序

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

现在，您可以在旧版列表和报告上以一致、可预测的顺序看到多选自定义字段的选定选项。 字段顺序由字段在自定义表单中的排列方式决定。

![自定义表单字段顺序与列表或报表中所选值的顺序匹配](assets/new-field-order-multi-select.png)

以前，选定的选项会以您选择它们的顺序显示，或者以不一致的顺序显示，这会使行更难以扫描和比较。

注：如果字段使用文本模式，则新排序不适用。
