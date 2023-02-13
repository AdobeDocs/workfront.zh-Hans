---
title: 将自定义条件设置为项目的默认条件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 如果项目的“条件类型”设置为“进度状态”而不是“手动”，则在项目继续运行时，Adobe Workfront会自动在项目上显示三个内置默认条件（“在目标”、“处于风险”或“处于故障”）中的一个，如项目条件和条件类型概述中所述。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 将自定义条件设置为项目的默认条件

如果项目的“条件类型”设置为“进度状态”而不是“手动”，则在项目继续运行时，Adobe Workfront会自动在项目上显示三个内置默认条件（“在目标”、“处于风险”或“出现故障”）中的一个，如 [项目条件和条件类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

您可以将自定义条件设置为默认条件，而不是使用这些三个内置的默认条件。 例如，您可以将“按目标”默认条件更改为在所有项目中显示为“跟踪良好”。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将自定义条件设置为所有项目的默认条件：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **条件**.

1. 单击 **项目** 选项卡。
1. 单击 **设置默认条件**.
1. 在要更改的默认条件旁边的下拉菜单中，单击要改用的自定义条件。
1. 对要更改的任何其他默认条件重复上一步。
1. 单击&#x200B;**保存**。

有关将自定义条件设置为任务和问题的默认条件的信息，请参阅 [将自定义条件设置为任务和问题的默认条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

有关设置项目以便用户手动更新其条件的信息，请参阅 [任务和问题的更新条件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

有关自定义条件的信息，请参阅 [自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
