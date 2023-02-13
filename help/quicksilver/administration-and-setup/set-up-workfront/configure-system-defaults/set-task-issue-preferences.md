---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置系统范围的任务和问题首选项
description: 您可以为任务和问题配置全系统的首选项。 这些首选项会影响用户在Workfront中创建任务和问题的方式。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# 配置系统范围的任务和问题首选项

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

作为 [!DNL Adobe Workfront] 管理员，您可以为任务和问题配置系统范围的首选项。 这些首选项会影响用户在中创建任务和问题的方式 [!DNL Workfront].

默认情况下，任务和问题首选项会被锁定，组管理员无法在组级别修改它们，除非您为整个系统中的所有组解锁它们。 有关更多信息，请参阅 [锁定组的任务和问题首选项](#lock-task-and-issue-preferences-for-groups) 在本文中。

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

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
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 为 [!DNL Workfront]

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 项目首选项]** >**[!UICONTROL 任务和问题].**

1. 在显示的页面上，继续下面列出的5个部分之一，以配置 [!UICONTROL 新任务默认值], [!UICONTROL 问题], [!UICONTROL 删除], [!UICONTROL 实际日期]和 [!UICONTROL 访问].
1. 单击&#x200B;**[!UICONTROL 保存]**。

* [[!UICONTROL 新任务默认值]](#new-task-defaults)
* [[!UICONTROL 问题]](#issues)
* [[!UICONTROL 删除]](#deletion)
* [[!UICONTROL 实际日期]](#actual-dates)
* [[!UICONTROL 委派]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL 访问权限]](#access)

### [!UICONTROL 新任务默认值] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL新任务的开始日期]</td> 
   <td> <p>确定项目经理新任务的默认开始日期。 新任务的起始日期可以是项目的计划起始日期或创建任务的日期。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL持续时间类型] </p> </td> 
   <td> <p>确定资源数量（及其分配百分比）与任务的持续时间或总工作量之间的关系。 有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Revenue Type]</td> 
   <td> <p>计算任务的计划收入和实际收入估计值。 当 <strong>[!UICONTROL Revenue Type]</strong> 设置为<strong>[!UICONTROL不可计费]</strong>，计划小时数和实际记录的小时数不会生成任务的收入估计值，并且任务的工作不会对项目级别的收入产生影响。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本类型]</td> 
   <td> <p>计算任务的计划成本估计和实际成本估计。 当设置为 <strong>[!UICONTROL无成本]</strong>，计划小时数和记录的实际小时数不会生成任务的计划成本或实际成本估计，并且任务的工作不会对项目层成本产生影响。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 问题 {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL当“解决对象”的状态发生更改时，会自动更新“可解决的问题”状态]</td> 
   <td> <p>当某人将问题转换为项目或任务时，原始问题和转换后的项目或任务都会成为解决对象。 此设置允许您将原始问题的解决方案与其可解析对象的解决方案相关联。 有关解析对象的详细信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> <p>要使此设置生效，请选择 <strong>[!UICONTROL保留原始问题并将其解决方案与任务绑定]</strong> 必须被选中。</p> 
    <ul> 
     <li>启用此设置后，您可以使用相同的键创建自定义状态，以用于问题和项目或任务。 当项目或任务（作为可解析的对象）变为自定义状态时，更改也会反映问题的状态。 问题和项目或任务状态的状态键必须相同。</li> 
     <li>禁用此设置后，解析对象状态将自动设置为默认状态，而不是自定义状态。 有关默认状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>将问题转换为任务时]</td> 
   <td> <p>此部分中的设置可确定在从问题到任务的转换过程中所发生的情况：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL保留原始问题并将其解决方案与任务绑定]</strong>:在转换问题时，该问题在任务完成之前仍显示为问题。 任务完成后，问题的状态会自动更改为[!UICONTROL已关闭]。 取消选择此选项后，问题将被删除。</p> <p><b>注释</b>:  <p>无权访问或无权删除问题的用户将无法删除问题，因为无论此设置的状态如何，用户都将无法在转换问题时将其删除。 有关问题的访问权限和权限的信息，请参阅：</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL允许主要联系人有权访问任务]</strong>:授予主联系人（问题创建者）访问任务的权限，以审核任务、进行更新并随时了解其进度</li> 
     <li> <p><strong>[!UICONTROL允许在转换期间更改这些设置]</strong>:允许转换问题的用户在将问题转换为任务期间更改这些选项。</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL将问题转换为项目时]</td> 
   <td> <p>此部分中的设置可确定在从问题到项目的转换过程中所发生的情况：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL保留原始问题并将其解决方案绑定到项目]</strong>:在转换问题时，它会一直显示为问题，直到项目完成为止。 项目完成时，问题的状态会自动更改为[!UICONTROL已关闭]。 取消选择此选项后，问题将被删除。 </p> <p><b>注释</b>:  <p>无权访问或无权删除问题的用户将无法删除问题，因为无论此设置的状态如何，用户都将无法在转换问题时将其删除。 有关问题的访问权限和权限的信息，请参阅：</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL允许主要联系人有权访问项目]</strong>:授予主要联系人（问题创建者）访问项目的权限，以审核项目、进行更新并随时了解其进度。</li> 
     <li><strong>[!UICONTROL允许在转换期间更改这些设置]</strong>:允许转换问题的用户在将问题转换为项目期间更改列出的选项。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除] {#deletion}

**[!UICONTROL 允许用户删除已记录小时的任务和问题]**:用于确定是否允许删除记录小时的任务或问题。 默认情况下，此选项处于选中状态。

>[!TIP]
>
>此设置还适用于删除任务或项目在登录小时数时出现问题的项目。 此设置不适用于删除直接为项目记录时间的项目。

* 选择该选项后，您会在删除任务或问题时收到一条信息性警告。 警告会提醒您，如果任务或问题已记录小时数，则它们将被移到项目或被删除。 您可以在 [!UICONTROL 工时单和工时首选项] 区域 [!UICONTROL 设置]. 确认您看到警告后，任务或问题将被删除。 有关配置工时单和工时首选项的详细信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >删除项目时，如果项目的任务和问题已记录小时数，则系统会删除已记录的小时数，或者根据 [!UICONTROL 工时单和工时首选项] 面积 [!UICONTROL 设置]. 删除项目时，不会显示警告消息。

* 如果取消选择此选项，则在删除任务或已记录时间的问题时，或删除项目并记录其任务或问题的时间时，您会收到禁止性警告。 警告指定管理员不允许删除已记录小时的任务或问题。 无法删除已为任务和问题记录小时的任务、问题或项目。

### [!UICONTROL 实际日期] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL当任务或问题从“新”变为“进行中”时，将实际开始日期设置为]</td> 
   <td> <p>选择以下选项之一，即当实际开始日期记录在 [!DNL Workfront] 任务或问题从 <strong>[!UICONTROL新建]</strong> to <strong>[!UICONTROL正在进行]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 实际开始日期设置为当前日期。</li> 
     <li><strong>[!UICONTROL计划开始日期]:</strong> 实际起始日期设置为任务或发放的计划起始日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL完成任务或问题后，将实际完成日期设置为]</td> 
   <td> <p>选择以下选项之一，以便在 [!DNL Workfront] 任务或问题完成时：</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 实际完成日期设置为当前日期。</li> 
     <li> <p><strong>[!UICONTROL计划完成日期]:</strong> 实际完成日期设置为任务或发放的计划完成日期。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 委派

启用 [!UICONTROL 允许用户委派其任务和问题] 设置允许中的所有用户临时将其工作委派给其他用户。

启用此设置后，用户可以看到以下内容：

* 的 [!UICONTROL 委派] 链接 [!UICONTROL 主页] 的上界。 他们可以从此处委派批准或任务并发出分配。
* 表示任务或问题已委派给 [!UICONTROL 任务和代表团] 任务或问题标题中的区域。

如果禁用 [!UICONTROL 允许用户委派其任务和问题] 设置时，当前计划的委派将停止，且委派的用户将收到一封电子邮件通知，告知已停止委派。

有关将工作委派给他人的信息，请参阅以下文章：

* [委派工作概述](../../../manage-work/delegate-work/delegate-work-overview.md)
* [管理任务和问题委派](../../../manage-work/delegate-work/how-to-delegate-work.md)

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

### [!UICONTROL 访问权限] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL将某人分配到任务时]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL为他们……授予任务访问权限]</strong>:定义用户对其分配给的任务的默认权限。 有关任务权限的更多信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</li> 
     <li> <p><strong>[!UICONTROL还授予他们……对项目的访问权限]</strong>:定义用户对其分配了任务的项目的默认权限。 有关项目权限的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL当某人被分配到问题时]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL为他们……授予任务访问权限]</strong>:定义用户对其分配给的任务的默认权限。 有关任务权限的更多信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</li> 
     <li> <p><strong>[!UICONTROL还授予他们……对项目的访问权限]</strong>:定义用户对其分配了任务的项目的默认权限。 有关项目权限的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL当某人提交请求时]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL为他们……授予对问题的访问权限]</strong>:定义用户在提交请求时拥有的默认权限。 有关更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a>.</li> 
     <li> <p><strong>[!UICONTROL来自同一公司的人员将继承所有请求的相同权限]</strong>:允许用户查看其他用户从与其相同的公司提交的请求。 他们对这些请求拥有与其自己提交的请求相同的权限。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 锁定组的任务和问题首选项 {#lock-task-and-issue-preferences-for-groups}

如果组织中的组需要以不同方式为其独特工作流配置任务或问题首选项，则可以解锁组织中所有组的首选项，以便他们可以自行配置。 解锁首选项并由组管理员修改该首选项后，与组关联的任务或问题将受首选项的组级别设置（而不是系统级别设置）的影响。

有关组管理员如何为组配置任务和问题首选项的信息，请参阅 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>在 [!DNL Workfront] 管理员在系统级别解锁首选项，任何组管理员都可以对其进行配置，然后将其锁定，以确保其组和以下子组中的每个人都使用相同的配置。 这与 [!DNL Workfront] 管理员必须为系统中的每个人配置并锁定首选项。 有关更多信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

锁定或解锁任务或问题首选项，以便组可以对其进行配置

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 任务和问题]**.

1. 执行以下任一操作：

   * 如果您希望群组下的群组管理员能够为其群组配置首选项，请解锁该首选项 ![](assets/unlock-toggle-button.png).
   * 如果希望组及其下的所有组使用配置作为首选项，请确保该组已锁定（这是默认设置）。

      >[!IMPORTANT]
      >
      >我们建议您与整个系统中的管理员和组中的用户通信，以确保通过配置锁定首选项的方式满足所有需求。 锁定后，系统中的所有组都会继承您的配置。 如果该首选项已在任意时间段内解锁，则您的配置将替换组管理员可能已设置的配置。

1. 单击&#x200B;**[!UICONTROL 保存]**。
