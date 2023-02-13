---
product-area: templates
navigation-topic: templates-navigation-topic
title: 将模板附加到项目
description: 您可以在项目的初始创建阶段或创建模板后，将模板附加到项目。
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# 将模板附加到项目

您可以在项目的初始创建阶段或创建模板后，将模板附加到项目。

有关使用模板创建项目的更多信息，请参阅 [使用模板创建项目](../../../manage-work/projects/create-projects/create-project-from-template.md).

## 访问要求

您必须具备以下条件才能执行本文中描述的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限 </p> <p>有关项目访问的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予对项目的访问权限</a>.</p> <p>查看对模板的访问权限</p> <p>有关模板权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">共享模板</a>. </p> <p>有关模板访问的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>. </p> <p>查看模板的权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## 将模板附加到现有项目 {#attach-a-template-to-an-existing-project}

您可以从项目页面或项目列表或报表将模板附加到Workfront中的项目。

1. 转到要附加模板的项目，然后单击 **更多** 图标 ![](assets/qs-more-icon-on-an-object.png) 项目名称的权限

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报表，选择一个项目，然后单击 **更多** 图标 ![](assets/qs-more-icon-on-an-object.png) 列表顶部。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. 单击 **附加模板**.

   此时将显示“附加模板”框。

1. 开始键入要附加到的模板的名称 **搜索模板** 字段，然后在显示时单击该字段。

   或

   在 **其他模板** 的上界。

   模板的预览将显示在右侧，其中包含有关模板的以下信息：

   * 持续时间
   * 所有者
   * 顶级任务的数量（包括前三个顶级任务的列表）
   * 任务总数
   * 附加的自定义表单的名称

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. （可选）单击 **收藏夹** 图标 ![](assets/favorites-icon-small.png) 模板名称的左侧，以将其标记为收藏。 这会在“收藏夹”列表中移动模板。

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. （可选）单击 **收藏夹** 图标 ![](assets/favorites-icon-selected.png) 再次将其从“收藏夹”列表中删除。
1. 单击 **自定义和附加**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. 在附加模板之前更新以下部分中的信息(或者，单击 **附加模板** 随时：):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">“任务”部分</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下选定的模板任务将导入项目。 取消选择要排除的对象。 </td> 
      <td>在将模板附加到项目之前，请取消选择要从模板中排除的任何任务。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">选择要作为此模板中任务的前置任务的项目任务。</td> 
      <td> <p>单击字段可显示项目任务列表。 选择要在模板任务开始之前完成的项目任务。 或者，您也可以跳过此步骤，在附加模板后在项目中设置关系。 </p> <p> 选择 <strong>依赖关系类型</strong>, <strong>滞后</strong> 信息，以及您是否希望前任 <strong>强制</strong> 或不。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">选择要作为此模板中任务父项的项目任务。</td> 
      <td> 选择要指定为所有模板任务的父任务的项目任务。 如果您没有进行选择，则所有模板任务都会显示在当前项目任务的末尾。 在附加模板后，您可以跳过此步骤并在项目中移动任务。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">“选项”部分</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下选定项目将转移到项目。 取消选择要排除的对象。</td> 
      <td> <p>取消选中要在将模板附加到项目之前从模板中清除的任何信息旁边的复选框。 此信息不会从模板传输到项目。 有关每个字段的更多信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">将模板附加到项目的概述</a>. </p> <p>重要信息：如果您选中 <strong>队列属性和问题设置</strong> 框中，模板的队列详细信息将覆盖项目的队列详细信息。 在这种情况下，模板的路由规则、队列主题和主题组将添加到项目的路由规则、队列主题和主题组中。 <br>如果将项目设置为请求队列，并且您附加到项目的模板未设置为请求队列，则如果您离开 <strong>队列属性和问题设置</strong> 复选框。 <br>如果取消选择 <strong>队列属性和问题设置</strong> 框中，将保留项目的所有“队列设置”设置，并且不会附加模板中的“队列设置”设置。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">自定义Forms部分</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义Forms</td> 
      <td> <p>将自定义表单附加到模板后，其名称会显示在左侧面板中。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）更新自定义表单中的信息。 此信息会传输到项目。

   >[!TIP]
   >
   >* 当模板上的自定义表单包含空的必填字段时，必须执行此步骤。
   >* 如果模板自定义表单中的字段在项目上已存在并包含信息，则它们会保留项目上已有的信息。 在附加模板期间，您无法编辑模板。


1. 单击 **附加模板。**
1. 单击 **取消附件** 以停止附加模板。

   或

   允许附件完成以将模板添加到项目。

   附加模板后，您可以编辑项目并根据需要调整任何任务、信息或设置。

1. （可选）单击 **项目详细信息**，则 **概述** 查看您在 **项目关系** 的上界。

   >[!TIP]
   >
   >如果向项目附加多个模板，则只有最先附加的模板才会显示在此字段中。 有关信息，请参阅 [将多个模板附加到现有项目并查看模板信息](#attach-multiple-templates-to-an-existing-project-and-view-template-information) 章节。

1. （可选）从附加了模板的项目中删除模板信息。 有关信息，请参阅 [从项目中删除模板信息](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## 将多个模板附加到现有项目并查看模板信息 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

您可以按照部分中描述的步骤，将多个模板（一次一个）附加到同一项目 [将模板附加到现有项目](#attach-a-template-to-an-existing-project) 在本文中。 这会将每个模板中的任务和其他信息添加到项目中。

>[!TIP]
>
>在将多个模板附加到项目时，只有最先附加的模板才会显示在项目详细信息区域中。

要了解将什么模板应用于项目，请执行以下操作：

1. 导航到附加了模板的项目。
1. 单击 **项目详细信息** 中。
1. 在中查找附加到项目的模板的名称 **模板** 字段 **概述** 部分 **项目关系** .

   ![](assets/nwe-template-info-on-project-350x356.png)

 

 
