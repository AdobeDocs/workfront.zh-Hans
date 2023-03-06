---
title: 使用布局模板自定义详细信息视图
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Workfront管理员，您可以使用布局模板来确定当用户查看任务、问题、文档、项目群或项目组合时选择左侧面板中的“详细信息”部分时显示哪些信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 使用布局模板自定义详细信息视图

<!-- drafted for bulk editing proejcts: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

作为Adobe Workfront管理员，您可以使用布局模板来确定当用户单击“详细信息”图标时会显示哪些信息 ![](assets/project-details-icon.png) 查看任务、问题、文档、项目群或项目组合时，位于左侧面板中。

<!--
or billing record
-->

您还可以更改此信息出现的顺序。 例如，对于用户看到的所有任务，您可以将自定义Forms信息移动到用户看到的所有任务的详细信息视图的顶部。

您对对象的“详细信息”视图所做的更改也会决定用户在以下区域看到的字段的可用性和顺序：

* “新对象”框，如“新任务”和“新问题”

   ![](assets/new-task-dialog.png)

* “编辑对象”屏幕，如“编辑任务”、“编辑问题”和“编辑项目”

   ![](assets/edit-task-screen.png)

<!--drafted for bulk editing proejcts - make this bullet live and in yellow at Preview: 

* <span class="preview">"Edit objects" screens when editing projects in bulk, like Edit Projects</span>

  <span>![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)</span>
  -->

* 摘要 ![](assets/summary-panel-icon.png) 任务和问题列表面板

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >对布局模板所做的更改只会影响分配给登录用户的任务和问题的“摘要”面板中字段的顺序和可用性。

* “转化”框，如“将问题转化为任务”或“将问题转化为项目”框。

   ![将问题转换为任务框](assets/convert-issue-to-task-box.png)

有关组的布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义用户在详细信息视图中看到的内容

1. 开始使用布局模板，如中所述 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击向下箭头 ![](assets/dropdown-arrow-12x12.png) 下 **自定义用户看到的内容**，然后单击 **项目**， **任务**， **问题**， **项目**，或 **Portfolio。**
<!--
, or billing record
-->

1. 在 **详细信息** 部分，执行以下任一操作可自定义用户在详细信息视图中看到的内容：

   * 拖动任意节标题 ![](assets/move-icon---dots.png) 来改变他们的顺序。
   * 启用或禁用下的选项 **概述** 和 **自定义Forms** 来显示或隐藏它们。

      如果隐藏其中一个部分中的所有字段，则会隐藏整个部分。

      所有字段默认处于启用状态。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

   >[!TIP]
   >
   >您可以随时单击保存以保存进度，然后稍后继续修改模板。
