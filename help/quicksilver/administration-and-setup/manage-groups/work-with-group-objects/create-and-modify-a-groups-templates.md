---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改组的项目模板
description: 在“组”区域中查看由您管理的组时，可以查看和使用与该组及其任何子组关联的项目模板。
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

在“组”区域中查看由您管理的组时，可以查看和使用与该组及其任何子组关联的项目模板。

如果您的组上有任何组，则其管理员也可以为您的组执行这些操作。 Workfront管理员（对于任何组）也是如此。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要查看和使用的模板的访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 从“组”区域查看、处理和创建组的模板

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要为其创建或修改模板的组名称。
1. 在左侧面板中，单击 **模板** 列出与群组及其可能拥有的任何子群组关联的模板。

   您必须拥有模板的查看访问权限才能在此列表中查看模板。 有关此访问的信息，请参阅 [授予对模板的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. 执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加模板</td> 
      <td> <p>单击 <strong>新模板</strong>，然后使用可用选项对其进行配置。 有关这些选项的信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">创建项目模板</a>.</p> <p>模板会自动与组关联。</p> <p>有关组首选项如何应用于新模板的信息，请参阅 <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">首选项如何应用于模板和模板任务</a> 在本文中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑一个或多个模板</td> 
      <td> <p>至少选择一个模板，单击编辑图标 <img src="assets/edit-icon.png">，然后使用任意可用选项对其进行配置。 有关这些选项的信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">编辑项目模板</a>.</p> <p>仅当您有权编辑所选所有模板时，才可使用“编辑”图标。 有关此访问的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除一个或多个模板</td> 
      <td> <p>至少选择一个模板，然后单击删除图标 <img src="assets/delete.png">.</p> <p>仅当您有权编辑所选所有模板时，此图标才可用。 有关此访问的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共享一个或多个模板</td> 
      <td> <p>至少选择一个模板，单击共享图标 <img src="assets/share-icon.png">，然后在下拉菜单中单击以下选项之一：</p> 
       <ul> 
        <li> <p><strong>模板</strong>:在 <strong>模板访问</strong> 框中，添加名称以指定您希望对模板本身具有访问权限的对象。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">共享模板</a> 在文章中 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">共享项目模板</a>.</p> </li> 
        <li><strong>项目</strong>:在 <strong>项目访问</strong> 框中，添加名称以指定您希望有权访问从模板创建的项目的对象</li> 
       </ul> <p>仅当您拥有对所选所有模板的共享访问权限时，“共享”图标才可用。 有关此访问的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予对模板的访问权限</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出模板列表</td> 
      <td>单击 <strong>导出</strong> <img src="assets/export.png">，然后为导出列表选择所需的文件格式。</td> 
     </tr> 
    </tbody> 
   </table>

## 首选项如何应用于模板和模板任务 {#how-preferences-apply-to-templates-and-template-tasks}

创建项目模板时，下表中列出的设置将通过关联项目或任务首选项自动进行配置。

>[!NOTE]
>
>组级或系统级项目或任务首选项会影响项目模板，具体取决于您在创建模板时是否将该模板与组关联。
>
>如果确实将其与某个组关联，则会生效组级别首选项。 这种情况发生在以下情况中：
>
>* 如本文所述，您可以从“组”区域创建模板
>* 在使用Kickstart文件创建模板时指定组
>* 在使用API创建模板时指定组
>
>如果未将新模板与组关联，则系统级别首选项生效。 在以下情况下，会发生这种情况。 （如果您稍后为模板或模板任务分配了组，则组的首选项不会影响该任务。）
>
>* 从“模板”区域创建模板
>* 使用Kickstart文件创建模板时，不指定组
>* 使用API创建模板时，您没有指定组
>


* [由项目和任务首选项配置的项目模板设置](#project-template-settings-configured-by-project-and-task-preferences)
* [由任务首选项配置的模板任务设置](#template-task-settings-configured-by-task-preferences)

### 由项目和任务首选项配置的项目模板设置 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>绩效指数方法</p> </td> 
   <td> <p>如果将新模板与组关联，则由组级项目首选项“性能索引方法”进行配置；如果不关联，则由相同的系统级项目首选项进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完成情况类型</p> </td> 
   <td> <p>如果将新模板与组关联，则由组级项目首选项“根据进度状态自动设置项目的条件”进行配置；如果未将新模板与组关联，则由同一系统级项目首选项进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>计划自</p> </td> 
   <td> <p>如果将新模板与组关联，则由组级项目首选项“计划自”进行配置；如果不关联，则由同一系统级项目首选项进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>用户关机时间</p> </td> 
   <td> <p>如果您将新模板与组关联，则由组级项目首选项“用户关闭时间”进行配置；如果您未关联，则由相同的系统级项目首选项进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新类型</p> </td> 
   <td> <p>如果将新模板与组关联，则由组级项目首选项“将自动重新计算项目时间轴”进行配置；如果不关联，则由同一系统级项目首选项进行配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>访问部分设置</p> </td> 
   <td> <p>如果将新模板与组关联，则由“访问”部分的组级任务首选项配置；如果不关联，则由相同的系统级项目首选项配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中列出的项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

有关任务和问题首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* 如果更改与现有项目模板关联的组，则模板的设置将保持不变。
>* 如果将现有模板任务移动到其他模板，则无论与新模板关联的组是什么，模板任务中的以下设置都将保持不变：>
   >   * 持续时间类型
   >   * 收入类型
   >   * 成本类型
>
>  但是，模板任务会受新模板上的“将某人分配到任务时”设置的影响。 有关更多信息，请参阅 [访问](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 在文章中 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* 当管理员将项目另存为模板时，该模板的所有设置都会继承自项目，包括该组。
>
>  当管理员使用模板将任务或问题转换为项目时，模板的所有设置取决于模板上已保存的内容。

### 由任务首选项配置的模板任务设置 {#template-task-settings-configured-by-task-preferences}

创建模板任务时，其某些设置会通过关联任务首选项自动配置。 下表列出了这些设置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>持续时间类型 </p> </td> 
   <td> <p>如果将模板与组关联，则由组级任务首选项“持续时间类型”配置；如果不关联，则由相同的系统级任务和问题首选项配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收入类型</p> </td> 
   <td> <p>如果将模板与组关联，则由组级任务首选项“收入类型”配置；如果不关联，则由同一系统级任务和问题首选项配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>成本类型 </p> </td> 
   <td> <p> 如果将模板与组关联，则由组层任务首选项“成本类型”配置；如果不关联，则由同一系统层任务和问题首选项配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中列出的任务首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
