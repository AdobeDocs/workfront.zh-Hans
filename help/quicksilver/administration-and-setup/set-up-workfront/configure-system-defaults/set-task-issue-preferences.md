---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置系统范围的任务和问题首选项
description: 您可以为任务和问题配置系统范围的首选项。 这些首选项会影响用户在Workfront中创建任务和问题的方式。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '2238'
ht-degree: 0%

---

# 配置系统范围的任务和问题首选项

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


作为[!DNL Adobe Workfront]管理员，您可以为任务和问题配置系统范围的首选项。 这些首选项会影响用户在[!DNL Workfront]中创建任务和问题的方式。

默认情况下，任务和问题首选项处于锁定状态，组管理员无法在组级别修改它们，除非您为系统中的所有组解锁它们。 有关详细信息，请参阅本文中[锁定组](#lock-task-and-issue-preferences-for-groups)的任务和问题偏好设置。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td><p>新文档： [！UICONTROL Standard]</p>
   或
   <p>当前： [！UICONTROL计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

*有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为[!DNL Workfront]中的每个人配置任务和问题首选项

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 项目首选项]** >**[!UICONTROL 任务和问题].**

1. 在出现的页面上，继续下面列出的六部分之一，配置[!UICONTROL 新任务默认值]、[!UICONTROL 问题]、[!UICONTROL 删除]、[!UICONTROL 实际日期]和[!UICONTROL 访问]的设置：

   * [[!UICONTROL 新任务默认值]](#new-task-defaults)
   * [[!UICONTROL 问题]](#issues)
   * [[!UICONTROL 删除]](#deletion)
   * [移动](#move)
   * [[!UICONTROL 实际日期]](#actual-dates)
   * [[!UICONTROL 委派]](#delegation)
   * [[!UICONTROL 访问]](#access)


### [!UICONTROL 新任务默认值] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL开始日期]</td> 
    <td> <p>确定项目经理新任务的默认开始日期。 新任务的开始日期可以是项目的计划开始日期，也可以是创建任务的日期。</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[！UICONTROL持续时间类型] </p> </td> 
    <td> <p>确定资源数（及其分配百分比）与任务的持续时间或总工作量之间的关系。 有关详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL收入类型]</td> 
    <td> <p>计算任务的计划和实际收入预估。 当<strong>[！UICONTROL收入类型]</strong>设置为<strong>[！UICONTROL不可记帐]</strong>时，计划的小时数和记录的实际小时数不会为任务生成收入估计值，并且任务上的工作不会对项目级别的收入做出贡献。</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL成本类型]</td> 
    <td> <p>计算任务的计划成本和实际成本预估。 当设置为<strong>[！UICONTROL无成本]</strong>时，计划小时数和实际记录小时数不会为任务生成计划或实际成本预估，并且任务上的工作不会计入项目级别的成本。</p> </td> 
    </tr> 
  </tbody> 
</table>

### 问题 {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL当解析对象的状态更改时自动更新可解析问题状态]</td> 
    <td> <p>当有人将问题转换为项目或任务时，原始问题和转换的项目或任务都会成为解析对象。 此设置允许您将原始问题的解决方案与其可解析对象的解决方案相关联。 有关解析对象的详细信息，请参阅<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述</a>。</p> <p>要使此设置生效，必须选择<strong>[！UICONTROL保留原始问题并将其解决方案与任务绑定]</strong>选项。</p> 
      <ul> 
      <li>启用此设置后，您可以为问题和项目或任务创建具有相同键的自定义状态。 当项目或任务（作为可解析对象）变为自定义状态时，更改也会反映在问题的状态上。 问题和项目或任务状态的状态键必须相同。</li> 
      <li>禁用此设置时，解析对象状态会自动设置为默认状态，而不是自定义状态。 有关默认状态的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL将问题转化为任务时]</td> 
    <td> <p>此部分中的设置确定在从问题到任务的转换过程中发生的情况：</p> 
      <ul> 
      <li> <p><strong>[！UICONTROL保留原始问题并将其解决方案与任务绑定]</strong>：在转换问题时，在任务完成之前，它始终被视为问题。 任务完成后，问题的状态自动更改为[！UICONTROL Closed]。 取消选择后，问题将被删除。</p> <p><b>注释</b>：  <p>无权删除问题的用户将无法删除问题，因为他们正在转换问题，无论此设置的状态如何。 有关对问题的访问和权限的信息，请参阅：</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[！UICONTROL允许主要联系人访问任务]</strong>：授予主要联系人（问题创建者）查看任务的权限以审阅任务、随时了解其进度并在任务的“更新”部分添加注释。</li> 
      <li> <p><strong>[！UICONTROL允许在转换期间更改这些设置]</strong>：允许正在转换问题的用户在将问题转换为任务期间更改这些选项。</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL将问题转化为项目时]</td> 
    <td> <p>此部分中的设置确定在从问题到项目的转换过程中发生的情况：</p> 
      <ul> 
      <li> <p><strong>[！UICONTROL保留原始问题并将其解决方案与项目绑定]</strong>：在转换问题时，在项目完成之前，它始终作为问题可见。 项目完成后，问题的状态自动更改为[！UICONTROL Closed]。 取消选择后，问题将被删除。 </p> <p><b>注释</b>：  <p>无权删除问题的用户将无法删除问题，因为他们正在转换问题，无论此设置的状态如何。 有关对问题的访问和权限的信息，请参阅：</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[！UICONTROL允许主要联系人拥有对项目的访问权限]</strong>：授予主要联系人（问题创建者）对项目的查看权限以审阅项目、随时了解其进度并在项目的更新部分做出评论。</li> 
      <li><strong>[！UICONTROL允许在转化期间更改这些设置]</strong>：允许正在转化问题的用户在将问题转化为项目期间更改列出的选项。</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL 删除] {#deletion}

**[!UICONTROL 允许用户删除具有记录小时数的任务和问题]**：允许您确定是否允许删除记录了小时数的任务或问题。 默认情况下，该选项处于选中状态。

>[!TIP]
>
>此设置还适用于删除具有登录了小时数的任务或问题的项目。 此设置不适用于直接为项目记录时间的删除项目。

* 选择该选项后，您在删除任务或问题时收到信息性警告。 警告提醒您，如果任务或问题已记录小时数，则将它们移至项目或删除它们。 您可以在[!UICONTROL 设置]的[!UICONTROL 时间表和小时偏好设置]区域中配置小时数是已删除还是移动到项目。 确认看到警告后，任务或问题即被删除。 有关配置时间表和小时首选项的详细信息，请参阅[配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

  >[!TIP]
  >
  >当您删除包含已记录小时数的任务和问题的项目时，将删除已记录小时数，或根据[!UICONTROL 设置]的[!UICONTROL 时间表和小时数首选项]区域中的设置保留已记录小时数。 删除项目时未显示警告消息。

* 取消选择此选项时，当您删除具有记录小时数的任务或问题时，或者当您删除具有记录其任务或问题的小时数的项目时，会收到禁止性警告。 警告指定管理员不允许删除具有记录小时数的任务或问题。 无法删除为任务和问题记录小时数的任务、问题或项目。

### 移动

**[!UICONTROL 允许用户移动具有记录小时数的任务和问题]**：允许您确定是否允许将记录小时数的任务或问题移动到此处。 默认情况下，该选项处于选中状态。

* 选择该选项后，您可以移动已记录时间的任务和问题。 小时数也会随着任务或问题而移动。

* 取消选择此选项时，在将具有记录小时数的任务或问题移动到另一个项目时，您将收到禁止性警告。 警告指定管理员不允许移动具有记录小时数的任务或问题。 无法移动记录了小时数的任务或问题。 即使取消选择该选项，您也可以在同一项目中移动任务。

### [!UICONTROL 实际日期] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL当任务或问题从“新”转换为“进行中”时，将实际开始日期设置为]</td> 
    <td> <p>当任务或问题从<strong>[！UICONTROL新建]</strong>变为<strong>[！UICONTROL正在进行]</strong>时，为[!DNL Workfront]中记录实际开始日期选择以下选项之一：</p> 
      <ul> 
      <li><strong>[！UICONTROL现在]：</strong>实际开始日期设置为当前日期。</li> 
      <li><strong>[！UICONTROL计划开始日期]：</strong>实际开始日期设置为任务或问题的计划开始日期。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL完成任务或问题后，将实际完成日期设置为]</td> 
    <td> <p>当任务或问题完成时，为在[!DNL Workfront]中记录实际完成日期选择以下选项之一：</p> 
      <ul> 
      <li><strong>[！UICONTROL现在]：</strong>实际完成日期设置为当前日期。</li> 
      <li> <p><strong>[！UICONTROL计划完成日期]：</strong>实际完成日期设置为任务或问题的计划完成日期。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### 委派

启用&#x200B;**[!UICONTROL 允许用户委派他们的任务和问题]**&#x200B;设置允许系统中的所有用户将其工作暂时委派给其他人。

启用此设置后，用户可以看到以下内容：

* [!UICONTROL 主页]区域中的[!UICONTROL 我的工作]、[!UICONTROL 我的任务]或[!UICONTROL 我的问题]小组件中的&#x200B;[!UICONTROL **代理**]&#x200B;链接。 他们可以从此处委派任务和问题分配。

  >[!NOTE]
  >
  >  [!UICONTROL **委托审批**]&#x200B;链接始终在[!UICONTROL 主页]区域中启用。

* 指示任务或问题已委派给任务或问题标题中[!UICONTROL 任务和委派]区域中的另一个用户。
* 表示任务或问题已委派给位于[!UICONTROL 主页]中其[!UICONTROL 我的工作]小部件中的其他用户。

  如果禁用[!UICONTROL 允许用户委派其任务和问题]设置，则当前计划的委派将停止，并且委派的用户将收到一封电子邮件通知，告知委派已停止。

有关将工作委派给其他人的信息，请参阅以下文章：

* [委派工作概述](../../../manage-work/delegate-work/delegate-work-overview.md)
* [委派任务和问题](../../../manage-work/delegate-work/how-to-delegate-work.md)


<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL 访问] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL将某人分配给任务时]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他们……对任务的访问权限]</strong>：定义用户对其所分配任务的默认权限。 有关任务权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</li> 
      <li> <p><strong>[！UICONTROL同时授予他们……对项目的访问权限]</strong>：定义用户对其分配了任务的项目具有的默认权限。 有关项目权限的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL将某人分派到一个问题时]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他们……对任务的访问权限]</strong>：定义用户对其所分配任务的默认权限。 有关任务权限的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</li> 
      <li> <p><strong>[！UICONTROL同时授予他们……对项目的访问权限]</strong>：定义用户对其分配了任务的项目具有的默认权限。 有关项目权限的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL当有人提交请求时]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他们……对问题的访问权限]</strong>：定义用户对其提交的请求具有的默认权限。 有关详细信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a>。</li> 
      <li> <p><strong>[！UICONTROL来自同一公司的人员将为所有请求继承相同的权限]</strong>：允许用户查看由来自与他们相同的公司的其他用户提交的请求。 他们对这些请求具有与其自己提交的请求相同的权限。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 锁定组的任务和问题偏好设置 {#lock-task-and-issue-preferences-for-groups}

如果贵组织中的组需要为其独特工作流配置不同的任务或问题偏好设置，您可以解锁整个组织中所有组的偏好设置，以便他们能够自行配置。 当解锁首选项且组管理员修改它时，与组相关联的任务或问题受首选项的组级别设置而不是系统级别设置的影响。

有关组管理员如何配置组的任务和问题首选项的信息，请参阅[配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

>[!NOTE]
>
>在[!DNL Workfront]管理员在系统级别解锁首选项后，任何组管理员都可以对其进行配置并锁定它，以确保其组中的每个人和下面的子组都使用相同的配置。 此功能与[!DNL Workfront]管理员为系统中的每个人配置和锁定首选项的能力并行。 有关详细信息，请参阅[配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。

要锁定或解锁任务或问题首选项以便组可以对其进行配置，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 项目首选项]** > **[!UICONTROL 任务和问题]**。

1. 执行以下任一操作：

   * 如果您希望组下的组管理员能够为其组配置首选项，请将其解锁![解锁切换](assets/unlock-toggle-button.png)。
   * 如果您希望您的组及其下的所有组使用首选项的配置，请确保该组已锁定（这是默认设置）。

     >[!IMPORTANT]
     >
     >我们建议您与系统中的管理员和用户群组进行通信，以确保以配置锁定首选项的方式考虑所有需求。 锁定后，其配置将由系统中的所有组继承。 如果首选项已解锁任意时间段，则您的配置将替换组管理员可能已做出的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
