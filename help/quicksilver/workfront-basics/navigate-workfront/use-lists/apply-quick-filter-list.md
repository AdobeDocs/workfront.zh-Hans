---
navigation-topic: use-lists
title: 将快速过滤器应用到列表
description: 您可以使用对象列表中的快速过滤器来帮助您仅查找对您很重要的项目，以便您可以快速查看、更新或与他人共享这些项目。
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# 将快速过滤器应用到列表

<!--
{{highlighted-preview}}
-->

您可以使用对象列表中的快速过滤器来帮助您仅查找对您很重要的项目，以便您可以快速查看、更新或与他人共享这些项目。

>[!IMPORTANT]
>
>您可以使用快速过滤器找到包含搜索词的项目，无论该项目是在屏幕上实际显示，还是在您滚动到页面底部后会显示。 使用浏览器的搜索功能时，您只能查找屏幕上实际显示的项目。 如果列表有多个页面，则快速过滤器不会找到页面上未显示的项目。

如果要保存快速过滤器，我们建议您为列表构建永久过滤器。\
有关如何在中构建过滤器的信息 [!DNL Adobe Workfront]，请参阅文章 [过滤器概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

快速过滤器当前在以下区域中可用


您可以在所有列表中使用临时快速过滤器，但以下情况除外：

* 的 [!UICONTROL 报表] 面积
* 文档列表和报表
* 几个 [!UICONTROL 设置] 地区
   >[!NOTE]
   >
   >快速过滤器在以下设置区域中可用： [!UICONTROL 群组], [!UICONTROL 团队], [!UICONTROL 公司], [!UICONTROL 计划], [!UICONTROL 布局模板]和 [!UICONTROL 自定义Forms].


在将快速过滤器应用到列表时，请考虑以下事项：

* 您可以使用关键字过滤列表视图中显示的任何字段。 这包括自定义字段或复杂字段，如 [!UICONTROL 前置任务], [!UICONTROL 分配], [!UICONTROL 分配] 和 [!UICONTROL 状态], [!UICONTROL 审批者] 和 [!UICONTROL 状态]等。
* 如果列表具有折叠的分组，则在使用快速过滤器时，这些分组会自动展开。 删除快速过滤器后，组将再次折叠。
* 无论应用了哪些快速过滤器或对列表中的对象进行了任何更改，分组都会保留原始列表的聚合信息。
* 快速过滤器是临时的。 更改列表的分组、查看、过滤或排序，会删除快速过滤条件。
* 无法保存快速过滤器。 如果要保存过滤器以便再次使用，请考虑为列表构建永久过滤器。
* 如果列表中有多个分组，并且快速过滤器仅在一个分组中查找项目，则只有该分组会显示找到的项目。 所有其他分组都将隐藏。
* 在任务或子任务列表中，当显示快速筛选结果时，将删除任务层次结构。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 计划*</b></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 许可证*</b></td> 
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>访问级别配置*</b></td> 
   <td> <p>查看对列表所在区域的访问权限</p> <p>例如，要对项目应用快速过滤器，您需要[!UICONTROL视图]访问“项目”。</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。<br>有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>对象权限</b></td> 
   <td> <p>[!UICONTROL视图]</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 将快速过滤器应用于列表

1. 转到支持快速过滤器的列表或报表，然后单击 **[!UICONTROL 快速筛选] 图标** ![](assets/qs-quick-filter-icon.png) 中。

   或

   根据您的操作系统或浏览器以及使用标准QWERTY键盘时的不同，按下列命令集以启动快速过滤器：

   * ALT+F表示 [!DNL Windows] 计算机
   * ALT/Option+F表示 [!DNL Mac] 计算机

      >[!TIP]
      >
      >如果按CTRL+F或CMD+F，快速过滤器旁边会显示工具提示，提醒您这些命令。 命令也显示在快速过滤器搜索框内。

1. 在 **[!UICONTROL 过滤页面]** 框中，输入要过滤的关键词。

   您可以使用当前显示在列表视图中的任何单词。

   >[!NOTE]
   >
   >如果您使用的词语可能显示在列表的其他页面上，则快速过滤器不会找到任何结果。

   当您键入并隐藏所有其他项目时，列表中会动态显示与搜索条件匹配的项目列表。 在所有独立和复杂字段中，搜索中使用的关键词将以黄色突出显示。 复杂字段的一些示例为共享列，或以下任何列： [!UICONTROL 分配], [!UICONTROL 分配] 和 [!UICONTROL 状态], [!UICONTROL 完成百分比], [!UICONTROL 前置任务], [!UICONTROL 批准者和状态], [!UICONTROL 资源管理器], [!UICONTROL 类别], [!UICONTROL 条件], [!UICONTROL 条件更新]等。

1. （可选）要批量编辑快速过滤器找到的项目，请执行以下操作：

   1. 选择列表中的所有或多个项目，然后单击 **[!UICONTROL 编辑]** 以批量编辑项目。
   1. 完成编辑后，单击 **[!UICONTROL 保存更改]**.

1. （可选）要导出快速过滤器找到的项目，请选择列表中的所有或多个项目，然后单击 **[!UICONTROL 导出]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >只有您在快速过滤器搜索中找到的项目才会导出到您选择的文件。 如果在导出列表之前未选择任何项目，则会导出完整的未过滤列表。\
   >有关更多信息，请参阅 [导出列表](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. （可选）要清除过滤的结果，请单击 **[!UICONTROL 快速筛选]** 图标。\
   或\
   刷新页面。
