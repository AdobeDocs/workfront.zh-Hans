---
product-area: templates
navigation-topic: templates-navigation-topic
title: 从项目中删除模板信息
description: 您无法从项目中删除模板。 您只能手动移除将模板附加到项目后添加到项目中的信息。 有关附加模板的信息，请参阅将模板附加到项目。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# 从项目中删除模板信息

您无法从项目中删除模板。 您只能手动移除将模板附加到项目后添加到项目中的信息。 有关附加模板的信息，请参阅[将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p>
   <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑任务访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对任务的访问 </p> <p>Contribute或更高项目访问权限 </p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 用于从项目中删除模板信息的选项

要删除已添加到项目中的模板信息，您可以执行以下操作之一：

* 在附加模板后，手动从项目中移除信息。

  有关信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

* 删除项目中添加了模板的任务。

  有关信息，请参阅本文中的[删除从模板](#delete-tasks-created-from-a-template)创建的任务。

* 从Workfront中删除模板。 从Workfront中删除模板不会从项目中删除从模板添加的任务。

  有关信息，请参阅[删除项目模板](../../../manage-work/projects/create-and-manage-templates/delete-templates.md)。

## 删除从模板创建的任务 {#delete-tasks-created-from-a-template}

1. 转到项目的&#x200B;**任务**&#x200B;部分。
1. 执行下列操作之一：

   * 为任务列表创建过滤器，以仅显示使用下列语句从模板创建的任务：

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     有关创建筛选器的信息，请参阅[在Adobe Workfront中创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

     应用过滤器时，列表中仅显示与模板任务ID关联的任务。

   * 为任务列表创建视图以在列中显示&#x200B;**模板任务ID**&#x200B;或&#x200B;**模板任务名称**&#x200B;字段。

     在应用视图时，使用模板创建了“模板任务ID”或“模板任务名称”列中包含信息的任务。

     有关创建视图的信息，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

1. 选择步骤2中标识为从模板创建的所有任务，然后单击&#x200B;**删除图标**&#x200B;**>是，删除**。 有关详细信息，请参阅[删除任务](../../../manage-work/tasks/manage-tasks/delete-tasks.md)。
