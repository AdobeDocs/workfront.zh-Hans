---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 配置时间表和小时首选项
description: 作为 [!DNL Adobe Workfront] 管理员，您可以在中指定时间表和小时数的首选项 [!DNL Workfront] 以定义时间表可预填充的项目以及用户可将时间记录到的项目。
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 配置时间表和小时首选项

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为 [!DNL Adobe Workfront] 管理员，您可以在中指定时间表和小时数的首选项 [!DNL Workfront] 以定义时间表可预填充的项目以及用户可将时间记录到的项目。

>[!IMPORTANT]
>
>除了根据本文中所述的条件预填充时间表的项目外，默认情况下，时间表上还会显示以下项目：
>* 您在时间表的时间范围内记录时间的项目
>* 固定到时间表的项目
>* 您搜索并手动添加到时间表的项目。 默认情况下会固定手动添加的项目。
>
>有关更多信息，请参阅 [记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md).



您对时间表所做的任何更改都会影响将来创建的所有时间表。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 设置时间表和小时首选项

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 时间表和小时数]** > **[!UICONTROL 偏好设置]**.

1. 在显示的页面上，在 **[!UICONTROL 常规首选项]** 部分，配置以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL记录未来日期的时间]</td> 
      <td> <p>允许用户在整个系统中记录未来日期的时间，位置如下：</p> 
       <ul> 
        <li>他们有权记录时间的任何项目、任务和问题</li> 
        <li>他们的工时表作为常规时间</li> 
       </ul> <p>当用户计划离开办公室并希望提前记录时间时，这将很有用。</p> <p><b>注释</b>:</p> 
       <p>您无法阻止用户记录已关闭或已取消的任务或问题的时间。 您只能阻止用户记录完成项目或停止项目的时间。 我们建议您在任务和问题列表中使用过滤器，以排除已完成或取消的任务和问题，以免用户看到它们。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[！UICONTROL手动将工作角色分配给小时条目]</td> 
      <td> <p>允许用户手动选择在其用户配置文件中分配或分配给对象的任意工作角色。</p> <p><b>重要</b>：  
        <ul> 
         <li>如果在将工作角色分配给小时条目后禁用此设置，则用户必须在项目、任务或问题的[！UICONTROL小时数]选项卡上调整在各种角色下记录的小时数。</li> 
         <li>如果用户在其配置文件中未分配工作角色，并且在[！UICONTROL高级分配]对话框中有任务被分配为[！UICONTROL任务所有者]，则当用户登录任务时间时，将显示该工作角色。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL限制对所有者和管理员编辑工时表]</td> 
      <td> <p>限制仅对时间表所有者和进行编辑 [!DNL Workfront] 管理员。 禁用此选项后，还可以通过以下方式编辑时间表：</p> 
       <ul> 
        <li> <p>对时间表和小时数的访问级别具有管理访问权限的用户</p> </li> 
        <li> <p>时间表批准者（如果在时间表上启用了“可以编辑小时数”）</p> </li> 
        <li> <p>时间表所有者的经理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL限制对所有者和管理员进行小时编辑]</td> 
      <td>将编辑限制于输入小时数和小时数的用户 [!DNL Workfront] 管理员。 此设置适用于项目或小时报表中的[！UICONTROL小时]选项卡。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 用户可以记录时间的位置]** 部分，配置以下任一选项：

   <table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL直接在项目上记录时间]</td>
        <td>允许用户在项目上记录时间（同时在[！UICONTROL更新]选项卡和时间表上）。 如果用户没有在项目级别记录时间，则此选项应保持未选中状态。</td>
    </tr>
    <tr>
        <td>在已完成的项目上记录时间</td>
        <td>允许用户在标记为完成的项目上记录时间。 如果禁用此选项，则用户无法记录他们在处于[！UICONTROL完成]状态的项目上完成的工作的时间。</td>
    </tr>
    <tr>
        <td>在停止的项目上记录时间</td>
        <td>启用此选项后，用户可以在处于[！UICONTROL Dead]状态的项目上记录小时数。</td>
    </tr>
   </table>

1. 在 **[!UICONTROL 预填充工时表]** 部分，配置以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL内的工作] &lt;number of="" weeks=""&gt; [！UICONTROL工时表的工作范围]</td> 
      <td> <p>定义包含分配给用户的任务和问题日期的时间表日期范围之前和之后的周数。 默认设置为1周，您可以将此范围扩展到4周。 这意味着在为时间表日期范围选择4周后，在时间表日期范围之前的4周到时间表日期范围之后的4周之间的任何时间，都会预填充时间表的任务和问题。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已完成的任务和问题]</td> 
      <td>如果通常将多个资源分配给单个任务，我们建议使用此设置。 这意味着当一个资源记录该任务的时间并将其标记为完成时，分配给该任务的其他资源仍然可以在其时间表中找到该任务或问题，以记录其小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划日期在时间表日期范围内的任务和问题]</td> 
      <td> <p>选择后，时间表包括其计划开始日期或完成日期在时间表日期范围内的任务和问题。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [！UICONTROL计划日期在时间表日期范围内的任务]</td> 
      <td> <p>选择后，时间表包括其预计开始日期或完成日期在项目时间框架内的任务，即使问题或任务的计划日期在时间表日期范围外也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 已删除项目、任务和问题]** 部分，指定以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL删除项目时]</td> 
      <td> 
       <ul> 
        <li><strong>[！UICONTROL保留已作为常规时间添加到时间表的已记录时间]</strong>：如果此项目在稍后时间恢复，则时间会保留在时间表中。</li> 
        <li><strong>[！UICONTROL Delete any logged time]</strong>：如果该项目在稍后时间恢复，则已记录的时间将恢复到项目中。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL删除任务或问题时]</td> 
      <td> 
       <ul> 
        <li><strong>[！UICONTROL将任意已记录的时间移动到任务或问题所在的项目]</strong>：如果该任务或问题在稍后时间恢复，则时间会保留在该项目中。<br></li> 
        <li> <p><strong>[！UICONTROL Delete any logged time]</strong>：如果该任务或问题在稍后时间恢复，则日志记录时间将恢复到任务或问题中。</p> <p>有关这些选项的更多详细信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">删除并恢复对象后的几小时内，[！UICONTROL配置会影响]</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 解锁组的工时表和小时首选项

组织中的组可能需要为其独特工作流以不同方式配置的时间表或小时首选项。 您可以解锁整个组织中所有组的首选项，以便他们能够自行配置首选项。

当某个首选项被解锁且组管理员修改时，如果该组是其主组，则它会影响时间表所有者。

有关组管理员如何为组配置时间表和小时首选项的信息，请参见 [配置组的工时表与小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>之后 [!DNL Workfront] 管理员在系统级别解锁首选项，任何组管理员都可以对其进行配置，然后将其锁定，以确保其组和以下子组中的每个人都使用相同的配置。 这与 [!DNL Workfront] 管理员必须为系统中的每个人配置和锁定首选项。 有关更多信息，请参阅 [锁定或解锁组时间表和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

要解锁项目首选项以便组可以对其进行配置，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 时间表和小时数]**，然后单击 **[!UICONTROL 偏好设置]**.

1. 执行以下任一操作：

   * 如果您希望组管理员能够为其组配置首选项，请将其解锁 ![](assets/unlock-toggle-button.png).
   * 如果您希望所有组都使用首选项的配置，请确保该首选项已锁定（这是默认设置）。

     >[!IMPORTANT]
     >
     >我们建议您与系统中的管理员和用户群组进行通信，以确保以配置锁定首选项的方式考虑所有需求。 锁定后，其配置将由系统中的所有组继承。 如果首选项已解锁任意时间段，则您的配置将替换组管理员可能已做出的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
