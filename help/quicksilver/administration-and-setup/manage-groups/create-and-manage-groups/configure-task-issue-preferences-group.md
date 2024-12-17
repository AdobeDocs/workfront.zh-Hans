---
title: 配置组的任务和问题首选项
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 组，首选项，任务，问题，解锁
navigation-topic: create-and-manage-groups
description: 如果贵组织中的组需要独立于系统级别配置任务或问题首选项的方式对其进行配置，Adobe Workfront管理员可以解锁首选项。 然后，作为组管理员，您可以为组配置首选项，这将影响与组关联的所有任务或问题。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1885'
ht-degree: 2%

---

# 配置组的任务和问题首选项

如果贵组织中的组需要独立于系统级别配置任务或问题首选项的方式对其进行配置，Adobe Workfront管理员可以解锁首选项。 然后，作为组管理员，您可以为组配置首选项，这将影响与组关联的所有任务或问题。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

有关Workfront管理员如何解锁首选项的信息，请参阅[锁定或解锁系统中所有组的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

>[!TIP]
>
>也可以对项目首选项进行组级别配置。 有关信息，请参阅[为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)。

>[!NOTE]
>
>* 通常，已解锁的首选项会无限期地保持解锁状态。 如果Workfront管理员将其重新锁定，则系统设置将再次生效，并且组管理员所做的首选项设置将丢失。
>* 为与项目关联的组设置的首选项优先于为创建项目的用户的主组设置的首选项。
>* 某些组级首选项会影响您为组创建的项目模板。 有关详细信息，请参阅文章[创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)中的“组”区域](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view)中的[查看、使用和创建组的模板。
>
>* Workfront管理员在系统级别解锁首选项后，您可以对其进行配置，然后将其锁定，以确保您的组及其子组中的每个人都使用相同的配置。 此功能与Workfront管理员为系统中的每个人配置和锁定首选项的功能相同。 有关详细信息，请参阅[锁定或解锁子组的项目、任务或问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为顶层组配置解锁的任务和问题偏好设置

>[!TIP]
>
>如果您是Workfront管理员，可以绕过步骤1-4，方法是转到设置>项目偏好设置>任务和问题，然后在页面顶部的框中搜索组的名称。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)。

1. 单击要为其配置解锁任务和问题首选项的组的名称。
1. 在显示的组页面上，在左侧面板中，单击&#x200B;**任务和问题偏好设置**。
1. 在显示的页面上，继续执行以下步骤所列5个部分之一，配置“新任务默认值”、“问题”、“删除”、“实际日期”和“访问”区域的设置，然后单击“保存”****。

   如果您将鼠标悬停在锁定图标![](assets/lock-toggle-button-dimmed.png)上需要配置的首选项，并显示工具提示以告知您已锁定，则可以要求Workfront管理员为组织中的所有组解锁该首选项。

   解锁后，您和其他组管理员可以单独为您自己的组配置它。 此外，您还可以为您的组和组下的任何子组锁定它。

   * [新任务默认值](#new-task-defaults)
   * [问题](#issues)
   * [删除](#deletion)

   <!--* <span class="preview">[Move](#move)</span>-->

   * [实际日期](#actual-dates)
   * [访问权限](#access)

### 新任务默认值 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新任务的开始日期</td> 
      <td> <p>确定项目经理新任务的默认开始日期。 新任务的开始日期可以是项目的计划开始日期，也可以是创建任务的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>持续时间类型 </p> </td> 
      <td> <p>确定资源数（及其分配百分比）与任务的持续时间或总工作量之间的关系。 有关详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型：文章索引</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>计算任务的计划和实际收入预估。 当<strong>收入类型</strong>设置为<strong>不可记帐</strong>时，计划小时数和实际记录小时数不会生成任务的收入估计值，并且任务上的工作不会计入项目级别的收入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>计算任务的计划成本和实际成本预估。 当设置为<strong>无成本</strong>时，计划小时数和实际记录小时数不会为任务生成计划或实际成本估计，并且任务上的工作不会计入项目级别的成本。</p> </td> 
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
      <td> <p>当有人将问题转换为项目或任务时，原始问题和转换的项目或任务都会成为解析对象。 此设置允许您将原始问题的解决方案与其可解析对象的解决方案相关联。 有关解析对象的详细信息，请参阅<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述</a>。</p> <p>要使此设置生效，必须选择<strong>保留原始问题并将其解决方案与任务绑定</strong>的选项。</p> 
       <ul> 
        <li>启用此设置后，您可以为问题和项目或任务创建具有相同键的自定义状态。 当项目或任务（作为可解析对象）变为自定义状态时，更改也会反映在问题的状态上。 问题和项目或任务状态的状态键必须相同。</li> 
        <li>禁用此设置时，解析对象状态会自动设置为默认状态，而不是自定义状态。 有关默认状态的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将问题转化为任务时</td> 
      <td> <p>此部分中的设置确定在从问题到任务的转换过程中发生的情况：</p> 
       <ul> 
        <li><strong>保留原始问题并将其解决方案与任务绑定</strong>：在转换问题时，在任务完成之前，它始终被视为问题。 任务完成后，问题的状态自动变为“已关闭”。</li> 
        <li><strong>允许主要联系人访问任务</strong>：授予主要联系人（问题创建者）访问任务的权限，以审阅任务、进行更新并随时了解其进度</li> 
        <li> <p><strong>允许在转换期间更改这些设置</strong>：允许正在转换问题的用户在将问题转换为任务期间更改这些选项。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将问题转化为项目时</td> 
      <td> <p>此部分中的设置确定在从问题到项目的转换过程中发生的情况：</p> 
       <ul> 
        <li><strong>保留原始问题并将其解决方案与项目绑定</strong>：在转换问题时，在项目完成之前，它始终显示为问题。 项目完成后，问题的状态自动变为“已关闭”。</li> 
        <li><strong>允许主要联系人访问项目</strong>：授予主要联系人（问题创建者）访问项目的权限，以便审阅项目、进行更新并随时了解项目的进度。</li> 
        <li><strong>允许在转换期间更改这些设置</strong>：允许正在转换问题的用户在将问题转换为项目期间更改列出的选项。</li> 
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
      <td> <p> 让您确定是否允许删除记录了小时数的任务或问题。 默认情况下，该选项处于选中状态。</p> 
       <div> 
        <p><b>提示</b>：此设置还适用于删除具有任务或登录有小时问题的项目。 此设置不适用于直接为项目记录时间的删除项目。 </p> 
        <p>请考虑以下事项：</p> 
        <ul> 
         <li> <p>选择该选项后，您在删除任务或问题时收到信息性警告。 警告提醒您，如果任务或问题已记录小时数，则将它们移至项目或删除它们。 您可以在“设置”的“时间表和小时首选项”区域中配置小时数是删除还是移动到项目。 确认看到警告后，任务或问题即被删除。 有关配置时间表和小时首选项的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置时间表和小时首选项</a>。 </p> <p>提示： <span>当您删除包含已记录小时数的任务和问题的项目时，将删除已记录小时数，或者根据设置程序</span>的“时间表和小时数首选项”区域中的设置保留已记录小时数。 </p> </li> 
         <li><span>取消选择此选项时，当您删除具有记录小时数的任务或问题时，或者当您删除具有记录其任务或问题的小时数的项目时，会收到禁止性警告</span> <span>。</span>警告指定管理员不允许删除具有记录小时数的任务或问题。 无法删除为任务和问题</span>记录小时数的任务、问题<span>或项目。 </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


<!-- *****also replace the & with "and" in the Deletion section

<div class="preview">

### Move

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Allow users to move tasks and issues with logged hours</td> 
      <td> <p> Lets you determine whether you allow the move of tasks or issues where hours are logged. This option is selected by default.</p> 
       <p>Consider the following:</p> 
        <ul> 
         <li> When it is selected, you can move tasks and issues that have time logged. The hours also move with the tasks or issues. </li>
      <li>When you deselect this option, you receive a prohibitive warning when you move a task or issue with logged hours. The warning specifies that the administrator does not allow for tasks or issues with logged hours to be moved. The tasks or issues that have hours logged cannot be moved. </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

</div>

-->

### 实际日期 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">当任务或问题从“新”转换为“进行中”时，将实际开始日期设置为</td> 
      <td> <p>当任务或问题从<strong>新建</strong>变为<strong>进行中</strong>时，为在Workfront中记录实际开始日期选择以下选项之一：</p> 
       <ul> 
        <li><strong>现在：</strong>实际开始日期设置为当前日期。</li> 
        <li><strong>计划开始日期：</strong>实际开始日期设置为任务或问题的计划开始日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成任务或问题后，将实际完成日期设置为</td> 
      <td> <p>完成任务或问题后，在Workfront中记录实际完成日期时，选择以下选项之一：</p> 
       <ul> 
        <li><strong>现在：</strong>实际完成日期设置为当前日期。</li> 
        <li> <p><strong>计划完成日期：</strong>实际完成日期设置为任务或问题的计划完成日期。</p> </li> 
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
      <td role="rowheader">将某人分派到一个任务时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对任务的访问权限</strong>：定义用户对其所分配任务的默认权限。 有关任务权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</li> 
        <li> <p><strong>同时授予他们……对项目的访问权限</strong>：定义用户对其分配了任务的项目的默认权限。 有关项目权限的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">将某人分派到一个问题时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对任务的访问权限</strong>：定义用户对其所分配任务的默认权限。 有关任务权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</li> 
        <li> <p><strong>同时授予他们……对项目的访问权限</strong>：定义用户对其分配了任务的项目的默认权限。 有关项目权限的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">当某人提交请求时</td> 
      <td> 
       <ul> 
        <li><strong>授予他们……对问题的访问权限</strong>：定义用户对其提交的请求具有的默认权限。 有关详细信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a>。</li> 
        <li> <p><strong>来自同一公司的人员将继承所有请求的相同权限</strong>：允许用户查看由来自他们所在公司的其他用户提交的请求。 他们对这些请求具有与其自己提交的请求相同的权限。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
