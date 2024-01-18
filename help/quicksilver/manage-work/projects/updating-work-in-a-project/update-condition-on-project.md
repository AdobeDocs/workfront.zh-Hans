---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新项目完成情况
description: 项目的状态为置于其上的标志，用于指示与其关联的工作是否进展顺利，或者您是否遇到任何障碍。 这与项目的状态不同，后者指示您是否正在积极处理项目。
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 更新项目完成情况

项目的状态为置于其上的标志，用于指示与其关联的工作是否进展顺利，或者您是否遇到任何障碍。 这与项目的状态不同，后者指示您是否正在积极处理项目。

您可以自动或手动设置项目的条件。 要手动更改项目的完成情况，您必须是项目所有者或具有项目管理权限。

Adobe Workfront管理员可以为您的环境创建自定义条件，如中所述 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>

对于新许可证：
<p>标准</p>

对于当前许可证：
<ul><li><p>计划</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p> <p>编辑对任务和问题的访问权限 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看任务或问题的或更高权限以查看其完成情况</p>
   <p>管理任务和问题的权限以更新条件</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 自动设置条件

自动设置项目条件由项目的条件类型确定。 完成情况类型必须设置为“进度状态”，Workfront才能自动设置项目完成情况。

在“设置”区域中设置项目首选项时，您的Workfront或组管理员会为系统中的新项目确定“条件类型”字段的默认值。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

创建项目时，会自动设置项目的完成情况以匹配当时的项目进度状态。 项目的进度状态基于项目上任务的进度。

有关项目完成情况以及如何根据进度状态计算项目完成情况的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## 手动更新项目的条件

如果将项目的“完成情况类型”设置为“手动”而不是“进度状态”，则可以手动更新项目的完成情况。

1. 转到要更新条件的项目。
1. 单击 **项目详细信息** 部分。

1. 确保 **完成情况类型** 字段设置为 **手动**.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. 在 **条件** 字段，从以下选项中选择符合您对与其关联的工作是否顺利进行或者是否有任何延迟的理解的选项：

   * **准时**
   * **处于风险**
   * **存在问题**

   有关项目条件的更多信息，请参阅 [项目完成情况和完成情况类型概览](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >可以为您的环境自定义条件，因此您可能会在环境中找到三个以上的条件选项。 条件的名称可能与上面列出的名称不同。 有关在Workfront中自定义条件的信息，请参阅 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. 单击 **保存更改**.
