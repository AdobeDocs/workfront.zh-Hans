---
user-type: administrator
product-area: system-administration;user-management
keywords: 组，首选项，任务，组，问题，解锁
navigation-topic: create-and-manage-groups
title: 配置组的工时表与小时首选项
description: 在系统级别，Adobe Workfront管理员可以使用解锁时间表和小时首选项部分“常规首选项”和“预填充时间表”。 这允许组管理员为自己的组独立配置这些部分中的选项。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1379'
ht-degree: 1%

---

# 配置组的工时表与小时首选项

Adobe Workfront管理员可以在系统级别解锁时间表和小时首选项的以下部分，以便组管理员可以独立为自己的组配置这些部分：

* 常规偏好设置
* 用户可记录时间的位置
* 预填充工时表

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

“时间表”和“小时首选项”页上的以下部分只能在系统级别配置，并且无法为组解锁：

* 删除的项目、任务和问题

有关Workfront管理员如何解锁时间表和小时首选项的信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)文章中的[解锁组的时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock)部分。

>[!TIP]
>
>对于项目首选项以及任务和问题首选项，也可以使用组级别配置。 有关信息，请参阅[配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

+++

## 组时间表和小时首选项

考虑以下有关为组配置解锁时间表或小时首选项的信息：

* 如果您是组管理员，并为组配置时间表或小时首选项，则会影响将该组用作其主组的人员。
* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员将其重新锁定，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
* 时间表会继承为时间表所有者的主组配置的时间表和小时首选项。

  <!--
  Add example here?
  -->

* Workfront管理员在系统级别解锁首选项并为您的组配置后，您随后可以锁定该首选项以确保您组下的每个用户都使用相同的配置。 此功能与Workfront管理员为系统中的每个人配置和锁定首选项的功能相同。 有关详细信息，请参阅[锁定或解锁组时间表和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)。

## 为组配置未锁定的时间表或小时首选项

>[!TIP]
>
>如果您是Workfront管理员，可以绕过步骤1-4，方法是转到设置>时间表和小时数>首选项，然后在页面顶部的框中搜索组的名称。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

1. 单击要配置其时间表或小时首选项的组的名称。
1. 在左侧面板中，单击&#x200B;**时间表和小时数**。

1. 在显示的页面上，在&#x200B;**常规首选项**&#x200B;部分中，配置以下任意选项：

   >[!TIP]
   >
   >如果将鼠标悬停在某个首选项上，并且会显示工具提示来告诉您该首选项已被锁定，则可以请求Workfront管理员为组织中的所有组解锁该首选项。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">记录未来日期的时间</td> 
      <td> <p>允许用户在整个系统中记录未来日期的时间，位置如下：</p> 
       <ul> 
       <li>他们有权记录时间的任何项目、任务和问题，而不管项目属于哪个组</li> 
       <li>他们的工时表作为常规时间</li>
       </ul> 
       <p>当用户计划离开办公室并希望提前记录时间时，这将很有用。</p> 
       <p><b>注意</b>：您无法阻止用户登录已关闭或已取消的任务或问题。 您只能阻止用户记录完成项目或停止项目的时间。 我们建议您在任务和问题列表中使用过滤器，以排除已完成或取消的任务和问题，以免用户看到它们。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">从时间表添加费用</td> 
      <td> <p>允许用户在时间表中记录时间和费用。</p> 
      <p>为某个组启用此首选项，并且该组被设置为某些用户的主组时，这些用户的时间表上的项目和任务旁边会显示一个费用图标。 用户可以单击此图标来添加或编辑项目或任务的费用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">手动将工作角色分配给小时条目</td> 
      <td> <p>允许用户手动选择在其用户配置文件中分配或分配给对象的任意工作角色。</p> <p><b>重要信息</b>：  
        <ul> 
         <li>如果在将工作角色分配给小时条目后禁用此设置，则用户必须在项目、任务或问题的小时选项卡上调整在各种角色下记录的小时数。</li> 
         <li>如果用户未在其配置文件中分配工作角色，并且在“高级分配”对话框中有任务被分配为任务所有者，则当用户登录该任务的时间时，将显示该工作角色。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制对所有者和管理员编辑的时间表</td> 
      <td> <p>限制对时间表所有者的编辑，而不考虑项目的组和Workfront管理员。 禁用此选项后，还可以通过以下方式编辑时间表：</p> 
       <ul> 
        <li> <p>对时间表和小时数的访问级别具有管理访问权限的用户</p> </li> 
        <li> <p>时间表批准者（如果在时间表上启用了“可以编辑小时数”）</p> </li> 
        <li> <p>时间表所有者的经理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制对所有者和管理员进行小时编辑</td> 
      <td>仅限编辑输入小时数的用户和Workfront管理员。 此设置适用于项目或小时报表中的小时选项卡。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**用户可以记录时间**&#x200B;部分中，配置以下任意选项：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">直接在项目上记录时间</td> 
      <td>允许用户在项目上记录时间（在更新选项卡和时间表上）。 如果要限制用户在项目级别记录时间，请取消选中此选项。</td>
     </tr>
     <tr>
      <td role="rowheader">在已完成的项目上记录时间</td>
      <td>允许用户在标记为完成的项目上记录时间。 如果禁用此选项，则用户无法记录他们在处于完成状态的项目上完成的工作的时间。</td>
     </tr>
     <tr>
      <td role="rowheader">在停止的项目上记录时间</td> 
      <td>启用此选项后，用户可以在处于非活动状态的项目上记录小时数。</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >此首选项根据用户主组首选项的配置应用。 如果在用户的主组首选项中启用了这些设置，则无论项目的组首选项是否允许，他们都将能够直接将时间记录到项目（包括已完成或停止的项目）上。

1. 在&#x200B;**预填充工时表**&#x200B;部分中，配置以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在时间表工作范围&lt;周数&gt;内的工作</td> 
      <td> <p>定义包含分配给用户的任务和问题日期的时间表日期范围之前和之后的周数。 默认设置为1周，您可以将此范围扩展到4周。 这意味着在为时间表日期范围选择4周后，在时间表日期范围之前的4周到时间表日期范围之后的4周之间的任何时间，都会预填充时间表的任务和问题。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已完成的任务和问题</td> 
      <td>如果通常将多个资源分配给单个任务，我们建议使用此设置。 这意味着当一个资源记录该任务的时间并将其标记为完成时，分配给该任务的其他资源仍然可以在其时间表中找到该任务或问题，以记录其小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划日期在时间表日期范围内的任务和问题</td> 
      <td> <p>选择后，时间表包括其计划开始日期或完成日期在时间表日期范围内的任务和问题。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 计划日期在工时表日期范围内的任务</td> 
      <td> <p>选择后，时间表包括其预计开始日期或完成日期在项目时间框架内的任务，即使问题或任务的计划日期在时间表日期范围外也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
