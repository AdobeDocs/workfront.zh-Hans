---
product-area: projects
navigation-topic: convert-issues
title: 在Adobe Workfront中将问题转化为任务
description: 如果在提交问题后必须完成更多工作才能完成问题，则可以将问题转换为任务。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# 在Adobe Workfront中将问题转化为任务

如果在提交问题后必须完成更多工作才能完成问题，则可以将问题转换为任务。

有关转换问题的一般信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题、任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p>参与项目的权限</p> <p>在问题转化后，您可获得该任务的管理权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将问题转化为任务

1. 转到项目，然后单击左侧面板中的&#x200B;[!UICONTROL **问题**]。
1. 单击要转换的问题，以转到问题的登陆页面。
1. 单击问题上的&#x200B;[!UICONTROL **更多**]&#x200B;菜单，然后单击&#x200B;[!UICONTROL **转换为任务**]。

   ![问题更多菜单](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >如果问题与审批流程相关联或已经与解析对象关联，则Workfront将在[!UICONTROL 转化为项目]框的顶部显示警告，以通知您审批被移除或在转换期间解析对象被覆盖。 有关详细信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. 更新[!UICONTROL 任务名称]分区中的任务名称。 默认情况下，任务的名称将与原始问题的名称相同。

   ![转换为任务框](assets/convert-to-task-box-nwe.png)

1. 单击&#x200B;[!UICONTROL **目标项目**]，然后开始在&#x200B;[!UICONTROL **目标项目**]&#x200B;字段中键入要将新任务放置到的项目的名称，并在该名称显示在列表中时将其选定。 默认情况下，选择问题的项目。

1. 单击&#x200B;[!UICONTROL **概述**]，然后为任务键入&#x200B;[!UICONTROL **描述**]。

   >[!TIP]
   >
   >   系统或组管理员可以通过修改布局模板来更改转换框左侧面板中部分的顺序。

1. （可选且有条件）单击&#x200B;[!UICONTROL **选项**]，选择以下任意选项。

   Workfront管理员或组管理员必须启用这些首选项，然后才能在转换问题期间显示：

   * [!UICONTROL **保留原来的问题，并将其解决方案与此任务绑定**]

     如果未选中，则会删除原始问题。

     >[!NOTE]
     >
     >无权删除问题的用户将无法删除问题，因为他们正在转换问题，无论此设置的状态如何。 有关对问题的访问和权限的信息，请参阅：
     >   
     >   * [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **允许（用户名）访问此任务**]

     如果未选中，问题的主要联系人将无权访问新任务。

   * [!UICONTROL **保留问题的计划完成日期**]

     如果未选中，则从任务的[!UICONTROL 计划开始日期]开始计算新任务的[!UICONTROL 计划完成日期]。 新任务的[!UICONTROL 计划开始日期]是根据新任务的系统首选项设置的。

     >[!NOTE]
     >
     >
     >此处显示的选项取决于Workfront管理员如何为系统中的每个人配置这些选项。 有关详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
     >
     >或者，如果贵组织中的顶级组单独配置了它们，则此处显示的选项取决于与您在步骤6中选择的项目关联的组。 有关详细信息，请参阅[为组配置任务和问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

1. （可选）单击&#x200B;[!UICONTROL **自定义Forms**]&#x200B;并为新任务附加自定义表单。

   >[!TIP]
   >
   >* 如果将附加到问题的多对象自定义表单配置为同时与问题和任务一起使用，则在进行转换时，如果问题中以及任务的自定义表单中存在字段，则保留表单中保存的所有信息。
   >* 如果将具有计算字段的多对象自定义表单附加到问题和任务，则问题和任务必须与表单的计算自定义字段中引用的所有字段兼容。 如果存在不兼容的情况，则会显示一条消息，提醒您进行调整。 有关详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。
   >* 如果目标项目在编辑项目时在任务默认自定义Forms字段中定义了任何默认表单，则这些任务表单也会添加到新任务中。 原始问题和默认任务表单上的字段之间通用的任何自定义字段会预填充问题字段中的信息。


1. 单击&#x200B;[!UICONTROL **转换为任务**]。

   如果您决定删除原始问题，则问题现在为指定项目上的任务。

   或

   问题现在链接到您所选项目中的新任务，并且一旦任务完成（如果您决定保留原始问题），问题就会完成。

   某些问题字段传输到任务。 有关信息，请参阅本文中的[查看有关项目和任务的原始问题信息](#view-original-issue-information-on-projects-and-tasks)部分。

1. （可选）根据需要继续编辑任务。

## 查看有关项目和任务的原始问题信息 {#view-original-issue-information-on-projects-and-tasks}

您可以在项目、任务列表和报告或项目详细信息区域中查看原始问题信息。 有关生成报表的信息，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

下表说明了哪些问题字段在转换后的项目和任务中可见。

| 问题字段 | 项目或任务字段 | 项目列表或报告 | 项目详细信息区域 | 任务列表或报告 | 任务详细信息区域 |
|---|---|---|---|---|---|
| [!UICONTROL 问题名称] | [!UICONTROL 转换的问题名称] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL 主要联系人] | [!UICONTROL 转换的问题发起人姓名] | ✔ | ✔ | ✔ |
| [!UICONTROL 输入日期] | [!UICONTROL 转换的问题输入日期] | ✔ |  | ✔ |


>[!CAUTION]
>
>如果问题的[!UICONTROL 主要联系人]发生更改，或者在问题转换之后问题变得与项目或任务取消链接，则[!UICONTROL 转换的问题发起人姓名]不会更新，并且会在问题转换时显示问题的原始[!UICONTROL 主要联系人]。
