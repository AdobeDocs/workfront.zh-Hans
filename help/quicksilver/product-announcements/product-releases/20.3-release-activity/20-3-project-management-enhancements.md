---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3项目管理增强功能
description: 本页介绍了在20.3版本中针对生产环境所做的所有项目管理增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 20.3项目管理增强功能

本页介绍了在20.3版本中针对生产环境所做的所有项目管理增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。

有关20.3版本可用的所有更改列表，请参阅 [20.3发行版概述](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 列表中的自定义字段格式

>[!NOTE]
>
>仅新Adobe Workfront Experience支持此功能。 它适用于Adobe Workfront Classic中的某些列表，但在Adobe Workfront Classic中不受支持。

现在，当系统管理员创建针对格式配置的自定义表单字段时，您可以在您最常使用的字段中设置文本格式：在整个Workfront的列表中。 您可以在列表中单击某个字段并将粗体、斜体和下划线应用于其中的文本，而不是进入“详细信息”区域以设置自定义表单中的文本格式。

请注意，此功能仅在更新的列表中可用。 有关已更新列表的详细信息，请参阅 [开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

有关Workfront管理员如何创建带格式的文本字段的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 更新了多个全局标头的外观

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

项目、Portfolio、项目和模板的全球区域现在有一个更新的标题，可以更好地利用屏幕上的空间。 此更新为您使用的需要关注的信息提供了更多空间。

已删除项目区域中的“模板”链接。 您仍然可以从主菜单访问“模板”区域。

## 新建编辑项目框

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

作为更新新Workfront Experience的外观的一部分，我们重新设计了编辑项目框。 您可以从单个项目访问新的“编辑项目”框，或在从列表编辑单个项目时访问它。

除了更新的外观，编辑项目框中还提供以下改进：

* 一次自定义您的布局模板，并在“详细信息”页面和“编辑对象”框中反映这些自定义设置。
* 现在，各个自定义表单名称在编辑项目框内的左侧面板上可用，您可以从该处快速访问每个表单。
* 从编辑项目屏幕中删除注释功能，以消除更新部分的冗余。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

有关新的“编辑项目”框的信息，请参见 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

## 新增了“摘要”面板，并改进了文档列表

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

文档列表右侧的新摘要面板现在在新的Workfront Experience中提供增强设计。 当您在Workfront Classic中选择文档时，此面板提供了右侧面板中提供的相同操作和信息，包括文档详细信息、更新、自定义Forms、审批和文档版本。

某些操作当前不可用，但将在未来版本中添加。 这些操作包括验证工作流。

有关更多信息，请参阅 [文档摘要概述](../../../documents/managing-documents/summary-for-documents.md).

## 文档详情改进

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

在“文档详细信息”页面中查找以下改进：

* 新版本选项移至左侧面板附近的下拉菜单，可更轻松地访问。
* 打开验证图标已更改为打开验证标签，使其更易于在页面上查看。
* 更大的预览缩略图，使您可以轻松识别文档
* 添加了全局编辑图标，使您能够一次编辑多个字段。

有关更多信息，请参阅 [文档详情概述](../../../documents/managing-documents/document-details-overview.md).

## 对于管理员：在组级别设置项目偏好设置

>[!NOTE]
>
>集群1、2、3和5上的大多数客户暂时无法使用此功能。 为所有客户恢复此功能后，将更新此页面。

为了给组管理员更大的自主性并允许对工作流进行更多的组级别自定义，您现在可以在组级别为您管理的组定义项目偏好设置。 创建项目时，组的首选项将在系统首选项之前生效。

所有项目首选项均可在组级别进行自定义，但时间线计算和自定义季度除外。

有关组项目首选项的详细信息，请参阅 [配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## 管理员的新增功能：创建用户可设置文本格式的自定义表单字段

在自定义表单中，您现在可以创建包含文本格式按钮的字段。 用户在这些字段中键入内容时，可以使用粗体、斜体和下划线突出显示和组织其文本。 15,000个字符的高限制允许使用大量的文本和格式。

有关更多信息，请参阅在新的Workfront Experience中创建自定义表单。

## 管理员的新增功能：为自定义表单字段创建内部名称和面向用户的标签

为在自定义表单字段上添加标签和重新添加标签提供更大的灵活性，您现在可以创建一个 *name* 除面向用户的字段外， *标签* 你一直在使用。 这样，您就可以自由更改用户看到的字段标签，而无需更改系统看到的字段名称。

过去，标签既显示在字段的上方，供用户使用，也供系统用于标识字段。 所以更换标签使现场在任何地方都出现了故障，因为系统无法再识别它。

有关更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

