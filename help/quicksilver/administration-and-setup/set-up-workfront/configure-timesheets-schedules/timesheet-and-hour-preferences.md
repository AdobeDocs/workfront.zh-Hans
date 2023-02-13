---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 配置工时单和工时首选项
description: 作为 [!DNL Adobe Workfront] 管理员，您可以指定工时表和工时的首选项 [!DNL Workfront] 为了定义时间表可以预填充哪些项目，以及用户可以记录哪些项目的时间。
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# 配置工时单和工时首选项

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为 [!DNL Adobe Workfront] 管理员，您可以指定工时表和工时的首选项 [!DNL Workfront] 为了定义时间表可以预填充哪些项目，以及用户可以记录哪些项目的时间。

对工时单所做的任何更改都会影响将来创建的所有工时单。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注释</b>

如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 设置工时单和工时首选项

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 工时单和小时数]** > **[!UICONTROL 首选项]**.

1. 在显示的页面上， **[!UICONTROL 常规首选项]** ，请配置以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL未来日期的日志时间]</td> 
      <td> <p>允许用户在以下位置记录整个系统中未来日期的时间：</p> 
       <ul> 
        <li>任何项目、任务和问题，它们有权访问日志时间</li> 
        <li>他们的工时单作为一般时间</li> 
       </ul> <p>当用户计划远离办公室并希望预先记录该时间时，此功能非常有用。</p> <p><b>注意</b>:您无法阻止用户记录关闭或取消的任务或问题的时间。 您只能阻止用户登录已完成或已停用项目的时间。 我们建议您在任务和问题列表中使用过滤器，以排除已完成或已取消的任务和问题对用户可见。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL手动将作业角色分配给小时条目]</td> 
      <td> <p>允许用户手动选择在其用户配置文件中分配或分配给对象的任何作业角色。</p> <p><b>重要信息</b>:  
        <ul> 
         <li>如果在将作业角色分配给小时条目后禁用此设置，则用户必须在项目、任务或问题的[!UICONTROL Hours]选项卡上调整各种角色下记录的小时数。</li> 
         <li>如果用户在其配置文件中没有分配作业角色，并且在[!UICONTROL Advanced Assignments]对话框中有分配为[!UICONTROL Task Owner]的任务，则当用户记录该任务的时间时，该作业角色即会显示。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL将工时单编辑限制为所有者和管理员]</td> 
      <td> <p>限制对时间表所有者和 [!DNL Workfront] 管理员。 禁用此选项时，还可通过以下方式编辑工时单：</p> 
       <ul> 
        <li> <p>在其访问级别具有时间表和小时数管理访问权限的用户</p> </li> 
        <li> <p>工时单批准者（如果在工时单上启用了“可以编辑工时”）</p> </li> 
        <li> <p>时间表所有者的经理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL限制对所有者和管理员进行小时编辑]</td> 
      <td>将编辑限制为输入小时和 [!DNL Workfront] 管理员。 此设置适用于项目或小时报表中的[!UICONTROL小时]选项卡。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 记录时间]** ，请配置以下任意选项：

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL直接在项目上记录时间]</td>
        <td>允许用户在项目上记录时间（在[!UICONTROL Updates]选项卡和时间表上）。 如果用户未在项目级别记录时间，则应保持未选中此选项。</td>
    </tr>
    <tr>
        <td>在项目完成后记录时间</td>
        <td>允许用户记录已标记为完成的项目的时间。 如果禁用此选项，则用户将无法在[!UICONTROL完成]状态下记录他们在项目上完成的工作的时间。</td>
    </tr>
    <tr>
        <td>记录已停用项目的时间</td>
        <td>启用此选项后，用户可以登录处于[!UICONTROL Dead]状态的项目数小时。</td>
    </tr>
   </table>

1. 在 **[!UICONTROL 使用]**&#x200B;部分，配置以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL内的工作] &lt;number of="" weeks=""&gt; [！时间表工作范围的UICONTROL]</td> 
      <td> <p>定义时间表日期范围前后的周数，其中包含分配给用户的任务和问题日期。 默认设置为1周，您可以将此范围延长到4周。 这意味着，如果您为时间范围选择4周，则时间表中会预填充任务和问题，这些任务和问题的日期范围在时间表日期范围之前的四周之间，而日期范围在时间表日期范围之后的四周之间。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL已完成的任务和问题]</td> 
      <td>如果通常将多个资源分配给单个任务，我们建议设置此设置。 这意味着当一个资源记录任务的时间并标记为完成时，分配给该任务的其他资源仍然可以在其时间表中查找任务或问题，以记录其小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL任务和在时间表日期范围内具有计划日期的问题]</td> 
      <td> <p>选择时间表后，该时间表包括具有计划起始日期或完成日期的任务和问题，这些任务和问题在时间表的日期范围内。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL在时间表日期范围内具有预计日期的任务]</td> 
      <td> <p>选择时间表后，该时间表包括具有预计起始日期或完成日期的任务，该日期在项目的时间范围内，即使问题或任务的计划日期在时间表日期范围之外也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 项目、任务或问题删除首选项]** ，请指定以下内容：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Better title would be Deleting projects, tasks, and issues</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL删除项目时]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL保留已作为一般时间添加到时间表的记录时间]</strong>:如果以后还原此项目，则时间仍保留在时间表上。</li> 
        <li><strong>[!UICONTROL删除任何记录的时间]</strong>:如果此项目稍后还原，则已记录的时间将还原到该项目。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL删除任务或问题时]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL将任何记录的时间移动到任务或问题所在的项目]</strong>:如果此任务或问题稍后恢复，则时间将保留在项目上。<br></li> 
        <li> <p><strong>[!UICONTROL删除任何记录的时间]</strong>:如果此任务或问题稍后还原，则记录的时间会还原到任务或问题。</p> <p>有关这些选项的更多详细信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL配置会影响]删除和还原对象的小时数</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 解锁组的工时单和小时首选项

组织中的组可能需要以不同方式为其独特工作流配置时间表或小时首选项。 您可以解锁组织中所有组的首选项，以便他们可以自行配置该首选项。

解锁首选项并由组管理员修改该首选项后，如果该组是其“主组”，则会影响时间表所有者。

有关组管理员如何为组配置时间表和小时首选项的信息，请参阅 [为组配置工时单和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>在 [!DNL Workfront] 管理员在系统级别解锁首选项，任何组管理员都可以对其进行配置，然后将其锁定，以确保其组和以下子组中的每个人都使用相同的配置。 这与 [!DNL Workfront] 管理员必须为系统中的每个人配置并锁定首选项。 有关更多信息，请参阅 [锁定或解锁组时间表和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

要解锁项目首选项以便组可以对其进行配置，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 工时单和小时数]**，然后单击 **[!UICONTROL 首选项]**.

1. 执行以下任一操作：

   * 如果希望群组管理员能够为其群组配置首选项，请解锁 ![](assets/unlock-toggle-button.png).
   * 如果希望所有组都使用您的配置作为首选项，请确保该配置已锁定（这是默认设置）。

      >[!IMPORTANT]
      >
      >我们建议您与整个系统中的管理员和组中的用户通信，以确保通过配置锁定首选项的方式满足所有需求。 锁定后，系统中的所有组都会继承您的配置。 如果该首选项已在任意时间段内解锁，则您的配置将替换组管理员可能已设置的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
