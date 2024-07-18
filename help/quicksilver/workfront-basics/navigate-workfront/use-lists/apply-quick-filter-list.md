---
navigation-topic: use-lists
title: 将快速筛选器应用到列表
description: 您可以在对象列表中使用快速过滤器，以帮助您仅查找对您很重要的项目，以便快速查看、更新或与他人共享这些项目。
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 将快速筛选器应用到列表

<!--
{{highlighted-preview}}
-->

您可以在对象列表中使用快速过滤器，以帮助您仅查找对您很重要的项目，以便快速查看、更新或与他人共享这些项目。

>[!IMPORTANT]
>
>您可以使用快速筛选器查找包含搜索词的项目，无论该项目是已实际显示在屏幕上，还是在滚动到页面底部之后显示。 使用浏览器的搜索功能时，您只能查找屏幕上实际显示的项目。 如果您的列表包含多个页面，则快速筛选器不会查找未显示页面上的项目。

如果要保存快速过滤器，我们建议您为列表构建永久过滤器。\
有关如何在[!DNL Adobe Workfront]中生成筛选器的信息，请参阅文章[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

目前，快速过滤器在以下区域可用


您可以在所有列表中使用临时快速过滤器，但以下列表除外：

* [!UICONTROL 报告]区域
* 文档列表和报告
* 多个[!UICONTROL 设置]区域
  >[!NOTE]
  >
  >快速筛选器在以下设置区域可用： [!UICONTROL 组]、[!UICONTROL 团队]、[!UICONTROL 公司]、[!UICONTROL 计划]、[!UICONTROL 布局模板]和[!UICONTROL 自定义Forms]。


将快速过滤器应用于列表时，请考虑以下事项：

* 您可以使用关键字来筛选在列表视图中显示的任意字段。 这包括自定义字段或复杂字段，如[!UICONTROL 前置任务]、[!UICONTROL 工作]、[!UICONTROL 工作]和[!UICONTROL 状态]、[!UICONTROL 审批者]和[!UICONTROL 状态]等。
* 如果您的列表包含折叠的分组，则当您使用快速筛选器时，这些分组会自动展开。 删除快速筛选器时，分组将再次折叠。
* 无论应用了快速过滤器还是对列表中的对象进行了任何更改，分组都会保留原始列表的聚合信息。
* 快速筛选器是临时的。 更改列表的分组、视图、过滤器或排序将删除快速过滤器条件。
* 无法保存快速筛选器。 如果要保存过滤器以再次使用，请考虑为列表构建永久过滤器。
* 如果列表中有多个分组，并且快速筛选器仅在一个分组中查找项目，则只有该分组会与找到的项目一起显示。 所有其他分组都已隐藏。
* 在任务或子任务列表中，当显示快速筛选器的结果时，将删除任务层次结构。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 计划*</b></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 许可证*</b></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>访问级别配置*</b></td> 
   <td> <p>查看列表所在区域的访问权限</p> <p>例如，要将快速过滤器应用于项目，您需要具有项目的[！UICONTROL视图]访问权限。</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。<br>有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>对象权限</b></td> 
   <td> <p>[！UICONTROL视图]</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 将快速过滤器应用于列表

1. 转到支持快速过滤器的列表或报告，然后单击工具栏中的&#x200B;**[!UICONTROL 快速过滤器]图标** ![](assets/qs-quick-filter-icon.png)。

   或

   根据您的操作系统或浏览器以及使用标准QWERTY键盘时，按下以下命令集以启动快速过滤器：

   * [!DNL Windows]台计算机的ALT+F
   * [!DNL Mac]台计算机的ALT/ Option+F

     >[!TIP]
     >
     >如果按CTRL+F或CMD+F，则会在快速筛选器旁边显示工具提示，以提醒您有关这些命令的信息。 这些命令也显示在快速过滤器搜索框内。

1. 在&#x200B;**[!UICONTROL 筛选页面]**&#x200B;框中，输入要作为筛选依据的关键字。

   您可以使用当前显示在列表视图中的任何单词。

   >[!NOTE]
   >
   >如果使用的单词可能显示在列表的其他页面上，则快速过滤器找不到任何结果。

   当您键入并隐藏所有其他项目时，与搜索条件匹配的项目列表会动态地显示在列表中。 您在搜索中使用的关键字在所有独立和复杂字段中均以黄色突出显示。 某些复杂字段的示例为共享列，或以下任意列：[!UICONTROL 分配]、[!UICONTROL 分配]和[!UICONTROL 状态]、[!UICONTROL 完成百分比]、[!UICONTROL 前置任务]、[!UICONTROL 审批者和状态]、[!UICONTROL 资源管理器]、[!UICONTROL 类别]、[!UICONTROL 条件]、[!UICONTROL 条件更新]等。

1. （可选）要批量编辑由快速筛选器找到的项目，请执行以下操作：

   1. 选择列表中的所有项或多项项，然后单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以批量编辑这些项。
   1. 完成编辑后，单击&#x200B;**[!UICONTROL 保存更改]**。

1. （可选）要导出通过快速筛选器找到的项，请选择列表中的所有项或若干项，然后单击&#x200B;**[!UICONTROL 导出]**。

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >仅在快速过滤器搜索中找到的项目导出到所选文件。 如果在导出列表之前未选择任何项目，则会导出完整的未筛选列表。\
   >有关详细信息，请参阅[导出列表](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md)。

1. （可选）要清除筛选的结果，请单击窗口右上角的&#x200B;**[!UICONTROL 快速筛选器]**&#x200B;图标。\
   或\
   刷新页面。
