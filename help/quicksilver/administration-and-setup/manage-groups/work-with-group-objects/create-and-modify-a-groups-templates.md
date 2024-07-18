---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改组的项目模板
description: 在组区域查看您管理的组时，您可以查看和使用与该组及其任何子组相关联的项目模板。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# 创建和修改组的项目模板

在组区域查看您管理的组时，您可以查看和使用与该组及其任何子组相关联的项目模板。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看您想要查看和使用的模板的访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

## 从组区域查看、处理和创建组模板

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

1. 单击要为其创建或修改模板的组的名称。
1. 在左侧面板中，单击&#x200B;**模板**&#x200B;可列出与组及其可能具有的任何子组关联的模板。

   您必须具有模板的查看权限才能在此列表中查看模板。 有关此访问权限的信息，请参阅[授予对模板的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)。

1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加模板</td> 
      <td> <p>单击<strong>新建模板</strong>，然后使用可用选项对其进行配置。 有关这些选项的信息，请参阅<a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">创建项目模板</a>。</p> <p>模板会自动与组关联。</p> <p>有关如何将组首选项应用于新模板的信息，请参阅本文中的<a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">如何将首选项应用于模板和模板任务</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑一个或多个模板</td> 
      <td> <p>至少选择一个模板，单击“编辑”图标<img src="assets/edit-icon.png">，然后使用任何可用选项对其进行配置。 有关这些选项的信息，请参阅<a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>。</p> <p>只有您对所有选定的模板具有“编辑”权限时，“编辑”图标才可用。 有关此访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除一个或多个模板</td> 
      <td> <p>至少选择一个模板，然后单击“删除”图标<img src="assets/delete.png">。</p> <p>此图标仅在您具有所有选定模板的“编辑”权限时可用。 有关此访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共享一个或多个模板</td> 
      <td> <p>至少选择一个模板，单击“共享”图标<img src="assets/share-icon.png">，然后在下拉菜单中单击以下选项之一：</p> 
       <ul> 
        <li> <p><strong>模板</strong>：在显示的<strong>模板访问</strong>框中，添加名称以指定您希望谁有权访问模板本身。</p> <p>有关详细信息，请参阅<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">共享项目模板</a>一文中的<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">共享模板</a>部分。</p> </li> 
        <li><strong>项目</strong>：在显示的<strong>项目访问</strong>框中，添加名称以指定您希望谁有权访问使用该模板创建的项目</li> 
       </ul> <p>仅当您对选择的所有模板具有“共享”访问权限时，“共享”图标才可用。 有关此访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出模板列表</td> 
      <td>单击<strong>导出</strong> <img src="assets/export.png">，然后为导出的列表选择所需的文件格式。</td> 
     </tr> 
    </tbody> 
   </table>

## 首选项如何应用于模板和模板任务 {#how-preferences-apply-to-templates-and-template-tasks}

在创建项目模板时，下表列出的设置由关联的项目或任务首选项自动配置。

>[!NOTE]
>
>组级别或系统级别的项目或任务首选项会影响项目模板，具体取决于您在创建项目模板时是否将该模板与组相关联。
>
>如果您确实将其与组相关联，则组级别首选项将生效。 这发生在以下情况中：
>
>* 您可以从组区域创建模板，如本文所述
>* 在使用Kickstart文件创建模板时指定组
>* 在使用API创建模板时指定组
>
>如果未将新模板与组相关联，则系统级别的首选项将生效。 在以下场景中，会发生这种情况。 （如果以后将组分配给模板或模板任务，则该组的首选项不会影响它。）
>
>* 从“模板”区域创建模板
>* 使用Kickstart文件创建模板时未指定组
>* 使用API创建模板时，未指定组
>

* [项目和任务首选项配置的项目模板设置](#project-template-settings-configured-by-project-and-task-preferences)
* [由任务首选项配置的模板任务设置](#template-task-settings-configured-by-task-preferences)

### 项目和任务首选项配置的项目模板设置 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>绩效指数方法</p> </td> 
   <td> <p>由组级别项目首选项“绩效指数方法”（如果将新模板与组关联）配置，或者由相同的系统级别项目首选项（如果不关联）配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完成情况类型</p> </td> 
   <td> <p>如果您将新模板与组关联，则由组级别项目首选项“根据进度状态自动设置项目条件”配置；如果未关联，则使用相同系统级别项目首选项。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>时间表开始日期</p> </td> 
   <td> <p>如果您将新模板与组关联，则由组级别项目首选项“计划自”配置；如果您未关联，则由相同系统级别项目首选项配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>用户空闲时间</p> </td> 
   <td> <p>如果您将新模板与组关联，则由组级别项目首选项“用户休息时间”配置；如果您未关联，则由相同系统级别项目首选项配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新类型</p> </td> 
   <td> <p>如果您将新模板与组关联，则由组级别项目偏好设置配置“项目时间线将自动重新计算”；如果您未关联，则使用相同的系统级别项目偏好设置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>访问部分设置</p> </td> 
   <td> <p>如果您将新模板与组关联，则由“访问”部分中的组级别任务首选项配置；如果您未关联，则由相同的系统级别项目首选项配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中列出的项目首选项的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

有关任务和问题首选项的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!NOTE]
>
>* 如果更改与现有项目模板关联的组，则模板的设置将保持不变。
>* 如果将现有模板任务移动到另一个模板，则无论与新模板关联的组如何，模板任务中的以下设置均保持不变：>
>   * 持续时间类型
>   * 收入类型
>   * 成本类型
>
>  但是，模板任务受新模板上的“将某人分配给任务时”设置的影响。 有关详细信息，请参阅文章[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)中的[访问](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access)部分。
>
>* 当管理员将项目另存为模板时，模板的所有设置都继承自该项目，包括组。
>
>  当管理员使用模板将任务或问题转化为项目时，模板的所有设置取决于模板上已保存的内容。
>

### 由任务首选项配置的模板任务设置 {#template-task-settings-configured-by-task-preferences}

创建模板任务时，其某些设置会通过相关任务首选项自动配置。 下表列出了这些设置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>持续时间类型 </p> </td> 
   <td> <p>由组级别任务首选项“持续时间类型”（如果将模板与组关联）配置，或者由相同的系统级别任务和问题首选项（如果不关联）配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收入类型</p> </td> 
   <td> <p>由组级别任务首选项“收入类型”（如果将模板与组关联）配置，或相同的系统级别任务和问题首选项（如果不关联）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>成本类型 </p> </td> 
   <td> <p> 由组级别任务首选项“成本类型”（如果将模板与组关联）配置，或者由相同的系统级别任务和问题首选项（如果不关联）配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中列出的任务首选项的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
