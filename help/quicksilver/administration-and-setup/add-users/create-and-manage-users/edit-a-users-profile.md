---
title: 编辑用户配置文件
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以创建新用户并管理现有用户的配置文件。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 72d0b8e0e190f774c7e3f14a78904fb1dd3f2b14
workflow-type: tm+mt
source-wordcount: '3403'
ht-degree: 0%

---

# 编辑用户配置文件

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

作为Adobe Workfront管理员，您可以创建用户并管理现有用户的配置文件。 有关创建用户的信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

有关用户更新其个人资料的信息，请参阅[配置我的设置](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 编辑用户配置文件

{{step-1-to-users}}

1. 选择用户，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

   此时将显示“编辑用户”框。

1. 在&#x200B;**编辑用户**&#x200B;框中，更改任何部分中的信息，然后随时单击&#x200B;**保存**。

### 个人信息

* **名字**
* **姓氏**

  >[!NOTE]
  >
  >在Workfront中编辑用户名不会在Adobe Admin Console中编辑用户名。

* **电子邮件地址**：用户的电子邮件地址也是他们在Workfront中的用户名。 此字段区分大小写，并且必须是唯一的。 如果任何用户尝试在10分钟窗口内添加非唯一电子邮件地址3次，则会显示reCAPTCHA响应。

  选择&#x200B;**我不是自动机**&#x200B;设置，然后才能继续。

  如果您使用电子邮件允许列表并输入不在列表中的电子邮件域，则用户不会收到电子邮件通知。 有关允许列表列入允许列表的详细信息，请参阅[配置电子邮件](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。

  如果贵组织已迁移到Adobe Admin Console，则无法在Workfront中编辑用户的电子邮件地址。 用户的电子邮件地址是在Adobe Admin Console中设置的。

* **更改密码**：单击此按钮可重置用户的密码。 在重置其他用户的密码之前，必须输入自己的密码。

  要重置其他用户的密码，您必须是Workfront管理员或组管理员。

  如果您是组管理员，则只能为您指定为管理员的组中的用户重置密码。 此外，必须在您的访问级别中启用“用户管理员（组用户）”权限：

  ![用户管理员访问级别设置](assets/group-admin-user.png)

  默认情况下禁用此设置。 有关详细信息，请参阅[创建或修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  您无法重置Workfront管理员的密码。

* **&lt;SSO配置>用户名**：如果您的Workfront管理员启用了与Workfront的SSO集成，则SSO用户名将显示在此字段中。 此字段将显示为您的Workfront实例启用的SSO配置类型。
* **OnlyAllow &lt;SSO Configuration>身份验证**：如果您的Workfront管理员启用了与Workfront的SSO集成，并更新了SSO的所有用户，则默认情况下会选择此字段。 此字段将显示为您的Workfront实例启用的SSO配置类型。

  如果选择此字段，用户需要使用其SSO凭据登录Workfront。 取消选中此项将允许他们使用其Workfront凭据登录Workfront。

  有关使用SSO解决方案配置Workfront的更多信息，请参阅[Adobe Workfront中的单点登录概述](/help/quicksilver/administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

  有关更新SSO用户的详细信息，请参阅[更新单点登录的用户](/help/quicksilver/administration-and-setup/add-users/single-sign-on/update-users-sso.md)。

  >[!NOTE]
  >
  >如果您是组管理员，则只能为您指定组的用户编辑&lt;SSO配置>字段。 此外，还必须在您的访问级别中启用“用户管理员（组用户）”权限。
  >
  >如果您是组管理员，并且在访问级别中启用了用户管理员（所有用户）权限，则可以编辑所有用户的&lt;SSO配置>字段。

* **个人资料照片**：单击&#x200B;**上传新照片**&#x200B;以加载用户的个人资料照片。 您可以上传JPG、GIF或PNG文件。 文件大小限制为4 MB。

  个人资料图片成为用户的头像，并且在整个Workfront系统中可见，无论在何处显示用户名。

* **工作信息**：有关该工作的信息，如职称（在&#x200B;**职称**&#x200B;字段中）以及用户负责哪方面的专业知识（在&#x200B;**与我谈关于**&#x200B;字段中）。
* **联系信息**：用户的电话号码(**电话号码**，**分机。**&#x200B;和&#x200B;**手机号码**&#x200B;字段)和地址（在&#x200B;**地址**、**城市**、**州**、**邮政编码**&#x200B;和&#x200B;**国家/地区**&#x200B;字段中）。

  如果用户启用了统一用户管理(UUM)或Adobe Identity Management System (IMS)，则联系人信息部分中的&#x200B;**国家/地区**&#x200B;字段仅接受国家/地区代码值（例如，US、GB、IN）。

### 首选项

* **时区**：用户的时区。

  有关帮助用户在Workfront中跨时区进行协作的信息，请参阅[跨时区工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

* **电子邮件区域设置**：用户首选的电子邮件区域设置。 这会影响从Workfront发往此用户的电子邮件中数字和日期的格式。

  >[!NOTE]
  >
  >当您的组织使用Adobe Unified Experience时，用户的语言首选项存储在其Adobe配置文件中，并且不使用电子邮件区域设置。 有关访问这些首选项的信息，请参阅[Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* **接收来自此测试环境的电子邮件**：如果要接收来自当前登录环境的电子邮件通知，请选中此选项。

  >[!NOTE]
  >
  >此选项仅在预览和沙盒环境中可用。 默认情况下，生产环境中启用了电子邮件通知。

* **当任务自行分配时，自动将任务状态设置为“进行中”**：选择此选项时，用户自行分配的工作将自动设置为“进行中”状态而不是“新建”。

* **上载文档时自动生成验证**：如果希望用户上载的文档立即生成验证，请选中此选项。

### 通知

选择应为新用户启用的电子邮件通知。

您可以选择即时通知和每日摘要通知。

有关详细信息，请参阅[为系统中的每个人配置事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

### 访问

* **用户处于活动状态**：启用此选项可指示用户处于活动状态。 活动用户使用Workfront许可证。 禁用字段会取消激活用户并阻止他们登录Workfront。

* **访问级别**：选择要分配给此用户的访问级别。

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

* **布局模板**：为用户选择布局模板。 此布局模板优先于分配给用户的主组、主团队或主角色的任何布局模板。 有关布局模板的分配优先级的详细信息，请参阅[创建和管理布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

  以下列表描述了在此字段中可用的模板列表如何取决于您的访问权限：

   * 作为Workfront管理员，您可以查看所有系统级和组级布局模板。
   * 作为组管理员，您可以查看系统级布局模板以及与您管理的组关联的模板。
   * 作为具有Standard或Plan许可证并有权编辑用户的用户，您只能看到系统级别的布局模板。

     有关组级布局模板的详细信息，请参阅[创建和修改组的布局模板](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

### 组织

* **公司**：用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中只显示有效的公司。 有关创建公司的信息，请参阅[创建和编辑公司](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。
* **报告给**：如果您为用户指定了公司，则还可以在此字段中指定该用户的直接经理。 用户只能有一个经理。 如果用户没有先与公司关联，则不会显示此字段。
* **直接下属**：如果您为用户指定了公司，则还可以指定该用户的直接下属。 一个用户可以有多个直接下属。 如果用户没有先与公司关联，则不会显示此字段。
* **主团队**：指定用户的主团队。 用户只能有一个主团队。 在分配布局模板或为分配给用户的任务和问题定义处理它按钮时，主团队非常重要。
* **其他团队**：用户可以属于多个团队。 用户可以在主页区域查看分配给其任何团队的工作项。
* **当前主组**：选择适当的组以分配用户。 这使用户能够访问与组共享的对象。 您还可以与用户的主组共享布局模板。

  这是必填字段。 每个用户都必须与主组关联。 如果未选择主组，则您的主组将被指定为新用户的主组。

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

* **设置停用日期**：如果要安排在特定日期和特定时间停用此用户，请单击此按钮。
* **停用日期**：停用用户的日期和时间。 有关安排用户停用的信息，请参阅[停用或重新激活用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)中的[安排用户停用](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
* **主要角色**：这是用户可以在Workfront中履行的主要工作角色。 分配给用户的每个任务和问题也会分配给此工作角色。 工作角色在资源管理中至关重要。 只有在您拥有管理用户访问权限的Standard或Plan许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅[授予用户访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

  列表中只显示活动工作角色。

* （视情况而定）如果您选择了&#x200B;**主要角色**，则会显示&#x200B;**FTE可用性百分比**&#x200B;字段。 指定将用户计划的时间百分比分配给此工作角色。 主角色的FTE可用性百分比的默认值为100%。
* **其他角色**：一个用户可以在Workfront中具有多个工作角色。 工作角色在资源管理中至关重要。 用户可以履行的工作角色数量没有限制。 但是，我们建议不要将一位用户分配给过多的工作角色，因为对于这些用户而言，资源管理可能变得过于复杂。

  列表中只显示活动工作角色。 有关工作角色的更多信息，请参阅[创建和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

  只有在您拥有管理用户访问权限的Standard或Plan许可证，或者您是Workfront管理员时，才能更新此字段。

  有关设置具有管理用户访问权限的用户的详细信息，请参阅[授予用户访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

* （视情况而定）如果您选择了一个或多个&#x200B;**其他角色**，则将为每个角色显示&#x200B;**FTE可用性百分比**&#x200B;字段。 指定将用户计划的时间百分比分配给每个工作角色。 其他角色的FTE可用性百分比的默认值为0%。

  如果其他角色的FTE可用性为0%，则它们不会显示在Resource Planner中，除非将用户分配给这些角色中的任务。

  ![用户角色和FTE](assets/user-roles-fte-2025.png)

  所有角色的所有&#x200B;**FTE可用性**&#x200B;百分比的总和必须等于100%。 每个FTE可用百分比计算资源规划者中每个用户的每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。

  Workfront会根据Workfront管理员在资源管理首选项中选择用于计算FTE的方法，计算用户的可用时间。

  有关计算用户可用性的信息，请参阅[计算资源规划者中用户和角色的小时和FTE的概述](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

  有关配置资源管理首选项的信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  <span class="preview">（可选）如果用户在项目期间的工作角色发生更改，则在财务计算中使用生效日期的工作角色分配。</span>

  <span class="preview">单击&#x200B;**按日期定义角色**，选择&#x200B;**主要角色**&#x200B;和&#x200B;**其他角色**，然后输入每个角色的分配百分比。 这些角色可以与现有角色（使用不同的百分比）相同，也可以是新角色。 选择这些角色生效时的“开始”日期。 这可以是未来的日期。 当最新的角色变为活动角色时，您可以单击&#x200B;**显示以前的角色**&#x200B;以查看以前的非活动角色。</span>

* **计划**：将计划与用户关联。 用户调度计算用户所分配任务的时间线。

  必须先创建计划，然后才能将其与用户关联。 有关创建计划的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  >[!NOTE]
  >
  >我们建议与用户关联的计划与用户的时区相匹配。

  >[!IMPORTANT]
  >
  >仅当&#x200B;**使用计算资源可用性**&#x200B;设置设置为&#x200B;**用户计划**&#x200B;时，Workfront才会使用用户的计划。 有关此设置如何影响用于资源管理的计划的信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **时间表配置文件**：将时间表配置文件与用户关联，以确保自动为用户生成时间表。

  在此字段中可用的配置文件列表取决于您的访问权限：

   * 作为Workfront管理员，您可以查看所有系统级别和所有组级别的时间表配置信息。
   * 作为组管理员，您可以查看系统级时间表配置文件，以及与您管理的组相关联的时间表配置文件。
   * 作为具有Standard或Plan许可证并有权编辑用户的用户，您只能看到系统级时间表配置文件。 有关组级时间表配置文件的详细信息，请参阅[创建、编辑和分配时间表配置文件](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **默认小时类型**：为用户选择默认小时类型。 这是用户记录时间时默认使用的小时类型。
* **可用小时类型**：选择用户应可用的小时类型。 这些小时类型在Workfront中用户可以记录时间的任意位置均可见。 用户只能看到在项目级别以及用户级别启用的小时类型。 有关用户可用的小时类型的详细信息，请参阅[定义小时类型和可用性](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)。
* **在**&#x200B;中记录时间：选择用户应在小时还是天中记录工作项的时间。 有关详细信息，请参阅[配置时间是以小时还是天数记录](/help/quicksilver/timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)。
* **FTE**：这是该用户的等效全职。 仅当系统级别的资源管理首选项设置为默认计划时，Workfront才使用此数字根据默认计划计算用户可用性。

  FTE表示用户可在工作上花费的时间。 这包括管理费用以及在项目工作上花费的时间。 例如，在会议或培训中花费的时间也包含在FTE中。

  FTE必须是最多为1的小数，并且不能为0。 例如，如果FTE值为0.5，且Workfront中的默认计划为40小时，则用户每周有20小时的空闲时间。

  该字段的默认值为1。

  计划例外、休息时间以及工作时间的值可能会影响用户的可用性。

  Workfront会根据设置区域中的资源管理首选项计算用户可用性。

  如果系统级别的资源管理首选项设置为用户调度，则此处指定的值将被忽略，并且会根据用户调度中指定的内容，将用户视为可用。

  有关详细信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  有关在Workfront中创建计划的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* **资源池**：将用户与资源池关联。 有关详细信息，请参阅[将资源池与用户关联](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)。
* **成本费率**：用户每小时的成本额。

  对于日期有效成本费率，请单击&#x200B;**添加费率**。 输入时间期的成本费率值，并根据需要分配起始日期和终止日期。 成本费率1没有起始日期，最后一个成本费率没有终止日期。

  某些日期会自动添加。 例如，如果成本费率1没有终止日期，并且您添加了“成本费率2”起始日期为2023年5月1日，则终止日期为2023年4月30日，这样成本费率1就不会出现任何差距。

* **记帐费率**：用户每小时的记帐金额。

  对于日期有效记帐费率，请单击&#x200B;**添加费率**。 输入时间期的开单费率值，并根据需要分配起始日期和终止日期。 记帐费率1没有开始日期，最后一个记帐费率没有结束日期。

  某些日期会自动添加。 例如，如果记帐费率1没有结束日期，而您添加了一个开始日期为2023年5月1日的秒数，则结束日期为2023年4月30日的秒数将添加到记帐费率1，因此不存在间隔。

  ![用户成本和记帐费率](assets/user-cost-billing-rates-2025.png)

### 自定义表单

将现有用户自定义表单与此用户关联。 您必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 您无权编辑的字段不会显示在单独的自定义表单中。

>[!NOTE]
>
>高级自定义表单功能(如外部查找字段和Workfront本地字段)仅在您于详细信息页面（而非“编辑用户”对话框）中打开用户记录时可用。 （在用户列表中，单击用户名以打开详细信息。）

有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 评论

键入要发送给用户的评论，并转到其用户配置文件的“更新”区域。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personal Info </td> 
      <td> 
       <ul> 
        <li><p><b>First Name</b></p></li>
        <li><p><b>Last Name</b></p><p><b>NOTE:</b></p><p>Editing a user's name in Workfront does not edit the user's name in the Adobe Admin Console.</p></li> 
        <li> <p><b>Email Address:</b> The email address for a user is also their username in Workfront. This field is case-sensitive and must be unique. If any user attempts to add a non-unique email address 3 times within a 10-minute window, a reCAPTCHA response appears.</p> <p> Select the <b>I am not a robot</b> setting before you can proceed.</p><p>If you use the email allowlist and enter an email domain not on the list, the user will not receive email notifications. For more information about the allowlist, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configure your email allowlist</a>.</p><p>If your organization has been migrated to the Adobe Admin Console, you cannot edit a user's email address in Workfront. The user's email address is set in the Adobe Admin Console. </li> 
        <li> <p><b>Reset Password</b>: Click this link to reset the user's password. You must enter your own password before you can reset another user's password.</p> <p>To reset another user's password, you must be a Workfront administrator, or a group administrator.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>If you are a group administrator, you can reset passwords only for users in the groups where you are designated as an administrator. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
           <li> <p>You cannot reset the password of a Workfront administrator.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Username</b>: If your Workfront administrator enabled an SSO integration with Workfront, the SSO Username displays in this field. The type of SSO configuration enabled for your Workfront instance is visible in this field. </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt; Authentication</b>: If your Workfront administrator enabled an SSO integration with Workfront and has updated all users for SSO, this field is selected by default. The type of SSO configuration enabled for your Workfront instance is visible in this field.</p> <p>When this field is selected, the user is required to log into Workfront with their SSO credentials. Unchecking it will allow them to log in to Workfront with their Workfront credentials.</p> <p>For more information about configuring Workfront with an SSO solution, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> If you are a group administrator, you can edit the &lt;SSO Configuration&gt; fields only for users in the groups where you are designated as such. Also, the User Admin (Group Users) permission must be enabled in your access level.
        <p>If you are a group administrator and you have the User Admin (All Users) permission enabled in your access level, you can edit the &lt;SSO Configuration&gt; fields for all users.</p> </li> 
        <li><b>Job Info:</b> Information about the job, like the job title (in the <b>Title</b> field), and what area of expertise the user is responsible for (in the <b>Talk to Me About</b> field).</li> 
        <li><p><b>Contact Info</b>: The user's phone number (in the <b>Phone number, Ext.</b>, and <b>Mobile number</b> fields) and address (in the <b>Address, City, State, Postal Code, Country</b> fields ).</p>
        <p>If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the <b>Country</b> field in the Contact Info section only accepts country code values (for example, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferences </td> 
      <td> 
       <ul> 
      <li> <p><b>Time Zone:</b> The user's time zone.</p> <p>For information about helping users collaborate in Workfront across time zones, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </li>

      <li><p><b>Email Locale</b>: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.</p>
      <p><b>NOTE:</b> When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li> 
      
      <li><b>Receive emails from this test environment</b>: Check this option if you want to receive email notifications from the environment that you are currently logged in.
      <p><b>NOTE</b></p>
      <p>This option is available only in the Preview and Sandbox environments. Email notifications are enabled in the Production environment by default. </p>
      </li> 
      
      </li> 
       <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       <li><b>Automatically generate proofs when uploading documents</b>: Check this option if you want the documents that the user uploads to immediately generate a proof. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Select the email notifications which should be enabled for the new user.</p> <p>You can select instant as well as daily digest notifications.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
      <li><b>Is Active:</b> Select this box to indicate that the user is active. Active users use a Workfront license. Clearing the box deactivates the user and prevents them from logging in to Workfront.</li> 
       <li> <p><b>Access Level:</b> Select the access level to assign to this user.</p> 
       <p>When you assign an access level to a user, you can assign a level equal to or lower than your own access level.</p>
       <p>For example, if your access level is Plan, you cannot assign the Administrator access level. However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level. </p>
       <p>For example, if you have a Plan license with no access to delete tasks, you cannot assign someone a Work license with access to delete tasks, although the Work license is lower than the Plan license. For more information, see  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> 
       <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month. </p><p>For more information on the new access model, see <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a>. </p><p>For information on decision limits, see <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Limited document and proof decision for non-paid users overview</a>.</p></li> 
       <li> <p><b>Layout Template</b>: Choose a Layout Template for the user. This Layout Template takes precedence over any Layout Template assigned to the user's Home Group, Home Team or Primary Role. For more information about the assignment priority of Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> <p><b>NOTE</b>:  <p>The following list describes how the list of templates you have available in this field depends on your access:</p> 
       <ul> 
       <li>As a Workfront administrator, you can see all system-level and group-level Layout Templates.</li> 
       <li>As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.</li> 
       <li>As a user with a Plan license and access to edit users, you can see only system-level Layout Templates.</li> 
       </ul> <p>For more information about group-level Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization </td> 
      <td> 
       <ul> 
      <li><b>Company</b>: The company of the user. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</li> 
      <li><b>Reports to:</b> If you specified a company for the user, you can also specify the direct manager of the user in this field. A user can have only one manager. This field does not display if the user is not associated with a company first. </li> 
      <li><b>Direct Reports:</b> If you specified a company for the user, you can also specify the direct reports of the user. A user can have multiple direct reports. This field does not display if the user is not associated with a company first.</li> 
      <li><b>Home Team</b>: Specify the home team for the user. Users can only have one home team. The Home Team is important when assigning a layout template or when defining the Work On It button for the tasks and issues assigned to the user. </li> 
      <li><b>Other Teams</b>: Users can belong to multiple teams. A user can view work items assigned to any of their teams in their Home area. </li> 
      <li> <p><b>Home Group:</b> Select an appropriate group to assign the user. This gives the user the ability to access objects that are shared with the group. You can also share layout templates with the user's Home Group.</p> <p>This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the new user's Home Group.</p> <p><b>NOTE</b>:</p> 
      <p> You can assign a group to a user only if one of the following is true:</p>
      <ul><li>you are a Workfront administrator</li>
      <li>you are the administrator of the group</li>
      <li>the group is public.</li></ul> 
      <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.</p> <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning </td> 
      <td> 
       <ul>
       <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.  

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user's capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 
      <li> <b>Schedule Deactivation</b>: Check this box if you want to schedule this user to be deactivated on a certain date and at a certain time. </li> 
       <li><b>Scheduled Deactivation Date</b>: The date and time on which the user becomes deactivated. For information about scheduling users for deactivation, see the <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that the user can fulfill in Workfront. Every task and issue that the user is assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Only active job roles display in the list. </p> </li> 
       <li>If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the user's schedule is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%. </li> 
       <li> <p><b>Other Roles</b>: A user can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.<p>Only active job roles display in the list. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. <br>For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the user's schedule is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>The sum of all <b>Percentages of FTE Availability</b> for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </p>
       <span class="preview"><p>(Optional) Date effective job role assignments are used in financial calculations if the user's job role changes during a project.</p><p>Click <b>Define roles by date</b>, select the <b>Primary Role</b> and <b>Other Roles</b>, and enter the allocation percentage for each role. The roles could be the same as the existing roles (using different percentages), or new roles. Select the <b>Start date</b> when these roles become active. This can be a future date. When the newest roles become active, you can click <b>Show previous roles</b> to see the previous, inactive roles.</p> </li></span>
       <li> <p><b>Schedule</b>: Associate a schedule with the user. The schedule of the user calculates the timeline of the tasks the user is assigned to.</p> <p>You must create a schedule before you can associate it with a user. For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>NOTE</b>: We recommend that the schedule you associate with the user matches the user's Time Zone.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the user to ensure that timesheets generate automatically for the user.</p> <p><b>NOTE</b>:  The list of profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.</li>
       <li>As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.</li>
       <li>As a user with a Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Create, edit, and assign timesheet profiles</a>.</li>
      </ul></p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the user. This is the hour type that is used by default when the user logs time.</li> 
       <li><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the user can log time. A user can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</li> 
       <li><b>Log Time in:</b> Select whether the user should log time on work items in hours or days. For more information, see <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure whether time is logged in hours or days</a>.</li>
       
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
      
      <li><b>Resource Pools</b>: Associate the user with Resource Pools. For more information, see <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</li> 
      
      <li><b>Cost Rate</b>: The amount of cost per hour for the user.
      <p>For date effective cost rates, click <strong>Add Rate</strong>. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.</p><p>Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.</p></li> 
      
      <li><b>Billing Rate</b>: The amount of billing per hour for the user.
      <p>For date effective billing rates, click <strong>Add Rate</strong>. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.</p><p> <img alt="User cost and billing rates" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td><p>Associate an existing user custom form with this user. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)</p> <p>For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Create a custom form</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comment</td> 
      <td>Type the comment you want to send to the users and to the Updates area of their user profiles.</td> 
     </tr> 
    </tbody> 
   </table>
-->
