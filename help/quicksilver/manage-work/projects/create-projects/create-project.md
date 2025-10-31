---
product-area: projects
navigation-topic: create-projects
title: 创建项目
description: 项目是Adobe Workfront中的一个大型工作单位。 您可以从头开始创建项目，使用模板，或将问题或任务转换为项目。
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 1%

---

# 创建项目

<!--remove Preview and Production references-->

<!-- Audited: 110/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

项目代表在Adobe Workfront中需要完成的大量工作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
        <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在创建项目时，您会自动收到该项目的管理权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->


## 创建项目的方法

您可以使用以下方法之一在Workfront中创建项目：

* 无需使用模板即可从头开始创建项目。 本文介绍了如何从头开始创建项目。

* 复制现有项目。\
  有关复制项目的详细信息，请参阅[复制项目](../../../manage-work/projects/manage-projects/copy-project.md)。

* 使用模板。\
  有关使用模板创建新项目的详细信息，请参阅[使用模板创建项目](../../../manage-work/projects/create-projects/create-project-from-template.md)。

* 从Microsoft项目导入项目。\
  有关从MS Project导入项目的详细信息，请参阅[从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)。

* 使用快速启动导入项目。

  作为Workfront管理员，您可以使用快速启动导入项目。

  有关在Workfront中使用Kick-Start导入数据的信息，请参阅[使用Kick-Start模板将数据导入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

  有关使用Kick-Starts导入项目的信息，请参阅[Kick-Starts方案：简单项目和任务导入准备](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md)。

* 从Adobe Workfront Scenario Planner中的方案发布计划。

  有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。

  有关通过发布计划创建项目的信息，请参阅[通过发布方案规划器](../../../scenario-planner/publish-scenarios-update-projects.md)中的计划来更新或创建项目。

* 在从Workfront Planning中的记录类型连接项目时添加项目。

  有关访问Workfront Planning的信息，请参阅[访问概述](/help/quicksilver/planning/access/access-overview.md)。

  有关通过将项目添加到记录来创建项目的信息，请参阅将项目与记录连接时[从Workfront Planning创建WorkfrontWorkfront对象一节](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## 先决条件

在开始之前，您必须确保：

* 您的系统或组管理员在设置区域中启用了“允许用户在不使用模板的情况下创建项目”偏好设置。

  有关详细信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 新项目默认设置

在创建项目时，Workfront会对其应用一组默认设置。 例如，创建项目时会预设“状态”、“组”和“计划模式”。

请考虑以下事项：

* 作为Workfront管理员或组管理员，您可以在配置整个Workfront实例或组的项目首选项时为新项目配置默认设置。
* Workfront会先应用组的设置（如果有），然后再应用Workfront管理员设置的设置。
* 新项目的默认状态与您的Workfront管理员在主“项目首选项”区域中定义的状态相对应，或与组管理员(或Workfront管理员)在组的“项目首选项”区域中定义的状态相对应。

  >[!NOTE]
  >
  >我们建议新项目的默认状态为“正在计划”。 当您对新项目进行更改时，这将确保不会向分配给项目的用户发送通知。
  >
  >有关为新项目设置默认状态和其他默认设置的详细信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)。

* 以下场景存在于Workfront如何定义新项目的组和状态：

   * 如果从头开始创建项目，则项目的组是您的主组。

     项目的状态是您的主组（如果有）或Workfront实例的项目首选项中的默认状态。 在创建项目时，您可以将默认状态更改为项目组可用的任何状态。

   * 如果使用模板创建项目，则模板中的设置优先于Workfront或组管理员建立的设置。

     新项目的组是模板的组。 如果模板未与组关联，则项目组是创建项目的用户的主组。

     通过模板创建的新项目的默认状态与您的Workfront管理员在主“项目首选项”区域中定义的状态相对应，或与组管理员(或Workfront管理员)在组的“项目首选项”区域中定义的状态相对应。 从模板创建项目时，可以将默认状态更改为项目组的任何状态，即模板的组或创建项目的用户的主组。

   * 如果通过转化问题创建项目，则新项目的组是问题现有项目的组。 如果转化问题的用户无权访问问题的项目或问题的项目没有组，则新项目的组是转化问题的用户的主组。

     新项目的状态与项目关联的组的组状态匹配，即原始项目的组或转换问题的用户的主组。

     如果通过转化问题创建项目时使用模板，请参阅上面第二个场景，了解哪个组和哪个状态Workfront适用于新项目。

## 从头开始创建项目

>[!NOTE]
>
>如果您使用模板创建项目，我们建议您也看到文章[使用模板创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)。

1. 执行下列操作之一：

   * 单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，或Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)（如果可用），然后单击&#x200B;**项目**&#x200B;并展开&#x200B;**新建项目**。
   * 转到项目组合，然后展开&#x200B;**新建项目**。
   * 转到项目群，然后展开&#x200B;**新建项目**。
   * 如果您是组管理员，则还可以在所管理组的项目部分中创建项目。 有关详细信息，请参阅[创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

   ![新建项目菜单](assets/new-project-dropdown-nwe-350x358.png)

1. 单击菜单中的&#x200B;**新建项目**&#x200B;以从头开始创建项目。
1. 键入项目的名称。 按Enter键保存名称。

   ![输入项目的名称](assets/rename-untitled-project.png)

   项目页面的标题显示项目的当前运行状况和进度的快速概述。 项目标题中的信息会随着项目信息的更新而更改。

1. 单击&#x200B;**开始添加任务**。

   或

   单击&#x200B;**新建任务**&#x200B;以将任务添加到项目并为其分配资源。

   有关将任务添加到项目的详细信息，请参阅[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

1. 通过单击项目名称右侧的&#x200B;**更多**&#x200B;菜单（在标题中），然后单击项目名称旁边的&#x200B;**编辑** ![编辑图标](assets/qs-edit-icon.png)来编辑项目详细信息。

   将打开&#x200B;**编辑项目**&#x200B;框。

1. 添加有关项目的信息。

   有关编辑项目的详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

   >[!TIP]
   >
   >项目的状态应为Planning，或其他非当前状态。 这样，您就可以对项目进行更改，而无需向项目参与者生成通知。

1. 单击&#x200B;**保存**&#x200B;以保存更改。

1. （可选）配置项目设置并添加任务后，您可以在项目标题中将项目状态更改为&#x200B;**当前**。

   这表示项目现在已准备好开始，并且分配给任务的用户现在可以开始处理这些任务。

   有关项目状态的详细信息，请参阅[访问系统项目状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)。
