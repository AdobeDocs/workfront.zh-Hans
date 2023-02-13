---
product-area: projects
navigation-topic: manage-issues
title: 删除问题
description: 如果您具有正确的访问权限和权限，则可以删除Adobe Workfront中的问题或请求。
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 删除问题

如果您具有正确的访问权限和权限，则可以删除Adobe Workfront中的问题或请求。

>[!TIP]
>
>“问题”和“请求”在Workfront中可互换使用。 您可以记录项目和任务中的问题，以指明需要解决的未预见工作。 您还可以提交被记录为指定为请求队列的项目问题的请求。

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
   <td> <p>请求或更高版本</p> <p>查看或获得更高许可，以删除项目“问题”部分中的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>对项目或任务提供或更高权限</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关删除问题的注意事项

* 您的Workfront管理员或组管理员必须在项目首选项区域中启用删除状态为“完成”的项目中的问题。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果问题已记录小时数，Workfront管理员或组管理员必须通过在Workfront实例中配置任务和问题首选项来允许删除这些问题。 当您尝试删除在登录时出现小时数问题的项目时，也会出现这种情况。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   有关启用删除记录小时数的问题的更多信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 删除问题的影响

删除问题时，会影响链接到该问题的其他对象。

在删除问题时，还会删除附加到问题的以下对象：

* 文档

   您无法删除附加了已签出文档的问题。 有关签出文档的更多信息，请参阅 [签出文档](../../../documents/managing-documents/check-out-documents.md).

* 注释
* 审批

根据Workfront或组管理员在 **时间表和小时首选项** 在您的Workfront实例中，在删除问题时，会通过以下方式之一处理问题记录的小时数：

* 移到项目，如果稍后还原了问题，则将无法在问题上还原。
* 如果以后还原了问题，则将删除并在问题上还原。

   当您尝试删除任务已记录小时的项目时，也会出现这种情况。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   有关为记录问题的小时配置删除首选项的详细信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 分配给问题或问题批准的用户仍保留在项目团队中。\
   有关项目团队的更多信息，请参阅 [项目团队概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 删除问题

* [同时删除项目中的多个问题](#delete-multiple-issues-in-a-project-simultaneously)
* [删除单个问题](#delete-a-single-issue)

### 同时删除项目中的多个问题  {#delete-multiple-issues-in-a-project-simultaneously}

1. 转到 **主菜单**.
1. 单击 **项目**.
1. 单击包含要删除的问题的项目名称。
1. 单击 **问题** 中。
1. 选择问题，然后单击 **删除** 图标 ![](assets/delete.png) 列表顶部。

1. 如果允许删除，请单击 **是，删除它**.\
   您的Workfront管理员可能不允许删除记录小时数的问题。\
   有关删除问题所需的访问权限和权限的更多信息，请参阅 [删除问题](#access-and-permissions-needed).

### 删除单个问题 {#delete-a-single-issue}

1. 单击 **主要** 菜单。
1. 单击 **项目**.
1. 单击包含要删除的问题的项目名称。
1. 单击 **问题** 中。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 单击要删除的问题的名称。
1. 单击 **更多** 菜单。

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. 单击 **删除**.
1. 如果允许删除，请单击 **是，删除它**.

   您的Workfront管理员可能不允许删除记录小时数的问题。\
   有关删除问题所需的访问权限和权限的更多信息，请参阅 [删除问题](#access-and-permissions-needed).

## 恢复已删除的问题

Workfront或组管理员可以在问题被删除后的30天内恢复它们。 有关在Workfront中恢复项目的更多信息，请参阅 [恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
