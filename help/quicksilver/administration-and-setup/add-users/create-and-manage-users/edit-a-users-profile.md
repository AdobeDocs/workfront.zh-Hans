---
title: 编辑用户配置文件
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以创建新用户和管理现有用户的配置文件。
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '2739'
ht-degree: 0%

---

# 编辑用户配置文件


>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未登记到Admin Console的组织。 如果您的组织已载入到Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中编辑用户配置文件的说明，请参阅文章中的“编辑用户详细信息”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系Adobe Admin Console管理员。
>
>有关因贵组织是否已载入Adobe Admin Console而不同的过程列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，您可以创建新用户和管理现有用户的配置文件。 有关创建用户的信息，请参见 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

拥有计划许可证的用户还可以创建和管理用户。 有关编辑用户所需的访问权限的信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一条件：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 将访问级别中的设置配置为 <b>编辑</b> 访问，使用 <b>创建</b> 而且至少两者 <b>用户管理员</b> 下启用的选项 <b>微调您的设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>这两个选项中的一个，如果用户 <b>管理员（组用户）</b> 启用，您必须是用户所属的组的组管理员。</p> <p>欲知关于 <b>用户</b> 在访问级别中设置，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 编辑用户配置文件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **用户** ![](assets/users-icon-in-main-menu.png).
1. 选择用户，然后单击编辑图标 ![](assets/edit-icon.png).

1. 在 **编辑用户** 框，更改以下任何信息，然后单击 **保存更改**：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">个人信息 </td> 
      <td> 
       <ul> 
        <li><b>名字</b>， <b>姓氏</b></li> 
        <li> <p><b>电子邮件地址：</b> 用户的电子邮件地址也是他们在Workfront中的用户名。 此字段区分大小写，且必须是唯一的。 如果有任何用户在10分钟窗口内尝试添加非唯一电子邮件地址3次，则会显示reCAPTCHA响应。</p> <p>如果您使用电子邮件允许列表并输入不在列表中的电子邮件域，则用户不会收到电子邮件通知。 允许列表有关的详细信息，请参见 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">配置电子邮件允许列表</a>.</p> </li> 
        <li> <p><b>重置密码</b>：单击此链接可重置用户的密码。 在重置用户的密码之前，系统会要求您提供自己的密码。</p> <p>要重置其他用户的密码，您必须是Workfront管理员或组管理员。</p> <p><b>注释</b>:  
          <ul> 
           <li> <p>如果您是组管理员，则只能为您指定密码的组中的用户重置密码。 此外，还必须在您的访问级别中启用“用户管理员（组用户）”权限：</p> <p> <img src="assets/group-admin-user.png" > </p> <p>默认情况下，此设置处于禁用状态。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </li> 
           <li> <p>您无法重置Workfront管理员的密码。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; 用户名</b>：如果您的Workfront管理员启用了与Workfront的SSO集成，则SSO用户名将显示在此字段中。 此字段将显示为您的Workfront实例启用的SSO配置类型。 </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; 身份验证</b>：如果您的Workfront管理员启用了与Workfront的SSO集成，并更新了所有SSO用户，则默认情况下会选中此字段。 此字段将显示为您的Workfront实例启用的SSO配置类型。</p> <p>如果选择此字段，用户需要使用其SSO凭据登录Workfront。 取消选中此项将允许他们使用其Workfront凭据登录Workfront。</p> <p>有关使用SSO解决方案配置Workfront的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront中的单点登录概述</a></p> <p>有关更新SSO用户的详细信息，请参见 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新单点登录的用户</a>.</p> <p><b>注意</b>：如果您是组管理员，则可以编辑 &lt;sso configuration=""&gt; 仅为您指定组的用户字段。 此外，还必须在您的访问级别中启用“用户管理员”（组用户）权限。
        <p>如果您是组管理员，并且在您的访问级别中启用了用户管理员（所有用户）权限，则可以编辑 &lt;sso configuration=""&gt; 所有用户的字段。</p> </li> 
        <li><b>作业信息：</b> 有关工作的信息（如职称）以及用户负责的专业领域。</li> 
        <li><p><b>联系信息</b>：用户的电话号码和地址。</p>
        <p>如果用户已启用统一用户管理(UUM)或AdobeIdentity Management System (IMS)，则 <b>国家/地区</b> “联系人信息”部分中的字段仅接受国家/地区代码值（例如，US、GB、IN）。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">首选项 </td> 
      <td> 
       <ul> 
        <li> <p><b>时区：</b> 用户的时区。</p> <p>有关帮助用户在Workfront中跨时区进行协作的信息，请参阅 <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨时区工作</a>.</p> </li> 
        <li><b>电子邮件区域设置</b>：用户的首选电子邮件区域设置。 这会影响来自Workfront的电子邮件中数字和日期的格式。</li> 
        <li><b>显示更新状态的完成百分比</b>：如果您希望在此用户任务的“更新”区域中显示完成百分比栏，请选中此选项。</li> 
        <li><b>将我分配给自己的工作发送到我的“正在处理”选项卡</b>：如果您希望用户分配给自己的所有内容直接显示在“正在处理”选项卡上，请选中此选项。 默认设置是在“工作请求”选项卡上列出分配给用户的所有内容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td> <p>选择应为新用户启用的电子邮件通知。</p> <p>您可以选择即时通知和每日摘要通知。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">为系统中的每个人配置事件通知</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问权限</td> 
      <td> 
       <ul> 
      <li><b>处于活动状态：</b> 选中此框可指示用户处于活动状态。 活动用户使用Workfront许可证。 清除该框将停用用户。</li> 
       <li> <p><b>访问级别：</b> 选择要分配给此用户的访问级别。</p> 
       <p>为用户分配访问级别时，可以分配等于或低于您自己的访问级别的级别。 （例如，如果您的访问级别是“规划者”，则不能分配“管理员”访问级别。） 但是，如果Workfront管理员在访问级别上启用了非默认权限，而您的访问级别上未启用非默认权限，则您不能分配默认低于您自己的访问级别的访问级别（通过“微调”设置），如中所述 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>)。 </p> 
       <p>有关访问级别的详细信息，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a>.</p> </li> 
       <li> <p><b>布局模板</b>：为用户选择布局模板。 此布局模板优先于任何分配给用户主组、主团队或主要工作角色的布局模板。 有关布局模板的分配优先级的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> <p><b>注释</b>:  <p>在此字段中可用的模板列表取决于您的访问权限：</p> 
       <ul> 
       <li>作为Workfront管理员，您可以查看所有系统级和组级布局模板。</li> 
       <li>作为组管理员，您可以查看系统级布局模板以及与您管理的组相关联的模板。</li> 
       <li>作为拥有计划许可证并有权编辑用户的用户，您只能看到系统级别的布局模板。</li> 
       </ul> <p>有关组级布局模板的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组织 </td> 
      <td> 
       <ul> 
      <li><b>公司</b>：用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中只显示活跃的公司。 有关创建公司的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">创建和编辑公司</a>.</li> 
      <li><b>报告对象：</b> 如果您为用户指定了公司，则还可以在此字段中指定用户的直接经理。 一个用户只能有一个经理。</li> 
      <li><b>直接下属：</b> 如果您为用户指定了公司，则还可以指定用户的直接下属。 一个用户可以有多个直接下属。</li> 
      <li><b>主团队</b>：指定用户的主团队。 用户只能有一个主团队。</li> 
      <li><b>其他团队</b>：用户可以属于多个团队。</li> 
      <li> <p><b>主组：</b> 选择适当的组以分配用户。 这使用户能够访问与组共享的对象。</p> <p>这是必填字段. 每个用户都必须与主组关联。 如果您未选择主组，则您的组会被分配为新用户的主组。</p> <p><b>注意</b>：仅当您是Workfront管理员、组管理员或组为公共组时，才能将组分配给用户。</p> </li> 
      <li> <p><b>其他组</b>：用户可以属于多个组。 只有在您是Workfront管理员、组管理员或组是公共组的情况下，才能将组分配给用户。</p> <p><b>重要</b>：将用户添加到100多个组可能会导致在加载组列表的Workfront的任何区域出现性能问题。</p> <p>有关公共组的详细信息，请参见 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建组</a>.</p> <p>有关组的详细信息，请参见 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">组概述</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源规划 </td> 
      <td> 
       <ul>
       <li>
       <b>工作时间</b>：表示用户可用于实际工作的相当于全职(FTE)时间的百分比，不包括开销。 工作时间必须是最多为1的小数，不能为0。 例如，实际工作的20%可用性将是0.2。

   该字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。

   系统使用此数字来计算用户实际完成项目相关工作的可用性。

   有关在Workfront中创建调度的详细信息，请参见 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>.

   安排例外和休息时间也可能会影响用户容量。

   Workfront会根据“设置”区域中的“资源管理”首选项计算用户的可用性。 有关更多信息，请参阅 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.

   <b>笔尖</b>

   将工作时间的值设置为1表示用户可用于其整个全职等效项目相关工作。
   </li> 
      <li> <b>计划停用</b>：如果您希望计划在一段时间后停用此用户，请选中此框。 </li> 
       <li><b>计划的停用日期</b>：用户被停用后的日期。 有关安排用户停用的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">计划用户以停用</a> 在 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</li> 
       <li> <p><b>主要角色</b>：这是用户可以在Workfront中履行的主要工作角色。 分配了用户的每个任务和问题也分配了此工作角色。 工作角色在资源管理中至关重要。 只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> <p>列表中只显示活动工作角色。 </p> </li> 
       <li>如果您选择了 <b>主要角色</b>，则 <b>FTE可用性的百分比</b> 字段显示。 指定将用户计划的时间百分比分配给此工作角色。 主角色的FTE可用性百分比的默认值为100%。 </li> 
       <li> <p><b>其他角色</b>：一个用户可以在Workfront中具有多个工作角色。 工作角色在资源管理中至关重要。 用户可以履行多少工作角色没有限制。 但是，我们建议不要将一个用户分配给过多的工作角色，因为对于这些用户而言，资源管理可能变得过于复杂。<p>列表中只显示活动工作角色。 有关工作角色的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> <p>只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 <br>有关设置具有管理用户访问权限的用户的详细信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
       <li> <p>（视情况而定）如果您选择了一个或多个 <b>其他角色</b>，则 <b>FTE可用性的百分比</b> 每个角色都会显示字段。 指定将用户计划的时间百分比分配给每个工作角色。 其他角色的FTE可用性百分比的默认值为0%。</p> <p><b>注意</b>：如果其他角色的FTE可用性为0%，则它们不会显示在资源规划者中，除非将用户分配给这些角色中的任务。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>注释</b>: <p>全部的总和 <b>FTE可用性的百分比</b> 对于所有角色，必须等于100%。 每个FTE可用百分比计算资源规划者中每个用户的每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。</p> <p>Workfront会根据Workfront管理员在资源管理首选项中选择的用于计算FTE的方法，计算用户的可用时间。</p> <p>有关计算用户可用性的信息，请参见 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">计算资源规划者中用户和角色的小时数和FTE的概览</a>.</p> <p>有关配置资源管理首选项的信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> </p> </li> 
       <li> <p><b>计划</b>：将计划与用户关联。 用户的计划计算用户所分配任务的时间线。</p> <p>必须先创建计划，然后才能将其与用户关联。 有关创建调度的详细信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p><b>注意</b>：我们建议与用户关联的计划与用户的时区匹配。</p> </li> 
       <li> <p><b>周期性工时表</b>：将时间表配置文件与用户关联，以确保自动为用户生成时间表。</p> <p><b>注意</b>：您在此字段中可用的配置文件列表取决于您的访问权限：
       <ul>
       <li>作为Workfront管理员，您可以查看所有系统级别和所有组级别的时间表配置信息。</li>
       <li>作为组管理员，您可以查看系统级别的时间表配置信息，以及与您管理的组关联的配置信息。</li>
       <li>作为拥有计划许可证并有权编辑用户的用户，您只能看到系统级时间表配置文件。 有关组级时间表配置文件的详细信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">创建、编辑和分配时间表配置文件</a>.</li>
      </ul></p> </li> 
       <li><b>默认小时类型</b>：为用户选择默认小时类型。 这是用户记录时间时默认使用的小时类型。</li> 
       <li><b>可用小时类型</b>：选择用户应可用的小时类型。 这些小时类型在Workfront中用户可以记录时间的任意位置都可见。 用户只能查看在项目级别以及用户级别启用的小时类型。 有关用户可以使用的小时类型的更多信息，请参见 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定义工时表的小时类型和可用性</a>.</li> 
       <li><b>记录时间：</b> 选择用户是否应以小时或天为单位记录工作项的时间。 有关更多信息，请参阅 <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">配置时间是以小时还是天为单位记录</a>.</li>

   <li> <b>FTE</b>：这是用户的等效全职。 仅当系统级别的资源管理首选项设置为默认计划时，Workfront才使用此数字根据默认计划计算用户可用性。

   <p>FTE表示用户可在工作上花费的时间。 这包括管理费用以及在项目工作上花费的时间。 例如，在会议或培训中花费的时间也包含在FTE中。</p>

   FTE必须是最多为1的小数，并且不能为0。 例如，如果FTE值为0.5，且Workfront中的默认计划为40小时，则用户每周有20小时的空闲时间。

   该字段的默认值为1。

   计划例外情况、休息时间以及工作时间的值可能会影响用户的可用性。

   Workfront会根据“设置”区域中的“资源管理”首选项计算用户的可用性。

   如果系统级别的资源管理首选项设置为用户的调度，则此处指定的值将被忽略，并根据用户调度中指定的内容，将用户视为可用。

   有关更多信息，请参阅 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.

   有关在Workfront中创建调度的详细信息，请参见 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>.
   </li>

   <li><b>资源池</b>：将用户与资源池关联。 有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">将资源池与用户关联 </a>.</li> 
        <li><b>成本/小时</b>：用户每小时的成本。 </li> 
        <li><b>记帐/小时</b>：用户每小时的计费金额。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>将现有用户自定义表单与此用户关联。 您必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论</td> 
      <td> <p>键入要发送给用户及其用户配置文件更新区域的评论。</p> </td> 
     </tr> 
    </tbody> 
   </table>
