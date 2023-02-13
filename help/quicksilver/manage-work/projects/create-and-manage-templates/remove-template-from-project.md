---
product-area: templates
navigation-topic: templates-navigation-topic
title: 从项目中删除模板信息
description: 您无法从项目中删除模板。 只有在将模板附加到项目后，您才能手动删除已添加到项目中的信息。 有关附加模板的信息，请参阅将模板附加到项目。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 从项目中删除模板信息

您无法从项目中删除模板。 只有在将模板附加到项目后，您才能手动删除已添加到项目中的信息。 有关附加模板的信息，请参阅 [将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 访问要求

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑任务访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的访问权限 </p> <p>为项目提供更高的访问权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 用于从项目中删除模板信息的选项

要删除已添加到项目中的模板信息，您可以执行以下操作之一：

* 在附加模板后，从项目中手动删除信息。

   有关信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

* 删除项目中随模板一起添加的任务。

   有关信息，请参阅 [删除从模板创建的任务](#delete-tasks-created-from-a-template) 章节。

* 从Workfront中删除模板。 从Workfront中删除模板时，不会从项目中删除从模板添加的任务。

   有关信息，请参阅 [删除项目模板](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## 删除从模板创建的任务 {#delete-tasks-created-from-a-template}

1. 转到 **任务** 的子代。
1. 执行下列操作之一：

   * 为任务列表创建过滤器，以便仅显示使用以下语句从模板创建的任务：

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      有关创建过滤器的信息，请参阅 [在Adobe Workfront中创建或编辑过滤器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      应用过滤器时，列表中只显示与模板任务ID关联的任务。

   * 为任务列表创建视图以显示 **模板任务ID** 或 **模板任务名称** 字段。

      应用视图时，使用模板创建包含“模板任务ID”或“模板任务名称”列中信息的任务。

      有关创建视图的信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 选择步骤2中标识的从模板创建的所有任务，然后单击 **删除图标****>是，删除它**。 有关更多信息，请参阅 [删除任务](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
