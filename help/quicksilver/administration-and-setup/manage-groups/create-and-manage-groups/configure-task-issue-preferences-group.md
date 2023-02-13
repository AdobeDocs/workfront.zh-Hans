---
title: 为组配置任务和问题首选项
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 组，首选项，任务，问题，解锁
navigation-topic: create-and-manage-groups
description: 如果贵组织中的组需要配置任务或问题首选项，而与在系统级别配置任务或问题首选项不同，则Adobe Workfront管理员可以解锁该首选项。 然后，作为组管理员，您可以配置组的首选项，该首选项将影响与组关联的所有任务或问题。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 3%

---

# 为组配置任务和问题首选项

如果贵组织中的组需要配置任务或问题首选项，而与在系统级别配置任务或问题首选项不同，则Adobe Workfront管理员可以解锁该首选项。 然后，作为组管理员，您可以配置组的首选项，该首选项将影响与组关联的所有任务或问题。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

有关Workfront管理员如何解锁首选项的信息，请参阅 [锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>项目首选项也可以进行组级别配置。 有关信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员重新锁定它，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
>* 与项目关联的组的首选项集优先于为创建项目的用户的“主页组”设置的首选项集。
>* 某些组级别首选项会影响您为组创建的项目模板。 有关更多信息，请参阅 [从“组”区域查看、处理和创建组的模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 在文章中 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* 在Workfront管理员解锁系统级别的首选项后，您可以对其进行配置，然后将其锁定，以确保组及其子组中的每个人都使用相同的配置。 这与Workfront管理员必须为系统中的每个人配置和锁定首选项的功能平行。 有关更多信息，请参阅 [锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


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

## 为顶级组配置已解锁的任务和问题首选项

>[!TIP]
>
>如果您是Workfront管理员，则可以绕过步骤1-4，方法是转到设置>项目首选项>任务和问题，然后在页面顶部的框中搜索组名称。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要为其配置解锁任务和问题首选项的组名称。
1. 在显示的群组页面的左侧面板中，单击 **任务和问题首选项**.
1. 在显示的页面上，继续执行以下步骤所列的5个部分之一，以配置新任务默认值、问题、删除、实际日期和访问区域的设置，然后单击 **保存**.

   如果将鼠标悬停在锁图标上 ![](assets/lock-toggle-button-dimmed.png) 要获取您需要配置的首选项，并显示工具提示来告知您已锁定该首选项，您可以请求Workfront管理员为组织中的所有组解锁该首选项。

   解锁后，您和其他组管理员可以为自己的组分别配置该组件。 此外，您还可以将其锁定到组及组下的任何子组。

   * [新任务默认值](#new-task-defaults)
   * [问题](#issues)
   * [删除](#deletion)
   * [实际日期](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [访问权限](#access)

### 新任务默认值 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新任务的开始日期</td> 
      <td> <p>确定项目经理新任务的默认开始日期。 新任务的起始日期可以是项目的计划起始日期或创建任务的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>持续时间类型 </p> </td> 
      <td> <p>确定资源数量（及其分配百分比）与任务的持续时间或总工作量之间的关系。 有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>计算任务的计划收入和实际收入估计值。 当 <strong>收入类型</strong> 设置为<strong>不可计费</strong>，计划小时数和实际记录的小时数不会生成任务的收入估计值，并且任务的工作不会对项目级别的收入产生影响。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>计算任务的计划成本估计和实际成本估计。 当设置为 <strong>无成本</strong>，计划小时数和记录的实际小时数不会生成任务的计划成本或实际成本估计，并且任务的工作不会对项目层成本产生影响。</p> </td> 
     </tr> 
    </tbody> 
   </table>

### 问题 {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">当解析对象状态更改时，自动更新可解析问题状态</td> 
      <td> <p>当某人将问题转换为项目或任务时，原始问题和转换后的项目或任务都会成为解决对象。 此设置允许您将原始问题的解决方案与其可解析对象的解决方案相关联。 有关解析对象的详细信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> <p>要使此设置生效，请选择 <strong>保留原始问题，并将其解决办法与任务挂钩</strong> 必须被选中。</p> 
       <ul> 
        <li>启用此设置后，您可以使用相同的键创建自定义状态，以用于问题和项目或任务。 当项目或任务（作为可解析的对象）变为自定义状态时，更改也会反映问题的状态。 问题和项目或任务状态的状态键必须相同。</li> 
        <li>禁用此设置后，解析对象状态将自动设置为默认状态，而不是自定义状态。 有关默认状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将问题转换为任务时</td> 
      <td> <p>此部分中的设置可确定在从问题到任务的转换过程中所发生的情况：</p> 
       <ul> 
        <li><strong>保留原始问题，并将其解决办法与任务挂钩</strong>:在转换问题时，该问题在任务完成之前仍显示为问题。 任务完成后，问题的状态将自动更改为“已关闭”。</li> 
        <li><strong>允许主要联系人有权访问任务</strong>:授予主联系人（问题创建者）访问任务的权限，以审核任务、进行更新并随时了解其进度</li> 
        <li> <p><strong>允许在转换期间更改这些设置</strong>:允许转换问题的用户在将问题转换为任务期间更改这些选项。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将问题转换为项目时</td> 
      <td> <p>此部分中的设置可确定在从问题到项目的转换过程中所发生的情况：</p> 
       <ul> 
        <li><strong>保留原始问题并将其解决方案与项目绑定</strong>:在转换问题时，它会一直显示为问题，直到项目完成为止。 项目完成时，问题的状态会自动更改为“已关闭”。</li> 
        <li><strong>允许主要联系人有权访问项目</strong>:授予主要联系人（问题创建者）访问项目的权限，以审核项目、进行更新并随时了解其进度。</li> 
        <li><strong>允许在转换期间更改这些设置</strong>:允许转换问题的用户在将问题转换为项目期间更改列出的选项。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 删除 {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">允许用户删除有记录小时数的任务和问题</td> 
      <td> <p> 用于确定是否允许删除记录小时的任务或问题。 默认情况下，此选项处于选中状态。</p> 
       <div> 
        <p><b>笔尖</b>:此设置还适用于删除任务或项目在登录小时数时出现问题的项目。 此设置不适用于删除直接为项目记录时间的项目。 </p> 
        <p>请考虑以下事项：</p> 
        <ul> 
         <li> <p>选择该选项后，您会在删除任务或问题时收到一条信息性警告。 警告会提醒您，如果任务或问题已记录小时数，则它们将被移到项目或被删除。 您可以在“设置”的“时间表和小时首选项”区域中配置是否将小时删除或移动到项目。 确认您看到警告后，任务或问题将被删除。 有关配置工时单和工时首选项的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置工时单和工时首选项</a>. </p> <p>提示： <span>在删除项目时，如果项目的任务和问题已记录小时数，则记录的小时数会被删除，或者会根据“设置”的“时间表和小时数首选项”区域中的设置保留</span>. </p> </li> 
         <li><span>如果取消选择此选项，则在删除任务或已记录时间的问题时，或删除已记录时间的项目以执行其任务或问题时，您会收到禁止性警告</span> <span>.</span> 警告指定管理员不允许删除已记录小时的任务或问题。 任务、问题<span>，或已记录任务和问题的小时的项目</span> 无法删除。 </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### 实际日期 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">当任务或问题从“新”变为“进行中”时，将“实际开始日期”设置为</td> 
      <td> <p>选择以下选项之一，以便当任务或问题发生时，Workfront中记录实际开始日期 <strong>新建</strong> to <strong>正在进行</strong>:</p> 
       <ul> 
        <li><strong>现在：</strong> 实际开始日期设置为当前日期。</li> 
        <li><strong>计划的开始日期：</strong> 实际起始日期设置为任务或发放的计划起始日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成任务或问题后，将实际完成日期设置为</td> 
      <td> <p>选择以下选项之一，以便在任务或问题完成时将实际完成日期记录在Workfront中：</p> 
       <ul> 
        <li><strong>现在：</strong> 实际完成日期设置为当前日期。</li> 
        <li> <p><strong>计划完成日期：</strong> 实际完成日期设置为任务或发放的计划完成日期。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### 访问权限 {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">将某人分配到任务时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对任务的访问权限</strong>:定义用户对其分配给的任务的默认权限。 有关任务权限的更多信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> 授予用户访问权限</a>.</li> 
        <li> <p><strong>还授予他们……对项目的访问权限</strong>:定义用户对其分配了任务的项目的默认权限。 有关项目权限的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将某人分配到问题时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对任务的访问权限</strong>:定义用户对其分配给的任务的默认权限。 有关任务权限的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</li> 
        <li> <p><strong>还授予他们……对项目的访问权限</strong>:定义用户对其分配了任务的项目的默认权限。 有关项目权限的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">当某人提交请求时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对问题的访问权限</strong>:定义用户在提交请求时拥有的默认权限。 有关更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a>.</li> 
        <li> <p><strong>来自同一公司的人员将继承所有请求的相同权限</strong>:允许用户查看其他用户从与其相同的公司提交的请求。 他们对这些请求拥有与其自己提交的请求相同的权限。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
