---
title: 使用布局模板自定义详细信息视图
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Workfront管理员，您可以使用布局模板来确定当用户查看任务、问题、文档、项目群或项目组合时选择左侧面板中的“详细信息”部分时显示的信息。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 使用布局模板自定义详细信息视图

{{preview-fast-release-general}}

作为Adobe Workfront管理员，您可以使用布局模板来确定当用户查看任务、问题、文档、项目或项目组合时单击左侧面板中的“详细信息”图标![详细信息图标](assets/project-details-icon.png)时显示哪些信息。

<!--
or billing record
-->

您还可以更改此信息出现的顺序。 例如，对于用户看到的所有任务，对于用户看到的所有任务，您可以将自定义Forms信息移动到详细信息视图的顶部。

有关创建布局模板的信息，请参阅[创建和管理布局模板](../use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

您对对象的“详细信息”视图所做的更改还决定了用户在以下区域看到的字段的可用性和顺序：


* “创建对象”框，如“创建任务”

  ![新任务对话框](assets/new-task-dialog.png)


* 编辑对象时显示“编辑对象”屏幕，例如“编辑任务”、“编辑问题”和“编辑项目”

  ![编辑任务屏幕](assets/edit-task-screen.png)


* 批量编辑对象时显示“编辑对象”屏幕。 当前支持批量编辑项目。

  ![自定义编辑项目](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* 任务及问题列表的摘要面板![摘要面板](assets/summary-panel-icon.png)

  ![摘要区域](assets/summary-area.png)

  >[!NOTE]
  >
  >对布局模板所做的更改只会影响分配给登录用户的任务和问题在“摘要”面板中字段的顺序和可用性。

* “转化”框，如“将问题转化为任务”或“将问题转化为项目”框。

  ![将问题转换为任务框](assets/convert-issue-to-task-box.png)

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
        <p>要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义用户在详细信息视图中看到的内容

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 单击![自定义用户看到的内容](assets/dropdown-arrow-12x12.png)下的向下箭头&#x200B;**向下箭头**，然后单击&#x200B;**项目**、**任务**、**问题**、**项目**&#x200B;或&#x200B;**Portfolio。**
<!--
, or billing record
-->

1. 在&#x200B;**详细信息**&#x200B;部分中，执行以下任一操作以自定义用户在“详细信息”视图中看到的内容：

   * 拖动任何节标题![移动图标](assets/move-icon---dots.png)以更改其顺序。
   * 启用或禁用各种区域(如&#x200B;**概述**、**财务**&#x200B;和&#x200B;**自定义Forms**)下的选项以显示或隐藏它们。

     如果隐藏其中一个部分中的所有字段，则会隐藏整个部分。

     所有字段默认处于启用状态。 您可以选中或清除某个区域中的&#x200B;**全选**&#x200B;复选框，以显示或隐藏该区域中的所有字段。

   ![布局模板中的详细信息视图](assets/layout-template-details-view.png)

1. 在“预览”环境中：继续自定义布局模板。 <span class="preview">您可以随时单击&#x200B;**应用**&#x200B;以保存进度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自定义，请单击&#x200B;**保存并关闭**。</span>

1. 在生产环境中：继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**保存**。

   >[!TIP]
   >
   >您可以随时单击&#x200B;**保存**&#x200B;以保存进度，然后稍后继续修改模板。
