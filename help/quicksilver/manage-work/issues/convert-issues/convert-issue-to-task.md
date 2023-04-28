---
product-area: projects
navigation-topic: convert-issues
title: 在Adobe Workfront中将问题转换为任务
description: 如果在提交问题后必须完成更多工作才能完成问题，则可以将问题转换为任务。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 44f01128ef4e6581dc8eaca318a999f2e7274f2a
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 2%

---

# 在Adobe Workfront中将问题转换为任务

如果在提交问题后必须完成更多工作才能完成问题，则可以将问题转换为任务。

有关转换问题的一般信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>编辑对问题、任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p>为项目贡献权限</p> <p>在问题转换后，您将获得任务的“管理”权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将问题转换为任务

1. 转到项目并单击 [!UICONTROL **问题** ] 中。
1. 单击要转换的问题以转到问题的登陆页面。
1. 单击 [!UICONTROL **更多**] 菜单，然后 [!UICONTROL **转换为任务**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >如果问题与批准流程相关联，或者已与解决对象关联，则Workfront会在 [!UICONTROL 转换为项目] 框，通知您在转换期间已删除批准或已覆盖解析对象。 有关更多信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

1. 在 [!UICONTROL 任务名称] 中。 默认情况下，任务的名称将与原始问题的名称相同。

   ![](assets/convert-to-task-box-nwe.png)

1. 单击 [!UICONTROL **目标项目**]，然后开始键入要将新任务放置到的项目名称 [!UICONTROL **目标项目**] 字段，并在其显示在列表中时将其选中。 默认情况下，会选择问题的项目。

1. 单击 [!UICONTROL **概述**]，然后键入 [!UICONTROL **描述**] 任务。

   >[!TIP]
   >
   >   系统或组管理员可以通过修改布局模板来更改转换框左侧面板中各个部分的顺序。

1. （可选和视情况而定）单击 [!UICONTROL **选项**]，请选择下面的任意选项。

   Workfront管理员或组管理员必须先启用这些首选项，然后才能在问题转换过程中看到这些首选项：

   * [!UICONTROL **保留原始问题，并将其解决办法与此任务挂钩**]

      如果取消选择，则删除原始问题。

      >[!NOTE]
      >
      >无权访问或无权删除问题的用户将无法删除问题，因为无论此设置的状态如何，用户都将无法在转换问题时将其删除。 有关问题的访问权限和权限的信息，请参阅：
      >   
      >   * [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **允许（用户名）有权访问此任务**]

      如果未选择，则问题的主要联系人无权访问新任务。

   * [!UICONTROL **保持该问题的计划完成日期**]

      如果未选择，则 [!UICONTROL 计划完成日期] 新任务的 [!UICONTROL 计划开始日期] 任务。 的 [!UICONTROL 计划开始日期] 根据新任务的系统首选项来设置新任务的。

      >[!NOTE]
      >
      >
      >此处显示的选项取决于Workfront管理员如何为系统中的每个人配置这些选项。 有关更多信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >或者，如果贵组织中的顶级组单独配置了这些组，则此处显示的选项取决于哪个组与您在步骤6中选择的项目关联。 有关更多信息，请参阅 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. （可选）单击 [!UICONTROL **自定义Forms**] 并附加新任务的自定义表单。

   >[!TIP]
   >
   >* 如果将附加到问题的多对象自定义表单配置为与问题和任务一起使用，则在转换时，如果问题和任务的自定义表单都存在字段，则表单中保存的所有信息都将保留。
   >* 如果将具有计算字段的多对象自定义表单附加到问题和任务，则问题和任务必须与表单的计算自定义字段中引用的所有字段兼容。 如果出现不兼容的情况，系统会显示一条消息，提醒您进行调整。 有关更多信息，请参阅 [使用旧版表单生成器将计算量度添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
   >* 如果目标项目在编辑项目时在“任务默认自定义Forms”字段中定义了任何默认表单，则这些任务表单也会添加到新任务中。 原始问题与默认任务表单上的字段之间通用的任何自定义字段都会预填充问题字段中的信息。



1. 单击 [!UICONTROL **转换为任务**].

   如果您决定删除原始问题，则问题现在是指定项目上的任务。

   或

   现在，该问题已链接到您所选项目上的新任务，并且如果您决定保留原始问题，则该问题将在任务完成后完成。

   某些问题字段会转移到任务。 有关信息，请参阅 [查看有关项目和任务的原始问题信息](#view-original-issue-information-on-projects-and-tasks) 章节。

1. （可选）根据需要继续编辑任务。

## 查看有关项目和任务的原始问题信息 {#view-original-issue-information-on-projects-and-tasks}

您可以在项目和任务列表和报表中或在“项目详细信息”区域中查看原始问题信息。 有关构建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

下表说明了在转换的项目和任务中显示哪些问题字段。

| 问题字段 | 项目或任务字段 | 项目列表或报表 | 项目详细信息区域 | 任务列表或报表 | 任务详细信息区域 |
|---|---|---|---|---|---|
| [!UICONTROL 问题名称] | [!UICONTROL 转换的问题名称] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL 主要联系人] | [!UICONTROL 已转换的问题创作者名称] | ✔ | ✔ | ✔ |
| [!UICONTROL 输入日期] | [!UICONTROL 转换的问题输入日期] | ✔ |  | ✔ |


>[!CAUTION]
>
>如果 [!UICONTROL 主要联系人] 问题更改或问题在问题转换后从项目或任务中取消链接时， [!UICONTROL 已转换的问题创作者名称 ]不会更新，它会显示原始 [!UICONTROL 主要联系人] 问题时的问题。
