---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 批量编辑用户配置文件
description: 作为Adobe Workfront管理员，您可以批量编辑用户帐户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 1a81c1becfc0866b92dbd1358af23671e5302266
workflow-type: tm+mt
source-wordcount: '2610'
ht-degree: 0%

---

# 批量编辑用户配置文件

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

您可以批量编辑用户帐户。 在批量编辑用户时，只有您专门选择的字段会更新为所有选定用户提供的相同信息。 您未选择的所有其他字段对于每个用户都将保持不变，即使每个用户各自的字段各不相同。

>[!NOTE]
>
>* 您无法批量编辑用户配置文件的“个人信息”部分，因为对于每个用户来说，该信息必须是唯一的。
>* 为确保数据的准确性和最佳性能，我们建议您一次性选择不超过2000个用户进行批量编辑。
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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p><p>或</p><p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 批量编辑用户帐户

{{step-1-to-users}}

1. 选择多个用户，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

1. 在&#x200B;**编辑用户**&#x200B;框中，更改任何部分中的信息，然后随时单击&#x200B;**保存**。

### 首选项

* **时区**：用户的时区。

  有关帮助用户在Workfront中跨时区进行协作的信息，请参阅[跨时区工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

* **电子邮件区域设置**：用户首选的电子邮件区域设置。 这会影响从Workfront发往此用户的电子邮件中数字和日期的格式。

  >[!NOTE]
  >
  >当您的组织使用Adobe Unified Experience时，用户的语言首选项存储在其Adobe配置文件中，并且不使用电子邮件区域设置。 有关访问这些首选项的信息，请参阅[Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

### 通知

选择应为用户启用的电子邮件通知。

您可以选择即时通知和每日摘要通知。 对于您选择的所有用户，所有每日摘要通知将在同一时间后发送。

有关详细信息，请参阅[为系统中的每个人配置事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

### 访问

* **用户处于活动状态**：启用此选项可指示用户处于活动状态。 活动用户使用Workfront许可证。 禁用字段将停用用户，并阻止他们登录Workfront。

* **访问级别**：选择要分配给这些用户的访问级别。 您选择的所有用户都将具有相同的访问级别。

  当用户分配访问级别时，您可以分配等于或低于您自己的访问级别的级别。 （例如，如果您的访问级别为“标准”，则不能分配“管理员”访问级别。）

  但是，如果Workfront管理员在访问级别上启用了非默认权限，而您的访问级别中未启用这些权限，则您不能分配默认低于您自己的访问级别的访问级别。

  例如，如果您拥有无权删除任务的Standard许可证，则不能向某人分配有权删除任务的Light许可证，尽管Light许可证低于Standard许可证。 有关详细信息，请参阅[创建或修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  有关访问级别的详细信息，请参阅[配置对Adobe Workfront的访问](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md)。

  >[!NOTE]
  >
  >如果您的组织使用新的访问模型（标准/轻量级/参与者），并且用户已达到其当月的决策限制，则您无法将“标准”或“轻量级”用户重新分配给“参与者”访问级别。
  >
  >有关新访问模型的详细信息，请参阅[新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。
  >
  >有关决策限制的信息，请参阅[非付费用户的有限文档和验证决策概述](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

* **布局模板**：为用户选择布局模板。 此布局模板优先于任何分配给其主组、主团队或主角色的布局模板。 有关布局模板的分配优先级的详细信息，请参阅[创建和管理布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

  以下列表描述了在此字段中可用的模板列表如何取决于您的访问权限：

   * 作为Workfront管理员，您可以查看所有系统级和组级布局模板。
   * 作为组管理员，您可以查看系统级布局模板以及与您管理的组关联的模板。
   * 作为具有Standard或Plan许可证并有权编辑用户的用户，您只能看到系统级别的布局模板。

     有关组级布局模板的详细信息，请参阅[创建和修改组的布局模板](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

### 组织

* **公司**：用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中只显示有效的公司。 有关创建公司的信息，请参阅[创建和编辑公司](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。
* **主团队**：指定用户的主团队。 用户只能有一个主团队。
* **其他团队**：用户可以属于多个团队。
* **当前主组**：选择适当的组以分配用户。 这使用户能够访问与组共享的对象。 您还可以与主组共享布局模板。

  这是必填字段。 每个用户都必须与主组关联。 如果未选择主组，则会将主组指定为主组。

  仅当以下任一情况为真时，才能将组分配给用户：

   * 您是Workfront管理员
   * 您是组的管理员
   * 该组为公开组

* **其他组**：用户可以属于多个组。 只有在您是Workfront管理员、组管理员或组为公共时，才能将组分配给用户。

  >[!IMPORTANT]
  >
  >将用户添加到100多个组可能会导致在加载组列表的Workfront的任何区域出现性能问题。

  有关公用组的详细信息，请参阅[创建组](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

  有关组的详细信息，请参阅[组概述](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md)。

### 资源规划

* **工作时间**：表示用户可用于实际工作的相当于全职(FTE)时间的百分比，不包括开销。 工作时间必须为最多为1的小数，不得为0。 例如，实际工作的20%可用性为0.2。

  该字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。

  系统使用此数字来计算用户是否可用于实际的项目相关工作。

  有关在Workfront中创建计划的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  安排例外和休息时间也可能会影响用户的容量。

  Workfront会根据设置区域中的资源管理首选项计算用户可用性。 有关详细信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  >[!TIP]
  >
  >将“工作时间”值设置为1，表示用户可用于其整个全职等效项目相关工作。

* **设置停用日期**：如果要安排在特定日期和特定时间停用这些用户，请单击此按钮。
* **停用日期**：停用用户的日期和时间。 有关安排用户停用的信息，请参阅[停用或重新激活用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)中的[安排用户停用](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
* **主要角色**：这是用户可以在Workfront中履行的主要工作角色。 分配给用户的每个任务和问题也会分配给此工作角色。 工作角色在资源管理中至关重要。 只有在您拥有管理用户访问权限的Standard或Plan许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅[授予用户访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

  列表中只显示活动工作角色。

* （视情况而定）如果您选择了&#x200B;**主要角色**，则会显示&#x200B;**FTE可用性百分比**&#x200B;字段。 指定将用户计划的时间百分比分配给此工作角色。 主角色的FTE可用性百分比的默认值为100%。
* **其他角色**：用户在Workfront中可以有多个工作角色。 工作角色在资源管理中至关重要。 用户可以履行的工作角色数量没有限制。 但是，我们建议不要将一位用户分配给过多的工作角色，因为对于这些用户而言，资源管理可能变得过于复杂。

  列表中只显示活动工作角色。 有关工作角色的更多信息，请参阅[创建和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

  只有在您拥有管理用户访问权限的Standard或Plan许可证，或者您是Workfront管理员时，才能更新此字段。

  有关设置具有管理用户访问权限的用户的详细信息，请参阅[授予用户访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

* （视情况而定）如果您选择了一个或多个&#x200B;**其他角色**，则将为每个角色显示&#x200B;**FTE可用性百分比**&#x200B;字段。 指定将用户计划的时间百分比分配给每个工作角色。 其他角色的FTE可用性百分比的默认值为0%。

  如果其他角色的FTE可用性为0%，则它们不会显示在Resource Planner中，除非将用户分配给这些角色中的任务。

  所有角色的所有&#x200B;**FTE可用性**&#x200B;百分比的总和必须等于100%。 每个FTE可用百分比计算资源规划者中每个用户的每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。

  Workfront会根据Workfront管理员在资源管理首选项中选择用于计算FTE的方法，计算用户的可用时间。

  有关计算用户可用性的信息，请参阅[计算资源规划者中用户和角色的小时和FTE的概述](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

  有关配置资源管理首选项的信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **计划**：将计划与用户关联。 用户调度计算用户所分配任务的时间线。

  必须先创建计划，然后才能将其与用户关联。 有关创建计划的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  >[!IMPORTANT]
  >
  >仅当&#x200B;**使用计算资源可用性**&#x200B;设置设置为&#x200B;**用户计划**&#x200B;时，Workfront才会使用用户的计划。 有关此设置如何影响用于资源管理的计划的信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **时间表配置文件**：将时间表配置文件与用户关联以确保时间表自动生成。

  在此字段中可用的配置文件列表取决于您的访问权限：

   * 作为Workfront管理员，您可以查看所有系统级别和所有组级别的时间表配置信息。
   * 作为组管理员，您可以查看系统级时间表配置文件，以及与您管理的组相关联的时间表配置文件。
   * 作为具有Standard或Plan许可证并有权编辑用户的用户，您只能看到系统级时间表配置文件。 有关组级时间表配置文件的详细信息，请参阅[创建、编辑和分配时间表配置文件](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **默认小时类型**：为用户选择默认小时类型。 这是用户记录时间时默认使用的小时类型。
* **可用小时类型**：选择用户应可用的小时类型。 这些小时类型在Workfront中用户可以记录时间的任意位置均可见。 用户只能看到在项目级别以及用户级别启用的小时类型。 有关用户可用的小时类型的详细信息，请参阅[定义小时类型和可用性](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)。
* **FTE**：这是用户的等效全职。 仅当系统级别的资源管理首选项设置为默认计划时，Workfront才使用此数字根据默认计划计算用户可用性。

  FTE表示用户可在工作上花费的时间。 这包括管理费用以及在项目工作上花费的时间。 例如，在会议或培训中花费的时间也包含在FTE中。

  FTE必须是最多为1的小数，并且不能为0。 例如，如果FTE值为0.5，且Workfront中的默认计划为40小时，则用户每周可工作20小时。

  该字段的默认值为1。

  计划例外、休息时间以及工作时间的值可能会影响用户的可用性。

  Workfront会根据设置区域中的资源管理首选项计算用户可用性。

  如果系统级别的资源管理首选项设置为用户调度，则此处指定的值将被忽略，并且会根据用户调度中指定的内容，将用户视为可用。

  有关详细信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  有关在Workfront中创建计划的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* **资源池**：将用户与资源池关联。

  >[!NOTE]
  >
  >只有所有选定用户通用的资源池才会显示在此字段中。 如果您选择的用户没有共享资源池，则此字段为空。 如果此字段为空，则在此处指定的资源池将覆盖其各自的资源池。

  有关资源池的详细信息，请参阅[将资源池与用户关联](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)。

* **成本费率**：用户每小时的成本额。

  对于日期有效成本费率，请单击&#x200B;**添加费率**。 输入时间期的成本费率值，并根据需要分配起始日期和终止日期。 成本费率1没有起始日期，最后一个成本费率没有终止日期。

  某些日期会自动添加。 例如，如果成本费率1没有终止日期，并且您添加了“成本费率2”起始日期为2023年5月1日，则终止日期为2023年4月30日，这样成本费率1就不会出现任何差距。

* **记帐费率**：用户每小时的记帐金额。

  对于日期有效记帐费率，请单击&#x200B;**添加费率**。 输入时间期的开单费率值，并根据需要分配起始日期和终止日期。 记帐费率1没有开始日期，最后一个记帐费率没有结束日期。

  某些日期会自动添加。 例如，如果记帐费率1没有结束日期，而您添加了一个开始日期为2023年5月1日的秒数，则结束日期为2023年4月30日的秒数将添加到记帐费率1，因此不存在间隔。

### 自定义表单

将现有用户自定义表单与用户关联。 您必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 您无权编辑的字段不会显示在单独的自定义表单中。

>[!NOTE]
>
>高级自定义表单功能(如外部查找字段和Workfront本地字段)仅在您于详细信息页面（而非“编辑用户”对话框）中打开用户记录时可用。 （在用户列表中，单击用户名以打开详细信息。）

您可以选择性地选择&#x200B;**重新计算自定义表达式**&#x200B;选项，以确保附加到所选用户的自定义表单中的所有已计算自定义字段都是最新的。

有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 评论

键入要发送给用户的评论以及用户配置文件的更新区域。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

