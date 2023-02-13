---
product-area: projects
navigation-topic: create-projects
title: 创建项目
description: (注意：这是从UI中的Projects全局导航部分链接到的，位于经典中。 请勿更改/删除)
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# 创建项目

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

项目是Adobe Workfront需要做的大量工作。

## 访问要求

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问项目的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予对项目的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在创建项目时，您会自动收到该项目的管理权限 </p> <p> 有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>.</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建项目的方法

您可以使用以下方法之一在Workfront中创建项目：

* 无需使用模板即可从头开始创建项目。 本文介绍了如何从头开始创建项目。

* 复制现有项目。\
   有关复制项目的更多信息，请参阅 [复制项目](../../../manage-work/projects/manage-projects/copy-project.md).

* 使用模板。\
   有关使用模板创建新项目的更多信息，请参阅 [使用模板创建项目](../../../manage-work/projects/create-projects/create-project-from-template.md).

* 从Microsoft项目导入项目。\
   有关从MS项目导入项目的详细信息，请参阅 [从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* 使用启动项导入项目。

   作为Workfront管理员，您可以使用启动项导入项目。

   有关在Workfront中使用启动导入数据的信息，请参阅 [使用“启动”模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

   有关使用启动导入项目的信息，请参阅 [“启动”方案：简单项目和任务导入准备](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* 在Adobe Workfront方案计划器中根据方案发布方案。 方案计划员需要附加许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md). 有关通过发布计划创建项目的信息，请参阅  [通过在方案规划器中发布方案来更新或创建项目](../../../scenario-planner/publish-scenarios-update-projects.md).

## 先决条件

在开始之前，您必须确保

* 您的系统或组管理员在“设置”区域启用了“允许用户在不使用模板的情况下创建项目”首选项。

   有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 新项目默认设置

在创建项目时，Workfront会为其应用一组默认设置。 例如，在创建项目时，状态、组或计划模式是预设。

请考虑以下事项：

* 作为Workfront管理员或组管理员，您可以在配置项目首选项时为新项目配置默认设置。
* Workfront在应用由Workfront管理员设置的设置之前，会应用组的设置（如果存在）。
* 如果您使用模板创建项目，则模板中的设置优先于Workfront或组管理员建立的设置。

>[!NOTE]
>
>我们建议新项目的默认状态为“计划”。 在对新项目进行更改时，这可确保通知不会触发给分配给项目的用户。

有关为新项目设置默认状态和其他默认设置的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).



## 从头开始创建项目

1. 执行下列操作之一：

   * 单击 **主菜单** ![](assets/main-menu-icon.png)，单击 **项目**，然后展开 **新建项目**.
   * 转到项目组合，然后展开 **新建项目**.

      >[!TIP]
      >
      >当您使用组合中的模板创建项目时，新项目的Portfolio字段会更新，以显示您选择从中创建项目的组合。 如果指定了Portfolio，则会覆盖模板上的模板字段。

   * 转到项目，然后展开 **新建项目**.

      >[!TIP]
      >
      >使用项目的模板创建项目时，新项目的“项目”(Program)字段会更新，以显示您选择从中创建项目的项目。 模板的Portfolio字段会更新，以显示您选择从中创建项目的项目组合。 如果指定了程序和Portfolio字段，则会覆盖模板中的程序和模板字段。

   * 如果您是群组管理员，则还可以在您管理的群组的“项目”部分创建项目。 有关更多信息，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >使用组中的模板创建项目时，只有在未指定模板的组字段时，才会在新项目的组字段中显示从中创建项目的组。 如果指定了模板组字段，则新项目的组字段即为模板的组字段。
   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 单击 **新建项目** 要从头开始创建项目。
1. 输入项目的名称。 按Enter键保存名称。

   ![](assets/untitled-project-rename-new-project-nwe-350x127.png)

   项目页面的标题会显示项目当前运行状况和进度的快速概述。 项目标题中的信息会随着项目信息的更新而发生更改。

1. 单击 **开始添加** **任务**.

   或

   单击 **新任务** 向项目添加任务并为其分配资源。\
   有关向项目添加任务的更多信息，请参阅 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. 通过单击&#x200B;**“更多”菜单** 然后 **编辑** ![](assets/qs-edit-icon.png) 项目名称旁边。

   的 **编辑项目** 对话框。

   有关编辑项目的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. （可选）在配置项目设置并添加任务后，您可以将项目的状态更改为 **当前**.

   这表示项目现已准备就绪，可以启动，分配给任务的用户现在可以开始处理这些任务。

   有关项目状态的更多信息，请参阅 [访问系统项目状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
