---
product-area: projects
navigation-topic: manage-projects
title: 编辑项目
description: 您可以根据需要经常在Adobe Workfront中编辑项目。 理想情况下，当项目处于“计划”状态时，您应该编辑项目。
author: Alina
feature: Work Management
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '7705'
ht-degree: 2%

---

# 编辑项目

<span class="preview">此页面上突出显示的信息是指目前尚不普遍可用的功能。 它仅在“预览”环境中可用。</span>

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

您可以根据需要经常在Adobe Workfront中编辑项目。 我们建议您在项目状态变为“当前”(Current)后对其进行最少的编辑，以通过向整个项目团队发送有关更改的通知来避免混淆。 理想情况下，当项目处于“计划”状态时，您应该编辑项目。 有关项目团队的信息，请参阅 [项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 访问要求

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问项目的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予对项目的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <ul> 
     <li> <p>向项目贡献权限，以在项目详细信息区域对其进行编辑 </p> </li> 
     <li> <p>在“编辑项目”框中管理要编辑项目的权限</p> </li> 
    </ul> <p> 有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>.</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑项目的限制

有些限制可能会阻止您编辑项目。

编辑项目时请考虑以下事项：

* 除了记录时间外，您无法编辑处于审批流程中的项目。
* 仅当您的Workfront管理员或组管理员在“项目首选项”区域中启用此功能时，才能将文档或模板附加到状态为“完成”、“无效”或处于“待批准”的项目。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 您只能编辑处于“已停止”或“已完成”状态的项目的以下信息：

   * 修改现有费用。
   * 添加、删除或编辑自定义表单。

## 编辑项目

通过编辑项目，您可以修改项目的信息和设置，以及项目中的任务和问题。

本文中提及的某些设置可能会根据其默认状态，在创建项目的模板中进行相应的状态修改。 有关编辑模板的信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **项目**.
1. （可选）单击 **我正在执行的项目** 或 **我拥有的项目** 在右上角，显示您是项目团队所有者的项目或项目。

   ![](assets/projects-on-my-own-buttons-350x302.png)

1. 单击要编辑的项目名称以打开项目页面。

   >[!NOTE]
   >
   >如果您是组管理员，则可以在“组”区域以及“项目”区域中查看和编辑组的项目。 有关更多信息，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. （可选）要编辑有关项目的有限信息，请单击 **项目详细信息** 中。

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，项目详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   要编辑详细信息部分中的信息，请执行以下操作：

   1. （可选）单击 **全部折叠** 图标来折叠所有区域。
   1. （可选和视情况而定）折叠区域后，单击 **向右箭头** ![](assets/right-pointing-arrow.png) 展开要编辑的区域。
   1. 有关编辑“项目详细信息”选项卡中信息的更多信息，请参阅以下文章：

      * [在项目概述区域中管理信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [在项目财务区管理信息](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
   1. （可选）要附加自定义表单，请在 **添加自定义表单** 字段，然后在列表中显示时将其选中，然后单击 **保存更改**.
   1. （可选）单击 **导出** 图标 ![](assets/export.png) 要将概述和自定义表单信息导出到PDF文件，请单击 **导出**. 从以下选项中进行选择：

      * 全选（仅当至少附加了一个自定义表单时才显示）
      * 概述
      * 一个或多个自定义表单的名称

      PDF文件将下载到您的计算机。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      有关更多信息，请参阅 [导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   有关“项目详细信息”部分中显示的字段的信息，请按如下所述继续编辑“编辑项目”框中的项目。
1. 要编辑有关项目的所有信息，请单击 **更多** 菜单 ![](assets/qs-more-menu.png) 在项目名称旁边，单击 **编辑**.

   或

   从项目列表中，选择一个项目，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 列表顶部。

   的 **编辑项目** 框中。

   >[!IMPORTANT]
   >
   >您必须拥有项目的“管理”权限，才能看到“编辑”选项。

   所有项目字段在“编辑项目”框中均可用，并按左侧面板中列出的区域进行分组。

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，“编辑项目”框左侧面板中的区域或这些区域中列出的任何字段，可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （视情况而定）如果您单击 **更多** 菜单，然后 **编辑**，请考虑在左侧面板中列出的以下任何区域中更新信息：

   * [项目名称](#project-name)
   * [概述](#overview)
   * [自定义表单](#custom-forms)
   * [财务](#finance)
   * [项目设置](#project-settings)
   * [任务设置](#task-settings)
   * [问题设置](#issue-settings)
   * [访问权限](#access)

   >[!NOTE]
   >
   >根据Workfront管理员为项目的“详细信息”区域设置布局模板的方式，“编辑项目”框中的部分和字段在您的环境中可能有所不同。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 项目名称 {#project-name}

1. 按如上所述开始编辑项目。
1. 单击 **项目名称** 中。

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. 更新项目的名称。

   批量编辑项目时，无法编辑项目名称。

### 概述 {#overview}

1. 按如上所述开始编辑项目。
1. 单击 **概述** 中。

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. 更新有关项目的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td> <p>添加有关项目的其他信息。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状态</strong> </td> 
      <td> <p>选择项目的状态。 在完成所有任务和问题之前，不能将项目标记为已完成。 有关项目状态的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">访问系统项目状态列表</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>优先级</strong> </td> 
      <td> <p> <p>这只是一个用于显示项目优先级的可视标记。</p> <p>根据Workfront管理员选择的项目首选项，优先级名称可能会因您而异。 有关编辑优先级的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">创建和自定义优先级</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>指定与此项目相关信息的Web链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成情况类型</strong> </td> 
      <td> <p>在以下条件类型之间进行选择： 
       <ul> 
       <li><strong>手动：</strong> 项目所有者可手动设置项目上的条件。</li> 
       <li><strong>进度状态：</strong> Workfront会根据关键路径上任务的进度状态自动设置条件。 有关了解进度状态的详细信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任务进度状态概述</a>.</li> 
       </ul><p>您的Workfront管理员<span> 或组管理员</span> 选择系统中项目条件计算方式的默认值 <span>或您的组</span>. 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>. </p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成情况</strong> </td> 
      <td> <p> <p>(仅在您选择 <strong>手动</strong> 对于 <strong>条件类型</strong>):选择一个条件以指示项目的进行方式。 </p> <p>有关如何自动或手动设置项目条件的信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">项目条件和条件类型概述</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>时间表模式</strong> </td> 
      <td> <p>指定项目是从开始日期还是从完成日期开始计划。 此选择可确定项目中任务的计划日期。 
       <ul> 
       <li><strong>开始日期</strong>:默认情况下，项目的第一个任务与项目具有相同的计划起始日期。 有关任务计划起始日期的信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任务计划起始日期概览</a>. 项目时间轴从开始日期计算，项目的完成日期由系统根据所有任务的持续时间计算。 </li> 
       <li><strong>完成日期</strong>:项目的最后一个任务与项目具有相同的计划完成日期。 项目时间轴从完成日期计算，项目的开始日期由系统计算，方法是减去项目完成日期中所有任务的持续时间。 </li> 
       </ul><p>您的Workfront管理员<span> 或组管理员</span> 选择系统或组的默认计划模式设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划开始日期和时间</strong> </td> 
      <td> <p> <p>指定选择的日期 <strong>从开始日期开始计划</strong>. <br></p> <p>当您选择 <strong>从完成日期开始的计划</strong>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划完成日期和时间</strong> </td> 
      <td> <p>指定选择的日期 <strong>从完成日期开始的计划</strong>. </p> <p>当您选择 <strong>从开始日期开始计划</strong>.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>项目组合</strong></td> 
      <td>指示项目所属的Portfolio。 您必须先创建Portfolio，然后才能将其显示在下拉列表中。 只有活动项目组合才能与项目关联。 有关创建项目组合的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">创建项目组合 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>项目群</strong></td> 
      <td> <p>如果您为项目选择了Portfolio，请为项目指定项目计划。 某些Portfolio可能没有程序。 必须先创建程序，然后程序才会显示在此下拉列表中。 只能将活动项目与项目关联。 </p> <p>有关创建程序的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">创建项目</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>组</strong></td> 
      <td> <p> <p>指定与项目关联的组的名称。 </p>这是必填字段. 您不能有与组未关联的项目。 </p> <p>您可以通过将鼠标悬停在正确的组上并单击信息图标来确保选择正确的组 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> 默认情况下，除非您指定其他组，否则在创建项目时，以下组之一会自动与项目关联：</p> 
       <ul> 
       <li> <p><span>从“项目”区域创建项目时，项目创建者的“主页组”会与项目关联。</span> </p> <p>从项目组合或项目群的项目部分创建项目时，也是如此。</p> </li> 
       <li> <p>从“设置”区域的组主页创建项目时，该组将与项目关联。</p> </li> 
       </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
       <p><b>注释</b></p>

   <ul>
      <li><p>如果项目或其任务或问题与组级别的自定义状态相关联，则更改项目组可能会导致项目的状态、任务或问题发生更改以匹配新组。</p></li>
      <li><p>如果项目或其任务或问题已与使用组级别自定义状态的组级别审批流程相关联，则更改组可能会在上一个组的审批状态与系统级别现有的审批状态之间产生冲突。</p>
      <p>在更新项目组之前，请考虑删除项目上的组级审批流程或其任务或问题。</p>
      <p>有关创建组级审批流程的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">组级别的审批流程</a>.</p>
      <p>有关创建组级别自定义状态的信息，请参阅 <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">创建或编辑群组状态</a></p></li></ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>公司</strong> </td> 
      <td> <p>指定与项目关联的公司。 必须先创建公司，然后才能将其与项目关联。 只有活跃的公司才能与项目关联。 有关创建公司的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">创建和编辑公司</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>项目所有者</strong> </td> 
      <td> <p>开始键入用户的名称以将其添加到项目中，然后在列表中显示时将其选中。 用户将添加到项目团队，并自动获得项目的“管理”权限。 指定为项目所有者的用户必须是Workfront活动用户。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>项目赞助者</strong> </td> 
      <td> <p>开始键入用户的名称以将其添加到项目中，然后在列表中显示时将其选中。 用户将添加到项目团队，并自动获得项目的“查看”权限。 被指定为项目赞助商的用户必须是Workfront活动用户。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>资源管理器</strong> </td> 
      <td> <p> 开始键入用户名称以将其添加到项目，然后在列表中显示时选择它们。 用户将添加到项目团队，并自动获得项目的“管理”权限，并可以将资源分配给项目中的任务和问题。 即使从“资源管理器”字段中删除了项目的“管理”权限，用户也会对其进行维护。 您可以指定多个资源管理器。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在更新“项目所有者”、“项目赞助商”和“资源管理器”字段时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。

1. （可选）根据要修改的信息，继续编辑以下部分。

   或

   单击&#x200B;**保存**。

### 自定义表单 {#custom-forms}

根据您的访问级别和您对项目的权限，可能会出现以下情况：

* 如果您对项目没有“编辑自定义表单”权限，则无法编辑任何附加的自定义表单上的字段。 您只能查看附加到项目的自定义表单上的字段。
* 如果您对自定义表单中某个部分具有“查看”（而非“编辑”）访问权限，则无法编辑该部分中的字段。
* 如果您无权访问附加到项目的某个自定义表单上的某个部分，则该部分不会显示在“编辑项目”框中。

选择多个项目以批量编辑它们时，会出现以下情况：

* 如果您至少对一个选定项目没有“编辑自定义表单”权限，则无法编辑任何附加的自定义表单上的字段。 您只能查看附加的自定义表单上的字段
* 如果您对自定义表单中某个部分具有“查看”（而非“编辑”）访问权限，则无法编辑该部分中的字段。 您只能查看该部分中的字段。
* 如果您无权访问附加到其中至少一个项目的一个自定义表单上的某个部分，则该部分不会显示在“编辑项目”框中。

有关自定义表单访问的信息，请参阅以下文章：

* [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)

要编辑有关自定义表单的信息，请执行以下操作：


1. 按如上所述开始编辑项目。
1. 单击 **自定义Forms** 中。

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. 单击 **添加自定义表单** 框中，从列表中选择一个表单以将其附加到项目。 默认情况下，前40个表单按字母顺序显示。 如果在列表中未看到表单，请开始键入其名称，然后在该表单显示在列表中时将其选中。

   >[!NOTE]
   >
   >您必须先构建自定义表单，然后才能在此字段中进行选择。 列表中只显示活动的自定义表单。 有关构建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 一个项目最多可以添加10个自定义表单。


1. （视情况而定）如果您将自定义表单附加到项目，请编辑表单上的任何字段。 在保存项目之前，必须指定所有必填字段。
1. （可选）单击 **X图标** 在自定义表单名称右侧以将其删除，然后单击 **删除**.
1. （可选）根据要修改的信息，继续编辑以下部分

   或

   单击&#x200B;**保存**。

### 财务 {#finance}

根据您的访问级别和您对项目的权限，可能会出现以下情况：

* 如果您对项目具有查看财务数据访问权限和查看财务权限，则只能查看财务部分中的字段。 您无法编辑此部分中的字段。
* 如果您对项目具有“编辑”访问权限和“管理财务”权限，则可以更新此部分中的字段。

选择多个项目以批量编辑它们时，会出现以下情况：

* 如果您至少选择一个项目，其中您具有“查看财务”（而不是“管理财务”）权限，则您只能查看此部分中所有选定项目的字段。 不能批量编辑“财务”部分中的字段。
* 如果您至少选择了一个没有财务权限的项目，则此部分根本不会显示。

要编辑“财务”区域中的字段，请执行以下操作：


1. 按如上所述开始编辑项目。
1. 单击 **金融** 中。

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. 更新项目的以下财务信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>货币</strong> </td> 
      <td> <p> <p>如果项目的货币与系统的默认货币不同，请指定项目的货币。 如果项目中已有财务信息，则无法更改项目的货币。 如果系统中只有默认货币，则此字段不可见。 </p> <p>有关货币的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>预算</strong> </td> 
      <td> <p>为项目指定预算。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>绩效指数方法</strong> </td> 
      <td> <p>选择 <b>基于小时</b>或 <b>基于成本</b> 以指示项目的“挣值”量度（如“成本绩效指数”或“估计实际成本”）是否使用小时或成本计算。 </p> <p>有关性能索引方法的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">设置性能索引方法(PIM)</a>. </p> <p>您的Workfront管理员<span> 或组管理员</span> 为系统或组选择默认的性能索引方法设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完工估算</strong> </td> 
      <td> <p> <p>指定Workfront应如何计算完成时的估计(EAC)。 </p>
      从以下选项中进行选择： 
      <ul><li><b>在项目级别计算</b></li>
      <li><b>从任务/子任务汇总</b></li> </ul>
      <p>有关完成时估计的计算方式的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完成时计算估计(EAC)</a>.</p> <p>您的Workfront或组管理员为您的系统或组选择默认的“完成时估计”设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划收益</strong> </td> 
      <td> <p>估计项目的计划效益。 它用在项目和Portfolio优化程序的业务案例中。 有关项目计划效益的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">项目计划效益概述</a>. 在计算项目的净值时，会考虑项目的计划效益。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">在Portfolio优化器中管理项目</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>实际收益</strong> </td> 
      <td> <p>估计项目的实际效益。 这是表示公司或部门在完成此项目后将获得的好处的货币金额。 </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>固定成本</strong> </td> 
      <td> <p>为项目指定固定成本。 这与项目工时产生的人工成本和项目费用金额产生的费用成本不同。 在计算项目的净值时，会考虑项目的固定成本，并且它是预算成本的一部分。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>固定收入</strong> </td> 
      <td> <p>为项目指定固定收入。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）根据要修改的信息，继续编辑以下部分。

   或

   单击&#x200B;**保存**。

### 项目设置 {#project-settings}

1. 按如上所述开始编辑项目。
1. 单击 **项目设置** 中。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 更新以下信息：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>里程碑路径</strong> </td> 
       <td> <p>为项目选择里程碑路径。 列表中仅显示活动的里程碑路径。</p> <p>有关里程碑路径的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">创建里程碑路径</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>完成模式</strong> </td> 
      <td> <p>控制项目如何标记为完成。 从以下选项中进行选择： 
       <ul> 
       <li><p><strong>自动</strong>:完成所有任务和问题后，项目将标记为“完成”。</p><p>只有在任务完成后，项目状态为“当前”时，项目状态才会自动更改为“完成”。 </p></li> 
       <li><strong>手动</strong>:完成所有任务和问题后，您必须手动选择项目的“完成”状态。</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>摘要完成模式</strong></td> 
       <td> <p>控制父任务如何标记为“完成”。 从以下选项中进行选择： 
       <ul> 
       <li><strong>自动</strong>:父任务被标记为“完成”，并且随着子任务的完成和子任务的完成百分比的更新，父任务会自动更新其完成百分比。 </li> 
       <li><strong>手动</strong>:您必须手动更新父任务的完成百分比和状态，而与对子任务所做的更改无关。</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>更新类型</strong></td> 
       <td> <p>控制您对项目时间轴所做的更改何时保存在项目或父任务上。 例如，对项目所做的以下更改会触发对项目时间轴的更新： 
       <ul> 
       <li>更新任务日期</li> 
       <li>更改任务的前置关系</li> 
       <li><p>更改父子关系，添加或删除分配以及更改任务约束或持续时间类型。</p><p>当任务更新时，其父对象（父任务或项目）会在更新类型指示的时间更新。 </p><p>如果在选择“Automatic and On Change”（自动更改和更改时）或“Change Only”（仅更改）更新类型时，父对象在更改后没有立即更新，请刷新页面</p><p>从以下选项中进行选择： </p><p>- <strong>自动和更改</strong> （默认设置）：每当项目或项目所依赖的其他项目中发生更改（取决于更改）时，项目时间轴都会更新。 项目时间轴也会在每晚更新（自动）。</p><p>建议为此字段设置此设置，因为它可确保项目始终处于最新状态。</p><p>当您对触发时间轴重新计算的任务或项目执行操作时，将立即显示所有可用日期，从而允许您继续工作。 在任务超过100个的项目上，需要更长时间重新计算的日期会短暂地显示为问号（在1到5秒之间，或对于大型项目，最长为1分钟）。 这表示重新计算尚未完成，并且日期可能会发生更改。</p><p>- <strong>仅更改</strong>:每当项目或项目所依赖的其他项目中发生更改时，项目时间轴都会更新。 如果项目或时间轴所依赖的其他项目中很少发生更改，您可能需要选择此选项。</p><p>- <strong>仅自动</strong>:项目时间表每天晚上都会更新；进行更改后，时间轴不会立即更新。</p><p>如果项目或时间轴所依赖的其他项目中每天发生许多更改，您可能需要选择此选项。 但请注意，您选择了此设置，因为项目不会在进行更改的同时进行更新。</p><p>- <strong>仅手动</strong>:仅当您选择“重新计算时间轴”选项时，项目时间轴才会更新。 有关手动重新计算项目时间轴的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新计算项目时间表</a>. </p><p>如果您同时对项目进行多次更改，并且希望在所有更改（而不是在每次更改后）之后重新计算时间轴，则可能需要选择此选项。</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>计划</strong> </td> 
       <td> <p>为项目选择计划。 这应该是分配给大多数正在项目中工作的人员的相同计划。 您必须先创建计划，然后才能将其分配给项目或用户。 如果尚未在系统中创建自定义计划，则会选中“默认计划”。</p> <p>有关创建计划的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>用户空闲时间</strong> </td> 
       <td> <p>确定任务的主要任务负责人的休假时间是否调整项目上的任务计划日期。 </p><p>您的Workfront管理员<span> 或组管理员</span> 为系统选择此设置的默认设置 <span>或您的组</span>. 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>. </p><p>从以下选项中进行选择：<br>- <strong>考虑任务持续时间中的用户休息时间</strong>:在选择此选项时，如果任务在任务期间发生关闭，则任务的计划日期将根据任务的主要任务负责人的关闭时间进行调整。 </p><p>例如，如果具有“尽快”约束的任务计划在6月1日开始，并在6月3日完成，并且主要受分配人将6月2日标记为“超时”，则启用此选择后，任务计划日期为6月1日至6月4日。 根据任务约束，存在以下方案： </p> 
       <ul> 
       <li>对于与从起始日期开始计划相关的任务约束（尽早、最早可用时间、开始时间不早于、开始时间不晚于、必须开始），计划起始日期不会更改，但计划完成日期会更改。</li> 
       <li>对于与完成日期（尽可能晚、最新可用时间、完成时间不早于、完成时间不晚于、必须完成）计划相关的任务限制，计划完成日期不会更改，但计划开始日期会更改。</li> 
       <li>对于具有固定日期约束的任务，计划起始日期和完成日期均不会更改。 </li> 
       </ul><p>选择此设置后，任务的持续时间不会更改。 只有计划日期会更改，具体取决于任务约束。 有关任务约束的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>. </p><p>- <strong>忽略任务持续时间中的用户超时</strong>:选择此选项时，项目上任务的计划日期将保持原计划的状态，即使任务的主要任务负责人在任务期间有时间休息也是如此。 </p><p>选择此设置的选项时，请考虑以下事项：</p> 
       <ul> 
       <li><p>新项目的此设置的默认选项与系统级别项目首选项相同。 </p><p>有关系统级别的项目首选项的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>. </p></li> 
       <li>将模板附加到现有项目后，项目中的设置会更新以匹配其中一个模板。 </li> 
       <li><p>Workfront根据任务的“任务约束”值决定要调整的计划任务日期。 根据具体情况，计划起始日期或计划完成日期可能会受到影响，甚至可能会保持不变。 例如，如果任务具有固定日期约束，则当主要任务负责人有时间关闭时，即使在 <strong>考虑任务持续时间中的用户休息时间</strong> 中。 </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>资源均衡模式</strong> </td> 
       <td> <p> <p>从以下选项中进行选择：</p> <p>- <strong>手动</strong>:您必须手动级别资源（这是默认设置）</p> <p>- <strong>自动</strong>:Workfront会对您的资源进行分级。</p> <p>有关资源平整的详细信息，请参阅 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">甘特图中的级别资源 </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>风险</strong> </td> 
       <td> <p> <p>定义项目的风险级别。 风险只是一个指标，表明一个项目的风险有多大。 您可以根据风险级别优先执行项目。</p> <p> <p>考虑从以下风险级别进行选择：</p> <p>- 很低</p> <p>- 低</p> <p>- 中</p> <p>- 高</p> <p>- 很高</p> <p>您在此处指示的风险级别无法自定义。</p> <p>这些风险与在项目生命周期中可能发生的潜在风险无关，您应在项目的“风险”选项卡或“业务案例”中记录这些风险。 有关潜在项目风险的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">编辑和创建风险类型</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>资源池</strong> </td> 
       <td> <p> <p>指定与项目关联的资源池。 资源池是完成项目同时需要的用户集合，并允许在资源计划器中编制项目预算。 有关资源池的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 资源池概述 </a>. </p> <p>批量编辑项目时，此字段中只会显示所有选定项目共有的资源池。 如果选定的项目没有共享的资源池，则此字段将为空。 您在此处指定的资源池将覆盖项目的各个资源池。</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>允许公司级别的记帐费率覆盖项目级别的记帐费率</strong></td> 
       <td>选择此选项可允许公司层开单费率改写历史职务职责费率，除非这些费率标记为已开单。 启用此选项将覆盖历史职务角色费率，除非将其标记为已计费。 <br>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">使用公司层开单费率改写项目层开单费率</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>该项目需要批准时间</strong></td> 
       <td> <p> 选择此选项可要求项目所有者批准在项目上登录的时间。 如果您使用“开单记录”并选择此选项，则只有项目上已批准的小时数才显示为“开单记录”的可计费小时数。 项目的批准时间与批准时间表无关。 </p> <p>有关需要在项目上获得批准的时间的详细信息，请参阅 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">需要时间来批准项目</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>过滤小时类型</strong> 和</span> <strong>小时类型</strong></td> 
       <td> <p> <p>从以下选项中进行选择：</p> 
       <ul> 
       <li> <p>选择 <strong>否</strong> 以在项目中提供所有特定于项目的小时类型。 （这是默认选择）</p> <p>或</p> </li> 
       <li>选择 <strong>是</strong> 要在项目上仅提供项目特定小时类型的子集，请选择要提供的小时类型。 （按住Shift键可选择多个小时类型。）</li> 
       <p>如果选择此选项，则在记录项目上的小时数（或记录项目中的任务和问题）时，只能选择您选择的小时类型。 必须至少选择一小时类型；如果选择此选项，并且未选择任何小时类型，则项目中将提供所有小时类型。</p> </ul>

   <p>必须在单个用户级别选择相同的小时类型，以便用户在项目中查看这些小时类型选项。 有关在用户级别定义小时类型的详细信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">日志时间</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>提醒通知</strong> </td> 
       <td> <p> <p>选择应与项目关联的提醒通知。 您必须为项目配置提醒通知，以便此字段在编辑项目期间显示。 有关配置提醒通知的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">设置提醒通知</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>批准流程</strong></td> 
       <td> <p>选择要与项目关联的审批流程。 您的Workfront管理员必须定义系统级别的审批流程，然后才能将它们与项目关联。 <span>对审批流程具有管理访问权限的用户也可以创建特定于组的审批流程。</span> 有关创建审批流程的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>.</p> <p>添加审批流程时，请考虑以下事项： </p> 
       <ul> 
       <li>列表中仅显示活动的批准流程。 </li> 
       <li> <p>系统范围和特定于组的审批流程将显示在列表中。 与项目组以外的组关联的批准流程不会显示在列表中。</p> <p>如果与项目关联的组发生更改，则特定于组的审批流程将变成一次性审批流程。 有关项目组更改或审批流程更改如何影响审批设置的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>批量编辑项目时，会出现以下情况：</p> 
       <ul> 
       <li> <p>从同一组中选择项目时，系统级别和组级别的审批流程都会显示在此字段中。</p> </li> 
       <li> <p>从不同的组中选择项目时，此字段中只显示系统级别的审批流程。</p> </li> 
       <li> <p>如果任何项目附加了一次性使用的审批流程，则将由您选择的系统级别或组级别审批流程来替代。 </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. （可选）根据要修改的信息，继续编辑以下部分。

   或

   单击&#x200B;**保存**。

### 任务设置 {#task-settings}

您可以定义默认值，在将所有新任务添加到项目时，这些默认值将与它们关联。

有关这些设置如何影响创建新任务的信息，请参阅部分 [向项目添加任务时，任务默认值](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) 在文章中 [创建任务概述](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. 按如上所述开始编辑项目。
1. 单击 **任务设置** 中。

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. 在 **任务默认审批流程** 框中，选择要在将所有新任务添加到项目时与其关联的任务审批流程。

   您的Workfront管理员（或对审批流程具有管理权限的用户）必须为任务创建系统级别的审批流程，然后才能将其与项目关联。 列表中仅显示活动的批准流程。 有关创建审批流程的信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). 有关项目组更改或审批流程更改如何影响审批设置的信息，请参阅 [组和审批流程更改如何影响分配的审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   批量编辑项目时，会出现以下情况：

   * 当您从同一组中选择多个项目时，此字段中将显示系统级别和特定于组的任务审批流程。
   * 当您从不同的组中选择多个项目时，此字段中仅显示系统级任务审批流程。

1. 在 **任务默认自定义Forms** 框中，选择要在将自定义表单添加到项目时与所有新任务关联的自定义表单。 您必须先构建自定义表单，然后才能在此字段中进行选择。 列表中仅显示活动的自定义表单。 有关构建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 一个任务最多可以关联10个自定义表单。
1. （可选）选择 **使用工作量自动计算任务计划小时数** 如果要使用“工作”(Work Effort)而不是“计划时间”(Planed Hours)来启用管理任务工作。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. （视情况而定和可选）如果您选择使用工作自动计算任务计划小时数，请单击每个工作级别的下拉菜单，然后为每个级别选择一个百分比。 以下百分比值为默认值：

   | 大小 | 百分比 |
   |---|---|
   | 小 | 25% |
   | 中 | 50% |
   | 大 | 75% |

   >[!TIP]
   >
   >如果将项目更新类型设置为“自动”并选择此设置，则任务的“计划小时数”会根据任务持续时间和工作量百分比进行更新（如果将其设置为零）。 有关使用工作量计划任务工作量的详细信息，请参阅 [工作概述](../../../manage-work/tasks/task-information/work-effort.md).

1. （可选）根据要修改的信息，继续编辑以下部分。

   或

   单击&#x200B;**保存**。

### 问题设置 {#issue-settings}

1. 按如上所述开始编辑项目。
1. 单击 **问题设置** 中。

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. （可选）取消选择 **允许用户在内联中添加问题** 选项。 默认情况下，此参数处于选中状态。

   取消选择此选项时，用户无法将内联问题添加到项目或“问题”部分的任务中。

   >[!TIP]
   >
   >如果要强制用户填写新问题字段或与新问题关联的自定义表单，请取消选择此选项。 允许用户在内联输入问题，这允许他们在创建问题时绕过新问题字段和自定义表单。 有关为新问题设置字段和自定义表单的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   取消选择此选项时，有权向项目或任务添加问题的用户可以通过以下方式这样做：

   * 单击项目或任务问题部分问题列表顶部的新问题。
   * 将项目配置为请求队列后，他们可以在“请求”区域中输入新请求。

   >[!NOTE]
   >
   >在批量编辑项目时，如果至少有一个项目启用了此设置，则会启用此设置；如果所有选定项目都禁用了此设置，则会禁用此设置。

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. （可选）根据要修改的信息，继续编辑以下部分。

   或

   单击&#x200B;**保存**。

### 访问权限 {#access}

1. 按如上所述开始编辑项目。
1. 单击 **访问** 中。

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. 指定以下内容 **访问** 项目信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>将某人分配到任务时</strong></td> 
      <td><p>从 <strong>查看</strong>, <strong>贡献、</strong> 或 <strong>管理</strong> 对任务的访问权限。 分配给任务的用户将自动授予该任务的访问权限。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>还授予对项目的访问权限</strong></td> 
      <td><p>从 <strong>查看</strong>, <strong>Contribute</strong>或 <strong>管理</strong> 访问项目。 分配给任务的用户也会自动授予对项目的此访问权限。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>将某人分配到问题时</strong></td> 
      <td><p>从 <strong>查看</strong>, <strong>贡献、</strong> 或 <strong>管理</strong> 对问题的访问权限。 分配给问题的用户将自动授予对问题的此访问权限。 有关更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>还授予对项目的访问权限</strong></td> 
      <td><p>从 <strong>查看</strong>, <strong>Contribute</strong>或 <strong>管理</strong> 访问项目。 分配给问题的用户也会自动授予对项目的此访问权限。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>当某人提交请求时：授予他们访问权限</strong></td> 
      <td><p>从 <strong>查看</strong>, <strong>Contribute</strong>或 <strong>管理</strong> 访问请求。 当项目也是请求队列，并且用户向项目提交请求时，将向他们授予对其提交的请求的访问权限。 有关将项目设置为请求队列的信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>来自同一公司的人员将继承所有请求的相同权限</strong></td> 
      <td><p>如果您希望来自同一公司的人员对项目中的所有请求具有相同的访问权限（无论他们是否提交了请求），请选择此字段。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>当某人有权访问此项目时：授予他们访问……</strong></td> 
      <td><p>如果与用户共享了项目，请选择您希望用户在项目中拥有的访问选项。 如果将其指定为 <strong>查看器</strong>, <strong>参与者</strong>或 <strong>经理</strong> 与他们共享项目时。 </p><p>的 <strong>删除</strong> 在 <strong>管理</strong> 权限级别决定用户是否可以删除项目本身。 具有 <strong>管理</strong> 访问项目可以删除项目中的任务和问题，无论是否选择了此选项，如果这些任务和问题已 <strong>管理</strong> 任务和问题的权限。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

## 在项目标题中编辑项目（受限）

您可以在项目标题中编辑有限量的信息。

您的系统或群组管理员可以自定义您在项目标题中看到的字段。

![](assets/project-header-350x18.png)

默认情况下，项目标题中包含以下字段。

* 项目名称
* 项目所有者
* 计划完成日期和时间

   >[!NOTE]
   >
   >仅当项目计划从完成日期开始时，才可编辑此字段。 当从开始日期开始计划项目时，Workfront会根据任务的持续时间计算计划完成日期和时间。

* 完成情况

   >[!NOTE]
   >
   >仅当项目的条件类型为“手动”时，才可编辑此字段。 将“条件类型”设置为“进度状态”时，Workfront会根据任务的进度计算条件。 有关信息，请参阅 [项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* 状态
* 如果您在当前审批流程中设置为审批者，则应做出审批决策

## 批量编辑项目

您可以批量编辑项目，并同时更新所有选定项目的信息。


您正在更改的所有选定项目的信息将覆盖单个项目的现有信息，但“资源管理器”字段除外。

批量编辑项目时添加新的资源管理器会将该管理器添加到所有选定项目。 如果其他资源管理器与选定的项目相关联，则除了通过批量编辑添加的资源管理器之外，它们还会保留在项目中。

批量编辑项目会因您选择在哪个环境中更新项目而有所不同。

### 在生产环境中批量编辑项目

要批量编辑项目，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **项目**.
1. 在列表中选择多个项目。
1. 单击 **编辑**.

   的 **编辑项目** 对话框。

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. 在以下部分中指定有关所有选定项目的信息：

   * **概述**

      有关信息，请参阅 [概述](#overview) 章节。

   * **财务**

      有关信息，请参阅 [金融](#finance) 章节。

   * **项目组合**

      有关信息，请参阅 [概述](#overview) 章节。

   * **设置**

      有关信息，请参阅 [项目设置](#project-settings) 章节。

   * **访问权限**

      有关信息，请参阅 [访问](#access) 章节。

   * **自定义表单**

      有关信息，请继续执行下面的步骤7。

      <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     -->

   * **任务**

      有关信息，请参阅 [任务设置](#task-settings) 章节。

   * **问题**

      有关信息，请参阅   [问题设置](#issue-settings) 章节。

   * **评论**

      有关信息，请继续执行下面的步骤9。

      <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     -->


1. （可选）在“设置”区域中，选择以下任意选项：

   * **重新计算成本和收入**:选择此选项可重新计算选定所有项目的成本和收入。
   * **重新计算时间轴**:选择此选项可重新计算所有选定项目的时间轴。
   * **重新计算记分卡**:选择此选项可重新计算所有选定项目的记分卡值。

   ![recalculate_costs__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. 单击 **自定义Forms** 编辑附加到所有选定项目的自定义表单。

   如果所选项目没有任何常用的自定义表单，则此部分中不会列出任何表单。

   您只能编辑表单上附加到所有选定项目且您有权编辑的字段。

1. （可选）在自定义Forms部分中，选择 **重新计算自定义表达式** 选项，以确保附加到选定项目的自定义Forms中的所有计算量度自定义字段都是最新的。

   >[!IMPORTANT]
   >
   >我们建议在您重新计算自定义表达式时，不要一次选择500个以上的项目。

1. （可选）单击 **注释**，然后选择向每个项目框发布更新，并在可用字段中指定要在项目更新流中显示的评论，并执行以下操作之一：

   * 单击 **人员** 图标 ![](assets/people-icon-updates-classic.png) 以标记将收到您评论通知的用户。
   * 单击 **锁** 图标 ![](assets/lock-icon-open-updates-classic.png) 将您的评论限制为仅供公司内人员使用。

   此注释对具有项目查看权限和有权查看注释的每个人可见。

1. 单击 **保存更改**.

   现在，您所做的所有更改在所有选定项目上均可见。

<div class="preview">

### 在预览环境中以批量方式编辑项目

在“预览”环境中批量编辑项目时，请考虑以下事项：

* 当您为同一字段选择具有不同值的项目时，该字段会在“编辑项目”框中显示一个“多个值”指示器。 复选框、单选按钮和切换字段旁边有一个“多个值”指示器。

   ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* 除了“多个值”指示器之外，如果选定的选项在至少一个选定项目上不同，则具有多个选项的字段将以下列方式之一显示：

   * 复选框字段包含一行，而不是一个复选框，表示已为某些选定项目选中选项，但未为所有选定项目选中该选项。

      ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * 切换类型字段显示灰显，其中间的切换开关位于为某些选定项目（但并非所有选定项目）启用的选项。

   ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * 选择了某些选项但并非全部的单选按钮类型字段，会将所有单选按钮显示为空。

      ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)


* 当您在多选项字段中更新一个选项（例如显示为一组切换或复选框的字段）时，所有其他选项必须在选定项目之间匹配。

   >[!IMPORTANT]
   >
   >例如，您可能有一个复选框字段，其中包含三个复选框（选项1、选项2和选项3），并且对于所有项目，选项1处于未选中状态；对于某些项目，选项2和选项3处于选中状态，对于您选择的其他项目，则处于未选中状态。 如果要选中所有项目的选项1，则还必须使选项2和选项3与所有选定项目匹配，然后才能保存更改，因此您必须选择或取消选择它们，以便它们能够匹配所有选定项目。 如果不更改任何选项，则可以按原样保存字段，并且项目会保留其当前对所有选项的选择。

* 当您选择属于不同组的多个项目时，“状态”字段中显示的状态是系统级别状态，而不是组级别状态。

要在预览环境中编辑项目，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击 **项目**.
1. 在列表中选择多个项目。
1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 列表顶部。
的 **编辑项目** 对话框。

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

根据Workfront管理员或组管理员修改布局模板的方式，“编辑项目”框左侧面板中的区域或这些区域中列出的任何字段，可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 单击 **概述** 以编辑有关选定项目的常规信息。  有关编辑概述区域的更多信息，请参阅部分 [概述](#overview) 在本文中。

   >[!TIP]
   >
   >您编辑的字段显示为浅紫色背景。

1. 单击 **自定义Forms** 要编辑、添加或替换与选定项目关联的自定义表单，请执行以下操作：

   附加到所有选定项目的自定义表单会显示在 **自定义常见表单** 小节 **自定义Forms** 的上界。

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   所有选定项目通用的表单名称将显示在“编辑项目”框的左侧面板中。

1. 开始在中键入自定义表单的名称 **添加自定义表单** 字段。


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   已附加到选定项目的自定义表单显示在 **附加表单** 小节 **添加自定义表单** 字段。

   可与项目关联但未附加到任何选定项目的其他自定义表单会显示在 **Forms添加** 小节 **添加自定义表单** 字段。

1. 单击以在 **添加自定义表单** 或 **Forms添加** 子区域。

   如果自定义表单已附加到某些选定项目，则在添加表单时，表单名称旁会显示一个指示，指示有多少项目已选择表单。

1. （可选）单击 **x** 图标，然后单击 **删除** ，以将其从所有选定项目中删除。

   >[!CAUTION]
   >
   >删除自定义表单会导致表单上所有现有自定义字段信息丢失。 无法恢复。

   有关编辑自定义表单的更多信息，请参阅部分 [自定义Forms](#custom-forms) 在本文中。

1. 单击 **金融** 编辑所有选定项目的财务信息。
有关编辑“财务”区域的更多信息，请参阅 [金融](#finance) 在本文中。
1. 单击 **项目设置** 以编辑所有选定项目的设置。
有关编辑“项目设置”区域的更多信息，请参阅部分 [项目设置](#project-settings) 在本文中。
1. 单击 **任务设置** 编辑所有选定项目的任务设置。
有关编辑“任务设置”区域的详细信息，请参阅部分 [任务设置](#task-settings) 在本文中。
1. 单击 **问题设置** 编辑所有选定项目的问题设置。
有关编辑“问题设置”区域的更多信息，请参阅部分 [问题设置](#issue-settings) 在本文中。
1. 单击 **访问** 以编辑所有选定项目的访问设置。
有关编辑“访问”区域的更多信息，请参阅部分 [访问](#access) 在本文中。
1. （可选）要删除您在“编辑项目”框中添加的任何信息，请将鼠标悬停在已编辑的字段上，然后单击 **x** 放弃图标。

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. （可选）单击 **取消** 在 **编辑项目** 页面，以删除对所有项目所做的所有更改。
1. 单击&#x200B;**保存**。

</div>

