---
title: 将自定义条件设置为项目的默认值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 如果项目的完成情况类型被设置为“进度状态”而不是“手动”，Adobe Workfront会在项目进行时自动显示三个内置默认完成情况之一（“准时”、“处于风险中”或“存在问题”），如项目完成情况和完成情况类型概述中所述。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 将自定义条件设置为项目的默认值

如果项目的完成情况类型设置为“进度状态”而不是“手动”，Adobe Workfront会在项目进行时自动显示三个内置默认完成情况之一（“准时”、“处于风险中”或“存在问题”），如[项目完成情况和完成情况类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)中所述。

![](assets/condition-in-project-header-nwe.png)

您可以将自定义条件设置为默认条件，而不是使用这三个内置的默认条件。 例如，您可以更改“按目标”默认条件，使其在所有项目中均显示为跟踪良好。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将自定义条件设置为所有项目的默认条件：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 单击&#x200B;**项目首选项** > **条件**。

1. 单击&#x200B;**项目**&#x200B;选项卡。
1. 单击&#x200B;**设置默认条件**。
1. 在要更改的默认条件旁边的下拉菜单中，单击要改用的自定义条件。
1. 对要更改的任何其他默认条件重复上一步骤。
1. 单击&#x200B;**保存**。

有关将自定义条件设置为任务和问题的默认条件的信息，请参阅[将自定义条件设置为任务和问题的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)。

有关设置项目以便用户可以手动更新其条件的信息，请参阅[更新任务和问题的条件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)。

有关自定义条件的信息，请参阅[自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)。
