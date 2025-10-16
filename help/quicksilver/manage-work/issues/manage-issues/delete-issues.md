---
product-area: projects
navigation-topic: manage-issues
title: 删除问题
description: 如果您拥有正确的访问权限，可以在Adobe Workfront中删除问题或请求，并在您发现不再需要它们时，再进行删除。 我们建议关闭这些项目，而不是删除它们，这样您可以保留项目的准确性。
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 1%

---

# 删除问题

<!--Audited: 08/2025-->

如果您拥有正确的访问权限，可以在Adobe Workfront中删除问题或请求，并在您发现不再需要它们时，再进行删除。 我们建议关闭这些项目，而不是删除它们，这样您可以保留项目的准确性。

Workfront管理员可以恢复已删除的问题。

>[!TIP]
>
>“问题”和“请求”在Workfront中可互换使用。 您可以同时记录项目和任务中的问题以指示需要解决的意外工作。 您还可以提交在指定为请求队列的项目中记录为问题的请求。

## 访问要求

+++ 展开以查看访问要求。 

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
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>项目或任务的Contribute或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除问题的注意事项

* 您的Workfront管理员或组管理员必须在项目偏好设置区域中启用删除状态为“完成”的项目中的问题。

  有关设置项目首选项的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 如果问题记录了小时数，Workfront管理员或组管理员必须通过在Workfront实例中配置任务和问题首选项来允许删除这些问题。 当您尝试删除在登录有小时数的项目时，这也适用。

  有关启用删除记录小时数的问题的详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)中的“删除”部分。


## 删除问题的影响

删除问题时，会影响链接到问题的其他对象。

当您删除问题时，以下附加到问题的对象也会被删除：

* 文档

  您无法删除附加了已签出文档的问题。 有关签出文档的更多信息，请参阅[签出文档](../../../documents/managing-documents/check-out-documents.md)。

* 注释
* 审批

根据Workfront或组管理员在Workfront实例的&#x200B;**时间表和小时首选项**&#x200B;中配置项目、任务或问题删除首选项的方式，在删除问题时，会以下列方式之一处理为问题记录的小时数：

* 移至项目，如果该问题稍后恢复，则不会恢复该问题。
* 将被删除，如果问题稍后恢复，将恢复该问题。

  当您尝试删除具有已登录小时数的任务的项目时，这也适用。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  有关为登录问题的小时数配置删除首选项的详细信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

* 分配给问题或问题批准的用户仍保留在项目团队中。\
  有关项目团队的详细信息，请参阅[项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

## 删除问题

### 同时删除项目中的多个问题  {#delete-multiple-issues-in-a-project-simultaneously}

1. 转到&#x200B;**主菜单**。
1. 单击&#x200B;**项目**。
1. 单击包含要删除的问题的项目名称。
1. 单击左侧面板中的&#x200B;**问题**。

   与所选项目关联的问题列表将显示在右侧。
1. 选择列表中的一个或多个问题，然后单击列表顶部的&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

1. 如果允许删除，请单击&#x200B;**删除**。

   您的Workfront管理员可能不允许删除记录小时数的问题。\
   有关删除问题所需的访问和权限的更多信息，请参阅本文中的[删除问题的注意事项](#considerations-for-deleting-issues)部分。

### 删除单个问题 {#delete-a-single-issue}

{{step1-to-projects}}

1. 单击包含要删除的问题的项目名称。
1. 单击左侧面板中的&#x200B;**问题**。

   左侧面板中的![问题部分](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 单击要删除的问题的名称。
1. 单击问题名称右侧的&#x200B;**更多**&#x200B;菜单。

   ![问题更多菜单](assets/qs-issue-more-menu-highlighted-350x469.png)

1. 单击&#x200B;**删除问题**。
1. 单击&#x200B;**删除**&#x200B;至。

   >[!NOTE]
   >
   >  您的Workfront管理员可能不允许删除记录小时数的问题。\
   >  有关删除问题所需的访问和权限的更多信息，请参阅本文中的[删除问题的注意事项](#considerations-for-deleting-issues)部分。

## 恢复已删除的问题

Workfront或组管理员可以在问题删除后的30天内恢复问题。

有关在Workfront中还原项目的详细信息，请参阅[还原已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。
