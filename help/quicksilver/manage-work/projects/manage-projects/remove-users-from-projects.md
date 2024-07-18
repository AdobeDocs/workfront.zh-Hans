---
product-area: projects;user-management
navigation-topic: manage-projects
title: 从项目中删除用户
description: 当用户不再参与完成项目工作时，您可以从项目中移除用户。
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 从项目中删除用户

当用户不再参与完成项目工作时，您可以从项目中移除用户。 从项目中删除用户会影响任务和问题分配，以及项目角色。 已删除的用户停止接收针对项目团队的通知。 有关项目团队通知的详细信息，请参阅[事件通知类型](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

与项目关联的用户会列在项目的“人员”区域中。 他们代表项目团队。 有关项目团队的详细信息，请参阅[项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 移除用户对现有任务、问题和项目有何影响

从项目中删除用户时，分配给他们的任何任务或问题可能会受到影响，具体取决于删除用户时任务或问题是否已完成：

* **移除用户时该项尚未完成：**&#x200B;如果已经分配了工作角色，或者已将该项重新分配给用户对该项所执行的工作角色，则该项将重新分配给工作角色。 如果项目或用户未分配工作角色，则必须手动重新分配项目。
* **如果删除用户时项已完成：**&#x200B;被删除用户的名称将保留在该项中。
* **如果被移除的用户也是项目的创建者：**&#x200B;该项目未从项目区域其&#x200B;**我所在项目**&#x200B;列表中移除。 该项目将从按“输入者”字段筛选该项目的所有其他用户列表中删除。
* **如果用户是项目所有者或发起人：**&#x200B;用户将保留其作为项目发起人或所有者的角色。

## 从项目和项目团队中删除用户

您可以通过从项目团队中删除用户来从项目中删除用户。

当用户在项目中履行角色时，他们将成为项目团队的一部分。

从用户在项目中的角色中删除用户时，这些用户仍然是项目团队的一部分。

有关用户在项目中的角色的信息，请参阅[管理项目团队](../planning-a-project/manage-project-team.md)。

要从项目团队中删除用户，请执行以下操作：

1. 转到要删除用户的项目。

1. 单击左侧面板中的&#x200B;**人员**，然后选择要删除的用户。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**人员**。

1. 单击用户列表顶部的&#x200B;**删除**&#x200B;图标![删除项](assets/remove-icon---x-in-circle.png)。

1. 单击&#x200B;**是，删除选定的用户**&#x200B;以确认删除。

   用户将从项目团队以及为其分配的任何未完成任务或问题中删除。 他们不再收到针对项目团队的通知。
