---
title: 将自定义条件设置为项目的默认值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 如果项目的完成情况类型被设置为“进度状态”而不是“手动”，Adobe Workfront会在项目进行时自动显示三个内置默认完成情况之一（“准时”、“处于风险中”或“存在问题”），如项目完成情况和完成情况类型概述中所述。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 2%

---

# 将自定义条件设置为项目的默认值

如果项目的完成情况类型设置为“进度状态”而不是“手动”，Adobe Workfront会在项目进行时自动显示三个内置默认完成情况之一（“准时”、“处于风险中”或“存在问题”），如[项目完成情况和完成情况类型概述](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)中所述。

![项目标题和详细信息中的完成情况](assets/condition-of-project-0825.png)

您可以将自定义条件设置为默认条件，而不是使用这三个内置的默认条件。 例如，您可以更改“按目标”默认条件，使其在所有项目中均显示为跟踪良好。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将自定义条件设置为所有项目的默认条件：

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **条件**。

1. 单击&#x200B;**项目**&#x200B;选项卡。
1. 单击&#x200B;**设置默认条件**。
1. 在要更改的默认条件的下拉菜单中，单击要改用的自定义条件。
1. 对要更改的任何其他默认条件重复上一步骤。
1. 单击&#x200B;**保存**。

有关将自定义条件设置为任务和问题的默认条件的信息，请参阅[将自定义条件设置为任务和问题的默认值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)。

有关设置项目以便用户可以手动更新其条件的信息，请参阅[任务和问题的更新条件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)。
