---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3项目管理增强功能
description: 本页介绍了在生产环境的20.3版本中所做的所有项目管理增强。 这些增强功能已于2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 20.3项目管理增强功能

本页介绍了在生产环境的20.3版本中所做的所有项目管理增强。 这些增强功能已于2020年8月10日这一周的生产环境中提供。

有关20.3版本中可用的所有更改的列表，请参阅 [20.3版本概述](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 列表中的自定义字段格式

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中受支持。 它可用于Adobe Workfront Classic中的某些列表，但在Adobe Workfront Classic中不支持它。

现在，当系统管理员创建为格式配置的自定义表单字段时，您可以在最常用这些字段中设置文本格式：在整个Workfront的列表中。 您无需进入“详细信息”区域以在自定义表单中设置文本格式，而是可以单击列表中的某个字段，并在其中对文本应用粗体、斜体和下划线。

请注意，此功能仅在更新的列表中可用。 有关更新列表的更多信息，请参阅 [开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

有关Workfront管理员如何创建带格式的文本字段的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 更新了多个全局标头的外观

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

“项目”、“Portfolio”、“项目群”和“模板”的全局区域现在有一个更新的标题，可以更好地利用屏幕上的空间。 此更新为您处理的需要重点关注的信息提供了更多空间。

“项目”区域中的“模板”链接已被删除。 您仍可以从主菜单访问“模板”区域。

## “新建编辑项目”框

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

在更新新Workfront体验的外观时，我们重新设计了“编辑项目”框。 您可以从单个项目或在从列表中编辑单个项目时，访问新的“编辑项目”框。

除了更新的外观外，“编辑项目”框中还提供了以下改进：

* 只需自定义布局模板一次，即可在“详细信息”页面和“编辑对象”框中反映这些自定义设置。
* 现在，“编辑项目”框的左侧面板上提供了单个自定义表单名称，您可以从此处快速访问每个表单。
* 注释功能已从编辑项目屏幕中删除，以消除更新部分的冗余。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

有关新的“编辑项目”框的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

## 新增了“摘要”面板和文档列表的更新改进

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

文档列表右侧的新“摘要”面板现在提供，并在新的Workfront体验中增强了设计。 当您在Workfront Classic中选择文档(包括文档详细信息、更新、自定义Forms、批准和文档版本)时，此面板会在右侧的面板中提供相同的操作和信息。

某些操作当前不可用，但将在未来版本中添加。 这些操作包括校对工作流。

有关更多信息，请参阅 [文档摘要概述](../../../documents/managing-documents/summary-for-documents.md).

## 文档详细信息改进

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

在“文档详细信息”页面中查找以下改进：

* 新版本选项已移至左侧面板附近的下拉菜单，从而更便于访问。
* 打开校样图标已更改为打开校样标签，更便于在页面上查看。
* 更大的预览缩览图，使您能够轻松识别文档
* 添加了全局编辑图标，允许您一次编辑多个字段。

有关更多信息，请参阅 [文档详细信息概述](../../../documents/managing-documents/document-details-overview.md).

## 对于管理员：在组级别设置项目首选项

>[!NOTE]
>
>群集1、2、3和5上的大多数客户暂时无法使用此功能。 当为所有客户恢复功能时，将更新此页面。

为了向组管理员提供更多自主权，并允许对工作流进行更多组级别自定义，您现在可以在组级别为您管理的组定义项目首选项。 创建项目时，组的首选项将在系统首选项之前生效。

除时间轴计算和自定义季度外，所有项目首选项都可以在组级别自定义。

有关组项目首选项的详细信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## 管理员的新增功能：创建自定义表单字段，用户可在其中设置文本格式

在自定义表单中，您现在可以创建包含文本格式按钮的字段。 用户在这些字段中键入内容时，可以使用粗体、斜体和下划线突出显示和组织其文本。 字符数上限为15,000，允许大量的文本和格式。

有关更多信息，请参阅在新的Workfront体验中创建自定义表单。

## 管理员的新增功能：为自定义表单字段创建内部名称和面向用户的标签

为了在标签设置和重新标记自定义表单字段方面提供更大的灵活性，您现在可以创建内部 *name* 除面向用户的字段外， *标签* 你一直在用。 这样，您就可以自由更改用户看到的字段标签，而无需更改系统看到的字段名称。

过去，标签会显示在用户字段的上方，并由系统用来标识字段。 因此，更改用户的标签会导致字段在任何使用位置都无法正常工作，因为系统无法再识别它。

有关更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

