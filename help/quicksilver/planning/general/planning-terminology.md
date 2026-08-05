---
title: Workfront规划术语概述
description: 尽管Adobe Workfront Planning是一款Workfront产品，但它附带了专有的概念和术语。 在开始为组织设置Workfront计划之前，请确保您熟悉这些概念。
author: Alina
feature: Workfront Planning
role: User, Admin
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 4%

---

# Workfront Planning术语概述


<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning。 Workfront Planning是独立的产品，或者是Adobe Workfront另外购买的功能。
>
>
>本文包含有关客户同时购买Workfront或Workflow包时Workfront Planning的一般信息。
>
>有关包含Workfront Planning文档的文章的完整列表，请参阅[Adobe Workfront Planning的一般信息和文章索引](/help/quicksilver/planning/planning-information.md)。
>
>有关Workfront Planning作为独立产品的信息，请参阅[Adobe Workfront Planning作为独立产品入门](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。

虽然Workfront Planning是Workfront的一部分，但它附带了专有的概念和术语。 在开始为组织设置Workfront计划之前，请确保您熟悉这些概念。

Workfront Planning的框架是完全可自定义的。 您可以创建所有记录类型、其属性以及与其关联的任何字段，以满足贵组织的确切需求。

您可以创建的Workfront Planning对象数存在限制。 有关详细信息，请参阅[Adobe Workfront Planning对象限制概述](/help/quicksilver/planning/general/limitations-overview.md)。

以下是主要的Workfront Planning对象和概念：

* [工作区](#workspaces)
* [记录类型](#record-types)
* [记录](#records)
* [Workspace模板](#workspace-templates)
* [字段](#fields)
* [连接的记录类型、记录和字段](#connected-record-types-records-and-fields)
* [查找字段](#lookup-fields)
* [层级](#hierarchies)
* [视图](#views)
* [自动化](#automations)
* [请求表单](#request-forms)

## 工作区

工作区表示组织单位的框架。 它们是定义特定组织的运营生命周期的记录类型集合。

![具有记录类型分类的营销工作区打开页面](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

有关详细信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

## 记录类型

记录类型是Workfront Planning中的对象类型。

记录类型填充工作区。

与Workfront中预定义的对象类型不同，在Workfront Planning中，您可以创建自己的对象类型。

例如，在Workfront中，已创建Program、Portfolio、Project、Task或Issue的对象类型。

在Workfront Planning中，您可以创建符合组织工作流程的任何记录类型。 稍后，您可以定义记录类型如何相互关联或表单从属关系。

有关详细信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

## 记录

记录是记录类型的实例。

![在营销活动记录类型列表中突出显示的记录](assets/records-highlighted-in-campaign-record-type-list.png)

将记录类型添加到工作区后，您可以开始在该记录类型的页面上添加该类型的记录。

例如，“Campaign”可以是记录类型，“Summer Campaign for EMEA”是Campaign记录类型的记录。

有关详细信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

## Workspace模板

您可以使用预定义模板创建工作区。 您可以使用模板中的预定义记录类型和字段，也可以添加自己的类型和字段。

![带有模板缩略图的工作区页面](assets/workspaces-page-with-templates-thumbnails.png)

Adobe Workfront Planning包含以下模板：

* Operations Initiative Studio
* Communications Planning工作室
* 基本：营销管理
* 高级：营销管理
* 企业：营销管理
* 销售管理
* 产品管理

系统管理员在使用最佳实践的多空间模板时，还可以安装6个工作区。 多空间模板包含以下模板，这些模板同时生成6个独立但连接的工作区：

* 1.全局分类和分类
* 2.Fréscopa全球营销
* 3.Fréscopa社交营销
* 4.弗雷斯科帕媒体与公关
* 5.弗雷斯科帕全球活动
* 6.Fréscopa执行公司领导层

有关更多信息，请参阅以下文章：

* [工作区模板列表](/help/quicksilver/planning/architecture/workspace-templates.md)。
* [创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

## 字段

字段是您可以添加到记录类型的属性。 字段包含有关记录类型的信息。

![记录字段的下拉列表](assets/drop-down-list-of-record-fields.png)

有关记录字段的注意事项：

* 您为记录类型添加的字段会自动与该类型的所有记录相关联，并可用于捕获有关这些记录的数据。

* 字段在应用于记录类型页的“表”视图中显示为列。 它们也会显示在记录的页面中。

* 字段对于记录类型是唯一的，不会从一种记录类型转移到另一种记录类型。

* 字段可完全自定义，并且只能在Workfront Planning中访问。 您无法从Workfront访问Workfront Planning字段。

有关详细信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

默认情况下，新记录类型与以下预定义字段相关联：

* 名称
* 描述
* 开始日期
* 结束日期
* 状态

您可以创建以下类型的自定义字段：

* 单行文本
* 段落
* 多选
* 单选
* 日期
* 数值
* 百分比
* 货币
* 复选框
* 公式
* 人员
* 创建者
* 创建日期
* 上次修改者
* 上次修改日期
* 批准者
* 批准日期
* 记录 ID

<!--update the screen shot above-->

## 连接的记录类型、记录和字段

您可以在Workfront Planning中的以下实体之间创建连接：

* 两种Workfront Planning记录类型。
* 记录类型和Workfront项目、项目群、项目组合、公司或组对象类型。
* 记录类型和Adobe Experience Manager资源或文件夹。

  您必须拥有Adobe Experience Manager许可证才能将记录类型与Experience Manager对象连接。

  ![使用Workfront AEM选项新建连接选项卡](assets/new-connection-tab-with-workfront-aem-options.png)

* 记录类型和Adobe GenStudio for Performance Marketing品牌。

  您必须拥有Adobe GenStudio for Performance Marketing许可证才能将记录类型与GenStudio Brands连接。

  ![使用Adobe GenStudio Brand选项新建连接选项卡](assets/new-connection-tab-with-genstudio-option.png)

在记录类型或记录和对象类型之间建立连接后，可以将这些类型的单个记录或对象彼此连接。 记录之间的连接显示为已连接的记录字段或连接。

当有多种类型的工作对象相互影响时，连接记录类型会很有用。 例如，您可以与营销活动配合使用，每个营销活动可能适合多个品牌。 要指示这种关系，您可以将营销活动关联到品牌。 此外，每个营销活动的工作可能会在Workfront的多个项目中规划。 要指示这一点，您可以将营销策划关联到相关项目。 在Workfront Planning中，连接记录类型并随后连接单个记录即可实现这种关系。

## 查找字段

建立两个记录类型之间的连接并将单个记录连接在一起后，可以从要连接的记录中引用已连接记录的字段。

例如，如果将Campaign记录类型与Workfront Project对象类型连接，则可以在营销活动记录中显示已连接项目的“预算”字段。

![添加查找字段框](assets/add-lookup-fields-modal.png)

>[!TIP]
>
>* 不能将以下字段类型添加为已连接记录或对象类型中的查找字段：
>
>   * 创建者
>   * 上次修改者
>   * Workfront预输入字段（包括项目所有者或项目发起人等字段）
>

有关连接记录类型、记录和创建链接字段的信息，请参阅以下文章：

* [连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)
* [连接记录](/help/quicksilver/planning/records/connect-records.md)

<!--
not yet:* Fields are reusable across Record Types.
-->

## 层级

在工作区中连接记录类型后，您可以创建层次结构来组织这些连接。 层次结构将记录和对象类型组织为父子关系，最多可包含四种对象类型。

![工作区设置区域中的层次结构](assets/hierarchies-in-workspace-settings-area.png)

如果两个记录类型之间的连接尚不存在，则可以在设置层次结构时创建该连接。 定义后，该层级将在工作区内的相关记录类型之间建立结构化路径。

层级会为其各自的记录生成痕迹导航，这些痕迹导航会显示在它们的标题中。 这样，用户就可以在工作流的任何阶段了解自己在层级中的位置。

有关层次结构和痕迹导航的一般信息，请参阅[层次结构和痕迹导航概述](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 视图

记录以不同类型的视图显示在各自的记录类型页面中。

![记录类型列表中的查看类型下拉列表](assets/view-types-drop-down-from-record-type-list.png)

视图包含特定视图类型的个性化设置，如字段列表（列）、记录列表（行）、其顺序（排序）、应用或适用的过滤器和分组。

以下是可应用于记录类型页面的视图类型：

* **表视图**：以表格式显示记录及其字段，包括连接和查找字段。 表的行是单独的记录，列是记录字段。 表格视图是默认视图。

  ![表视图示例](assets/table-view-example.png)

* **时间线视图**：在时间线中显示至少有两个日期类型字段的记录。 您最多可以在时间轴视图中显示5个连接的记录类型及其记录。

  ![在时间轴视图中应用分组](assets/grouping-applied-in-timeline-view.png)

* **日历视图**：以日历格式显示至少有两个日期类型字段的记录。
  ![日历视图示例](assets/calendar-view-example.png)

<!--
add List view here when it's possible to display Planning RTs in it??
-->

其他视图：

* **列表视图**：您可以在Workfront Planning的以下区域列表视图中显示对象：

  * 项目连接的页面。
  * 请求表单列表

  在列表视图中![连接的项目页面](assets/list-view-projects-connected-page.png)

有关详细信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

## 自动化

您可以在Adobe Workfront Planning中配置自动化，在激活时，在从Planning记录触发时，在Workfront Planning中创建记录。 创建的记录会自动连接到从中触发自动化的记录。

您可以在Workfront Planning的记录类型页面中配置和激活自动化。

例如，您可以创建一个接受Workfront Planning营销活动的自动化，并创建一个要与该营销活动关联的品牌。

有关如何使用现有自动化创建对象的信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

## 请求表单

您可以创建请求表单，并将其与Adobe Workfront Planning中的记录类型相关联。 然后，您可以与他人共享该表单，他们也可以提交创建该类型记录的请求。

有关详细信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。