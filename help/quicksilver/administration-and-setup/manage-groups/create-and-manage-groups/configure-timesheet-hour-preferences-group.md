---
user-type: administrator
product-area: system-administration;user-management
keywords: 组，首选项，任务，组，问题，解锁
navigation-topic: create-and-manage-groups
title: 为组配置工时单和小时首选项
description: 在系统级别，Adobe Workfront管理员可以使用解锁工时单和小时首选项部分常规首选项和预填充工时单。 这允许群组管理员为自己的群组单独配置这些部分中的选项。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: df55d6659fac7588610bc05ea0380a766b4277a2
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 1%

---

# 为组配置工时单和小时首选项

Adobe Workfront管理员可以在系统级别解锁以下时间表和小时首选项部分，以便组管理员可以为自己的组单独配置它们：

* 常规偏好设置
* 用户可记录时间的位置
* 预填充工时单

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

“工时单”和“工时首选项”页上的以下部分只能在系统级别进行配置，并且无法为组解锁：

* 删除的项目、任务和问题

有关Workfront管理员如何解锁工时单和小时首选项的信息，请参阅部分 [解锁组的工时单和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>项目首选项以及任务和问题首选项也可以进行组级别配置。 有关信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 组工时单和小时首选项

请考虑以下有关为组配置解锁的时间表或小时首选项的信息：

* 如果您是组管理员，并且为组配置了时间表或小时首选项，则会影响使用该组作为其“主组”的人员。
* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员重新锁定它，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
* 时间表会继承为时间表所有者的“主组”配置的时间表和小时首选项。

   <!--
  Add example here?
  -->

* 在Workfront管理员解锁系统级别的首选项并为组配置该首选项后，您可以将其锁定，以确保您下面组中的每个人都使用相同的配置。 这与Workfront管理员必须为系统中的每个人配置和锁定首选项的功能平行。 有关更多信息，请参阅 [锁定或解锁组时间表和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## 为组配置已解锁的时间表或小时首选项

>[!TIP]
>
>如果您是Workfront管理员，则可以绕过步骤1-4，方法是转到“设置”>“时间表和小时数”>“首选项”，然后在页面顶部的框中搜索组名称。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要配置其工时单或小时首选项的组的名称。
1. 在左侧面板中，单击 **工时单和小时数**.

1. 在显示的页面上， **常规首选项** ，请配置以下任意选项：

   >[!TIP]
   >
   >如果将鼠标悬停在某个首选项上，则会显示一个工具提示来告知您该首选项已锁定，则可以请求Workfront管理员为组织中的所有组解锁该首选项。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">记录未来日期的时间</td> 
      <td> <p>允许用户在以下位置记录整个系统中未来日期的时间：</p> 
       <ul> 
       <li>任何项目、任务和问题，无论项目的组如何，它们都有权访问日志时间</li> 
       <li>他们的工时单作为一般时间</li>
       </ul> 
       <p>当用户计划远离办公室并希望预先记录该时间时，此功能非常有用。</p> 
       <p><b>注意</b>:您无法阻止用户记录关闭或取消的任务或问题的时间。 您只能阻止用户登录已完成或已停用项目的时间。 我们建议您在任务和问题列表中使用过滤器，以排除已完成或已取消的任务和问题对用户可见。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加工时单费用</td> 
      <td> <p>允许用户在工时单中记录时间和费用。</p> 
      <p>当为某个组启用此首选项并将该组设置为某些用户的主组时，这些用户工时单上的项目和任务旁边会显示一个费用图标。 用户可以单击此图标以添加或编辑项目或任务的费用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将作业角色手动分配给小时条目</td> 
      <td> <p>允许用户手动选择在其用户配置文件中分配或分配给对象的任何作业角色。</p> <p><b>重要信息</b>:  
        <ul> 
         <li>如果在将作业角色分配给小时条目后禁用此设置，则用户必须在项目、任务或问题的“小时”选项卡上调整各个角色下记录的小时数。</li> 
         <li>如果用户在其配置文件中没有分配作业角色，并且在“高级分配”对话框中有分配为任务所有者的任务，则当用户记录任务上的时间时，该作业角色即会显示。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">将工时单编辑限制为所有者和管理员</td> 
      <td> <p>将编辑限制为工时单所有者，而不考虑项目的组和Workfront管理员。 禁用此选项时，还可通过以下方式编辑工时单：</p> 
       <ul> 
        <li> <p>在其访问级别具有时间表和小时数管理访问权限的用户</p> </li> 
        <li> <p>工时单批准者（如果在工时单上启用了“可以编辑工时”）</p> </li> 
        <li> <p>时间表所有者的经理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制对所有者和管理员进行小时编辑</td> 
      <td>将编辑限制为输入小时的用户和Workfront管理员。 此设置适用于项目或小时报表中的小时选项卡。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **用户可在其中记录时间** ，请配置以下任意选项：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">直接在项目中记录时间</td> 
      <td>允许用户在项目上记录时间（在“更新”选项卡和时间表上）。 如果要限制用户在项目级别记录时间，请取消选中此选项。</td>
     </tr>
     <tr>
      <td role="rowheader">在项目完成后记录时间</td>
      <td>允许用户记录已标记为完成的项目的时间。 如果禁用此选项，则用户将无法记录在处于“完成”状态的项目上已完成的工作的时间。</td>
     </tr>
     <tr>
      <td role="rowheader">记录已停用项目的时间</td> 
      <td>启用此选项后，用户可以在处于“无效”状态的项目上登录数小时。</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >此首选项基于用户的主组首选项的配置来应用。 如果在用户的“主页组”首选项中启用了这些设置，则无论项目的组首选项是否允许，它们都将能够直接在项目（包括已完成或已终止的项目）上记录时间。

1. 在 **预填充工时单** ，请配置以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">内的工作 &lt;number of="" weeks=""&gt; 工时单的工作范围</td> 
      <td> <p>定义时间表日期范围前后的周数，其中包含分配给用户的任务和问题日期。 默认设置为1周，您可以将此范围延长到4周。 这意味着，如果您为时间范围选择4周，则时间表中会预填充任务和问题，这些任务和问题的日期范围在时间表日期范围之前的四周之间，而日期范围在时间表日期范围之后的四周之间。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已完成的任务和问题</td> 
      <td>如果通常将多个资源分配给单个任务，我们建议设置此设置。 这意味着当一个资源记录任务的时间并标记为完成时，分配给该任务的其他资源仍然可以在其时间表中查找任务或问题，以记录其小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表日期范围内具有计划日期的任务和问题</td> 
      <td> <p>选择时间表后，该时间表包括具有计划起始日期或完成日期的任务和问题，这些任务和问题在时间表的日期范围内。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 在工时单日期范围内具有预计日期的任务</td> 
      <td> <p>选择时间表后，该时间表包括具有预计起始日期或完成日期的任务，该日期在项目的时间范围内，即使问题或任务的计划日期在时间表日期范围之外也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
