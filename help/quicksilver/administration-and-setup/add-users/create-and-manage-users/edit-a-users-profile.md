---
title: 编辑用户的配置文件
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以创建新用户并管理现有用户的配置文件。
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2557'
ht-degree: 0%

---

# 编辑用户的配置文件

<!--drafted for Work Time field: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

In the table below, under Resource Planning, add the "Work Time" field and update the "FTE" field:

<b><span class="preview">Work Time</span></b>: <span class="preview">Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</span> 

<span class="preview">The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.</span>  

<span class="preview">The system uses this number to calculate the availability of the user for actual, project-related work.</span> 

<span class="preview">For more information about creating schedules in Workfront, see Create a schedule.</span>

<span class="preview">Schedule exceptions and time off might also affect the user capacity. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)


***UPDATED FTE FIELD***

FTE: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. The FTE indicates the amount of time that the user can spend at work. This includes overhead, and  time that is not spent on project work, but on other type of work. For example, time that is spent in meetings, or training is also included in the FTE. 

The FTE must be a decimal number up to 1, and it cannot be 0. 
The field's default is 1.

For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

Schedule exceptions, time off might, <span class="preview">and the value of Work Time</span> may affect the amount of available hours or the FTE. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

For more information about creating schedules in Workfront, see Create a schedule. (*****INSERT LINK*****)
-->

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中编辑用户配置文件的说明，请参阅文章中的“编辑用户详细信息”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或联系Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员，您可以创建新用户并管理现有用户的配置文件。 有关创建用户的信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

具有计划许可证的用户也可以创建和管理用户。 有关编辑用户所需访问权限的信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

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
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 在配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 编辑用户配置文件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).
1. 选择用户，然后单击编辑图标 ![](assets/edit-icon.png).

1. 在 **编辑用户** 框中，更改以下任何信息，然后单击 **保存更改**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">个人信息 </td> 
      <td> 
       <ul> 
        <li><b>名字</b>, <b>姓氏</b></li> 
        <li> <p><b>电子邮件地址：</b> 用户的电子邮件地址也是他们在Workfront中的用户名。 此字段区分大小写，且必须唯一。 如果任何用户尝试在10分钟窗口内3次添加非唯一电子邮件地址，则会显示reCAPTCHA响应。</p> <p>如果您使用电子邮允许列表件并输入不在列表中的电子邮件域，则用户将不会收到电子邮件通知。 有关的更多信允许列表息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">配置电子邮件允许列表</a>.</p> </li> 
        <li> <p><b>重置密码</b>:单击此链接可重置用户的密码。 系统会要求您提供自己的密码，然后才能重置用户的密码。</p> <p>要重置其他用户的密码，您必须是Workfront管理员或组管理员。</p> <p><b>注释</b>:  
          <ul> 
           <li> <p>如果您是组管理员，则只能为在您被指定为的组中的用户重置密码。 此外，必须在您的访问级别启用用户管理员（群组用户）权限：</p> <p> <img src="assets/group-admin-user.png" > </p> <p>默认情况下，此设置处于禁用状态。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </li> 
           <li> <p>无法重置Workfront管理员的密码。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; 用户名</b>:如果您的Workfront管理员启用了与Workfront的SSO集成，则此字段中会显示SSO用户名。 此字段中显示为Workfront实例启用的SSO配置类型。 </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; 身份验证</b>:如果您的Workfront管理员启用了与Workfront的SSO集成，并更新了所有用户的SSO，则默认情况下会选中此字段。 此字段中显示为Workfront实例启用的SSO配置类型。</p> <p>选择此字段后，用户需要使用其SSO凭据登录Workfront。 取消选中该复选框将允许他们使用其Workfront凭据登录Workfront。</p> <p>有关使用SSO解决方案配置Workfront的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront中的单点登录概述</a></p> <p>有关更新用于SSO的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新用户以进行单点登录</a>.</p> <p><b>注意</b>:如果您是群组管理员，则可以编辑 &lt;sso configuration=""&gt; 字段。 此外，必须在您的访问级别启用用户管理员（群组用户）权限。
        <p>如果您是群组管理员，并且在访问级别中启用了用户管理员（所有用户）权限，则可以编辑 &lt;sso configuration=""&gt; 字段。</p> </li> 
        <li><b>作业信息：</b> 有关工作的信息，如工作职位以及用户负责的专业领域。</li> 
        <li><p><b>联系信息</b>:用户的电话号码和地址。</p>
        <p>如果用户启用了统一用户管理(UUM)或AdobeIdentity Management系统(IMS)，则 <b>国家/地区</b> “联系信息”部分中的字段仅接受国家/地区代码值（例如，US、GB、IN）。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">首选项 </td> 
      <td> 
       <ul> 
        <li> <p><b>时区：</b> 用户的时区。</p> <p>有关帮助用户跨时区在Workfront进行协作的信息，请参阅 <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨时区工作</a>.</p> </li> 
        <li><b>电子邮件区域设置</b>:用户首选的电子邮件区域设置。 这会影响来自Workfront的电子邮件中的数字和日期格式。</li> 
        <li><b>显示更新状态完成百分比</b>:如果要在此用户任务的“更新”区域内显示完成百分比栏，请勾选此选项。</li> 
        <li><b>将我分配给自己的工作发送到我的工作选项卡</b>:如果希望用户分配给自己的所有内容直接显示在“工作于”(Working On)选项卡上，请勾选此选项。 默认设置是在用户的“工作请求”选项卡上列出分配给用户的所有内容。</li> 
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
        <p>在为用户分配访问级别时，您可以分配等于或小于您自己的访问级别的级别。 （例如，如果您的访问级别是“计划员”，则您无法分配“管理员”访问级别。） 但是，如果Workfront管理员在访问级别上启用了非默认权限，而在您自己的访问级别上也未启用(通过“微调”设置，如 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>)。 </p> 
        <p>有关访问级别的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a>.</p> </li> 
        <li> <p><b>布局模板</b>:为用户选择布局模板。 此布局模板优先于分配给用户的主组、主组或主作业角色的任何布局模板。 有关布局模板分配优先级的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> <p><b>注释</b>:  <p>您在此字段中可用的模板列表取决于您的访问权限：</p> 
          <ul> 
           <li>作为Workfront管理员，您可以看到所有系统级别和组级别的布局模板。</li> 
           <li>作为组管理员，您可以看到系统级别的布局模板，以及与您管理的组关联的布局模板。</li> 
           <li>作为具有计划许可证且有权编辑用户的用户，您只能看到系统级别的布局模板。</li> 
          </ul> <p>有关组级别布局模板的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组织 </td> 
      <td> 
       <ul> 
      <li><b>公司</b>:用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中仅显示活动的公司。 有关创建公司的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">创建和编辑公司</a>.</li> 
      <li><b>报告对象：</b> 如果您为用户指定了公司，则还可以在此字段中指定用户的直接经理。 用户只能有一个管理器。</li> 
      <li><b>直接报表：</b> 如果您为用户指定了公司，则还可以指定用户的直接报表。 用户可以有多个直接报表。</li> 
      <li><b>主队</b>:为用户指定主团队。 用户只能有一个主团队。</li> 
      <li><b>其他团队</b>:用户可以属于多个团队。</li> 
      <li> <p><b>主页组：</b> 选择相应的组以分配用户。 这允许用户访问与组共享的对象。</p> <p>这是必填字段. 每个用户都必须与一个主组关联。 如果未选择一个，则会将您的组分配为新用户的主组。</p> <p><b>注意</b>:仅当您是Workfront管理员、组管理员或组为公用时，才能将组分配给用户。</p> </li> 
      <li> <p><b>其他组</b>:用户可以属于多个组。 仅当您是Workfront管理员、组管理员或组为公用时，才能将组分配给用户。</p> <p><b>重要信息</b>:将用户添加到100多个组可能会在加载组列表的Workfront的任何区域中导致性能问题。</p> <p>有关公共群组的更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建群组</a>.</p> <p>有关群组的更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群组概述</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源规划 </td> 
      <td> 
       <ul>
       <li><b>计划停用</b>:如果要计划在一段时间后停用此用户，请选中此框。 </li> 
       <li><b>计划停用日期</b>:用户在此日期之后被停用。 有关计划用户停用的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">计划用户停用</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</li> 
       <li> <p><b>主要角色</b>:这是用户可以在Workfront中履行的主要作业角色。 分配给用户的每项任务和问题也会分配给此作业角色。 作业角色在资源管理中是必不可少的。 仅当您具有具有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> <p>列表中仅显示活动作业角色。 </p> </li> 
       <li>如果您选择了 <b>主要角色</b>, <b>FTE可用性百分比</b> 字段。 指定将用户计划的时间百分比分配给此作业角色。 主角色的FTE可用性百分比的默认值为100%。 </li> 
       <li> <p><b>其他角色</b>:用户在Workfront中可以具有多个作业角色。 作业角色在资源管理中是必不可少的。 用户可以履行的作业角色数量没有限制。 但是，我们建议不要为一个用户分配过多的作业角色，因为对于这些用户而言，资源管理可能变得过于复杂。<p>列表中仅显示活动作业角色。 有关作业角色的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> <p>仅当您具有具有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 <br>有关设置具有管理用户访问权限的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
       <li> <p>（视情况而定）如果您选择了一个或多个 <b>其他角色</b>, <b>FTE可用性百分比</b> 字段。 指定将用户计划的时间百分比分配给每个作业角色。 其他角色的FTE可用性百分比的默认值为0%。</p> <p><b>注意</b>:如果其他角色具有0% FTE可用性，则它们不会显示在资源计划器中，除非将用户分配到这些角色中的任务。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story_png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>注释</b>: <p>所有 <b>FTE可用性百分比</b> 对于所有角色，必须等于100%。 每个FTE可用性百分比计算资源计划器中每个用户每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。</p> <p>用户的可用时间由Workfront计算，具体取决于Workfront管理员在“资源管理首选项”中选择的用于计算FTE的方法。</p> <p>有关计算用户可用性的信息，请参阅 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.</p> <p>有关配置资源管理首选项的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> </p> </li> 
       <li> <p><b>计划</b>:将计划与用户关联。 用户的计划将计算用户分配到的任务的时间轴。</p> <p>必须先创建计划，然后才能将其与用户关联。 有关创建计划的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p><b>注意</b>:我们建议您与用户关联的计划与用户的时区匹配。</p> </li> 
       <li> <p><b>时间表配置文件</b>:将工时单配置文件与用户关联，以确保为用户自动生成工时单。</p> <p><b>注意</b>:此字段中可用的用户档案列表取决于您的访问权限：
       <ul>
       <li>作为Workfront管理员，您可以查看所有系统级别和所有组级别的时间表配置文件。</li>
       <li>作为组管理员，您可以看到系统级别的时间表配置文件以及与您管理的组关联的时间表配置文件。</li>
       <li>作为具有计划许可证并有权编辑用户的用户，您只能看到系统级别的时间表配置文件。 有关组级别时间表配置文件的详细信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">创建、编辑和分配工时单配置文件</a>.</li>
      </ul></p> </li> 
       <li><b>默认小时类型</b>:为用户选择默认的小时类型。 这是用户记录时间时默认使用的小时类型。</li> 
       <li><b>可用小时类型</b>:选择用户应可用的小时类型。 这些小时类型在Workfront中的任意位置都可见，用户可以在其中记录时间。 用户只能查看在项目级别和用户级别启用的小时类型。 有关用户可使用的小时类型的更多信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定义工时单的工时类型和可用性</a>.</li> 
       <li><b>登录时间：</b> 选择用户是否应以小时或天为单位记录工作项的时间。 有关更多信息，请参阅 <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">配置时间是以小时还是天记录</a>.</li> 
       <li> <p><b>FTE</b>:仅当系统级别的“资源管理首选项”设置为 <b>默认计划</b>. 值必须为 <i>0</i> 或介于 <i>.1</i> 和 <i>1</i>.</p> <p>例如，如果FTE值为0.5，而默认计划为40小时，则用户每周可工作20小时。</p> <p>如果系统级别的“资源管理首选项”设置为 <b>用户的计划</b>，则此处指定的值将被忽略，用户将根据其计划中指定的内容被视为可用。 在这种情况下，资源计划员用户的FTE通过以下公式计算：</p> <p ><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><em><br></em> </p> <p>有关计算用户FTE的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.<br>有关在Workfront中创建计划的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p>计划例外和休息时间可能会影响计划小时数或FTE的数量。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>. </p> </li> 
        <li><b>资源池</b>:将用户与资源池关联。 有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">将资源池与用户关联 </a>.</li> 
        <li><b>每小时成本</b>:用户每小时的成本金额。 </li> 
        <li><b>每小时计费</b>:用户每小时的账单金额。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>将现有用户自定义表单与此用户关联。 必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论</td> 
      <td> <p>键入要发送给用户及其用户配置文件的Updates区域的评论。</p> </td> 
     </tr> 
    </tbody> 
   </table>
