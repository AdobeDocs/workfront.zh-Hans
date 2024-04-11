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
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '3334'
ht-degree: 0%

---

# 编辑用户配置文件

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

作为Adobe Workfront管理员，您可以创建用户并管理现有用户的配置文件。 有关创建用户的信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td> <p>新增：标准</p>
   或
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>. </p> </li> 
     <li> <p>此 <b>用户</b> 访问级别中配置为以下对象的对象： <b>编辑</b> 访问，使用 <b>创建</b> 以及以下两个中的至少一个 <b>用户管理员</b> 下启用的选项 <b>微调您的设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> 用户管理员 (所有用户)</li>
     <li>用户管理员（组用户）</li></ul>
     <p>如果  <b>用户管理员（组用户）</b> 启用，您必须是用户所属的组的组管理员才能编辑该用户。</p> 
     <p>欲知关于 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑用户配置文件

{{step-1-to-users}}

1. 选择用户，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

   此时将显示“编辑用户”框。

1. 在 **编辑用户** 框中，更改以下任何信息，然后单击 **保存更改** 随时：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">个人信息 </td> 
      <td> 
       <ul> 
        <li><p><b>名</b></p></li>
        <li><p><b>姓</b></p></li> 
        <li> <p><b>电子邮件地址：</b> 用户的电子邮件地址也是他们在Workfront中的用户名。 此字段区分大小写，并且必须是唯一的。 如果任何用户尝试在10分钟窗口内添加非唯一电子邮件地址3次，则会显示reCAPTCHA响应。</p> <p> 选择 <b>我不是机器人</b> 设置，然后才能继续。</p><p>如果您使用电子邮件允许列表并输入不在列表中的电子邮件域，则用户不会收到电子邮件通知。 有关允许列表的详细信息，请参见 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">配置电子邮件允许列表</a>.</p> </li> 
        <li> <p><b>重置密码</b>：单击此链接可重置用户的密码。 在重置其他用户的密码之前，必须输入自己的密码。</p> <p>要重置其他用户的密码，您必须是Workfront管理员或组管理员。</p> <p><b>注意</b>：  
          <ul> 
           <li> <p>如果您是组管理员，则只能为您指定为管理员的组中的用户重置密码。 此外，必须在您的访问级别中启用“用户管理员（组用户）”权限：</p> <p> <img src="assets/group-admin-user.png" > </p> <p>默认情况下禁用此设置。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </li> 
           <li> <p>您无法重置Workfront管理员的密码。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; 用户名</b>：如果您的Workfront管理员启用了与Workfront的SSO集成，则SSO用户名将显示在此字段中。 此字段将显示为您的Workfront实例启用的SSO配置类型。 </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; 身份验证</b>：如果您的Workfront管理员启用了与Workfront的SSO集成，并更新了用于SSO的所有用户，则默认情况下会选中此字段。 此字段将显示为您的Workfront实例启用的SSO配置类型。</p> <p>如果选择此字段，用户需要使用其SSO凭据登录Workfront。 取消选中此项将允许他们使用其Workfront凭据登录Workfront。</p> <p>有关使用SSO解决方案配置Workfront的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront中的单点登录概述</a></p> <p>有关为SSO更新用户的详细信息，请参见 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新单点登录的用户</a>.</p> 
        <p><b>注意</b>：</p> 
        <p> 如果您是组管理员，则可以编辑 &lt;sso configuration=""&gt; 仅为您指定组的用户字段。 此外，还必须在您的访问级别中启用“用户管理员（组用户）”权限。
        <p>如果您是组管理员，并且您的访问级别中启用了用户管理员（所有用户）权限，则可以编辑 &lt;sso configuration=""&gt; 所有用户的字段。</p> </li> 
        <li><b>作业信息：</b> 有关作业的信息，如职务(在 <b>标题</b> 字段)，以及用户负责哪个专业领域(在 <b>和我谈及</b> 字段)。</li> 
        <li><p><b>联系信息</b>：用户的电话号码(在 <b>电话号码，分机</b>、和 <b>手机号码</b> 字段)和地址(在 <b>地址、城市、州/省、邮政编码、国家/地区</b> 字段)。</p>
        <p>如果用户已启用统一用户管理(UUM)或AdobeIdentity Management System (IMS)，则 <b>国家/地区</b> 联系人信息部分中的字段仅接受国家/地区代码值（例如，US、GB、IN）。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">首选项 </td> 
      <td> 
       <ul> 
      <li> <p><b>时区：</b> 用户的时区。</p> <p>有关帮助用户在Workfront中跨时区进行协作的信息，请参阅 <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨时区工作</a>.</p> </li> 
       <li><b>电子邮件区域设置</b>：用户的首选电子邮件区域设置。 这会影响从Workfront发往此用户的电子邮件中数字和日期的格式。</li>

   <li><b>接收来自此测试环境的电子邮件</b>：如果您希望从当前登录的环境接收电子邮件通知，请选中此选项。
      <p><b>注释</b></p>
      <p>此选项仅在预览和沙盒环境中可用。 默认情况下，生产环境中启用了电子邮件通知。 </p>
      </li>

   <li><b>显示更新状态的完成百分比</b>：如果您希望在使用旧版评论体验时在此用户任务的更新区域中显示完成百分比栏，请选中此选项。 有关信息，请参阅 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新的评论体验</a>.
      <p><span class="preview">此选项已从“预览”环境中删除。</span></p>

   </li> 
       <li><b>将我分配给自己的工作发送到我的工作选项卡中</b>：如果您希望用户分配给自己的所有内容直接显示在“主页”区域的“处理中”列表中，请选中此选项。 默认情况下，在“主页”区域的“准备开始”或“未就绪”列表中列出分配给用户的所有内容。</li> 
       <li><b>上传文档时自动生成验证</b>：如果您希望用户上传的文档立即生成验证，请选中此选项。 </li>
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
      <li><b>处于活动状态：</b> 选中此框可指示用户处于活动状态。 活动用户使用Workfront许可证。 清除该框将停用用户并阻止他们登录Workfront。</li> 
       <li> <p><b>访问级别：</b> 选择要分配给此用户的访问级别。</p> 
       <p>当用户分配访问级别时，您可以分配等于或低于您自己的访问级别的级别。</p>
       <p>例如，如果您的访问级别是“计划”，则不能分配“管理员”访问级别。 但是，如果Workfront管理员在访问级别上启用了非默认权限，而您的访问级别中未启用这些权限，则您不能分配默认低于您自己的访问级别的访问级别。 </p>
       <p>例如，如果您拥有无权删除任务的“计划”许可证，则不能向某人分配有权删除任务的“工作”许可证，尽管“工作”许可证低于“计划”许可证。 有关更多信息，请参阅  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> 
       <p>有关访问级别的详细信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a>.</p>
       <p> <b>注意：</b></p> 
       <p> 如果您的组织使用新的访问模型（标准/轻量级/参与者），并且用户已达到其当月的决策限制，则您无法将“标准”或“轻量级”用户重新分配给“参与者”访问级别。 </p><p>有关新访问模型的更多信息，请参阅 <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">新访问级别概述</a>. </p><p>有关决策限制的信息，请参阅 <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">非付费用户的有限文档和验证决策概述</a>.</p></li> 
       <li> <p><b>布局模板</b>：为用户选择布局模板。 此布局模板优先于分配给用户主组、主团队或主角色的任何布局模板。 有关布局模板分配优先级的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> <p><b>注意</b>：  <p>以下列表描述了在此字段中可用的模板列表如何取决于您的访问权限：</p> 
       <ul> 
       <li>作为Workfront管理员，您可以查看所有系统级和组级布局模板。</li> 
       <li>作为组管理员，您可以查看系统级布局模板以及与您管理的组关联的模板。</li> 
       <li>作为拥有计划许可证并有权编辑用户的用户，您只能看到系统级别的布局模板。</li> 
       </ul> <p>有关组级布局模板的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组织 </td> 
      <td> 
       <ul> 
      <li><b>公司</b>：用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中只显示有效的公司。 有关创建公司的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">创建和编辑公司</a>.</li> 
      <li><b>报告给：</b> 如果您为用户指定了公司，则还可以在此字段中指定用户的直接经理。 用户只能有一个经理。 如果用户没有先与公司关联，则不会显示此字段。 </li> 
      <li><b>直接下属：</b> 如果您为用户指定了公司，则还可以指定用户的直接下属。 一个用户可以有多个直接下属。 如果用户没有先与公司关联，则不会显示此字段。</li> 
      <li><b>主团队</b>：指定用户的主团队。 用户只能有一个主团队。 在分配布局模板或为分配给用户的任务和问题定义处理它按钮时，主团队非常重要。 </li> 
      <li><b>其他团队</b>：用户可以属于多个团队。 用户可以在主页区域查看分配给其任何团队的工作项。 </li> 
      <li> <p><b>主组：</b> 选择适当的组以分配用户。 这使用户能够访问与组共享的对象。 您还可以与用户的主组共享布局模板。</p> <p>这是必填字段。 每个用户都必须与主组关联。 如果未选择主组，则您的组将被分配为新用户的主组。</p> <p><b>注意</b>：</p> 
      <p> 仅当以下任一情况为真时，才能将组分配给用户：</p>
      <ul><li>您是Workfront管理员</li>
      <li>您是组的管理员</li>
      <li>该团体是公开的。</li></ul> 
      <li> <p><b>其他组</b>：用户可以属于多个组。 只有在您是Workfront管理员、组管理员或组为公共时，才能将组分配给用户。</p> <p><b>重要</b>：</p> 
      <p>将用户添加到100多个组可能会导致在加载组列表的Workfront的任何区域出现性能问题。</p> <p>有关公共组的详细信息，请参见 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建组</a>.</p> <p>有关组的详细信息，请参见 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">组概述</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源规划 </td> 
      <td> 
       <ul>
       <li>
       <b>工作时间</b>：表示用户可用于实际工作（不包括开销）的等效全职(FTE)时间百分比。 工作时间必须为最多为1的小数，不得为0。 例如，实际工作的20%可用性为0.2。

   该字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。

   系统使用此数字来计算用户是否可用于实际的项目相关工作。

   有关在Workfront中创建时间表的详细信息，请参阅 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>.

   安排例外和休息时间也可能会影响用户的容量。

   Workfront会根据设置区域中的资源管理首选项计算用户可用性。 有关更多信息，请参阅 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.

   <b>提示</b>

   将“工作时间”值设置为1，表示用户可用于其整个全职等效项目相关工作。
   </li> 
      <li> <b>计划停用</b>：如果要安排在特定日期和特定时间停用此用户，请选中此框。 </li> 
       <li><b>计划的停用日期</b>：用户被取消激活的日期和时间。 有关安排用户停用的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">安排用户停用</a> 在 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</li> 
       <li> <p><b>主要角色</b>：这是用户可以在Workfront中履行的主要工作角色。 分配给用户的每个任务和问题也会分配给此工作角色。 工作角色在资源管理中至关重要。 只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> <p>列表中只显示活动工作角色。 </p> </li> 
       <li>如果您选择了 <b>主要角色</b>， <b>FTE可用性的百分比</b> 字段显示。 指定将用户计划的时间百分比分配给此工作角色。 主角色的FTE可用性百分比的默认值为100%。 </li> 
       <li> <p><b>其他角色</b>：一个用户可以在Workfront中具有多个工作角色。 工作角色在资源管理中至关重要。 用户可以履行的工作角色数量没有限制。 但是，我们建议不要将一位用户分配给过多的工作角色，因为对于这些用户而言，资源管理可能变得过于复杂。<p>列表中只显示活动工作角色。 有关工作角色的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> <p>只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 <br>有关设置具有管理用户访问权限的用户的详细信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
       <li> <p>（视情况而定）如果您选择了一个或多个 <b>其他角色</b>， <b>FTE可用性的百分比</b> 字段将为每个角色显示。 指定将用户计划的时间百分比分配给每个工作角色。 其他角色的FTE可用性百分比的默认值为0%。</p> <p><b>注意</b>：如果其他角色的FTE可用性为0%，则它们不会显示在资源规划者中，除非将用户分配给这些角色中的任务。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>注意</b>： <p>全部的总和 <b>占FTE可用性的百分比</b> 所有角色的均必须等于100%。 每个FTE可用百分比计算资源规划者中每个用户的每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。</p> <p>Workfront会根据Workfront管理员在资源管理首选项中选择用于计算FTE的方法，计算用户的可用时间。</p> <p>有关计算用户可用性的信息，请参见 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">计算资源规划者中用户和角色的小时数和FTE的概述</a>.</p> <p>有关配置资源管理首选项的信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> </p>
       <span class="preview"><p>（可选）如果用户在项目期间的工作角色发生更改，则在财务计算中使用有效工作角色分配的日期。</p><p>单击 <b>按日期定义角色</b>，选择 <b>主要角色</b> 和 <b>其他角色</b>，并输入每个角色的分配百分比。 这些角色可以与现有角色（使用不同的百分比）相同，也可以是新角色。 选择 <b>开始日期</b> 这些角色生效时。 这可以是未来的日期。 当最新的角色变为活动角色时，您可以单击 <b>显示以前的角色</b> 查看以前的非活动角色。</p> </li></span>
       <li> <p><b>计划</b>：将计划与用户关联。 用户调度计算用户所分配任务的时间线。</p> <p>必须先创建计划，然后才能将其与用户关联。 有关创建调度的详细信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p><b>注意</b>：我们建议与用户关联的计划与用户的时区匹配。</p> </li> 
       <li> <p><b>周期性工时表</b>：将时间表配置文件与用户关联，以确保自动为用户生成时间表。</p> <p><b>注意</b>：在此字段中可用的配置文件列表取决于您的访问权限：
       <ul>
       <li>作为Workfront管理员，您可以查看所有系统级别和所有组级别的时间表配置信息。</li>
       <li>作为组管理员，您可以查看系统级时间表配置文件，以及与您管理的组相关联的时间表配置文件。</li>
       <li>作为拥有计划许可证并有权编辑用户的用户，您只能看到系统级时间表配置文件。 有关组级时间表配置文件的详细信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">创建、编辑和分配时间表配置文件</a>.</li>
      </ul></p> </li> 
       <li><b>默认小时类型</b>：为用户选择默认的小时类型。 这是用户记录时间时默认使用的小时类型。</li> 
       <li><b>可用小时类型</b>：选择用户应该可用的小时类型。 这些小时类型在Workfront中用户可以记录时间的任意位置均可见。 用户只能看到在项目级别以及用户级别启用的小时类型。 有关用户可以使用的小时类型的更多信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定义工时表的小时类型和可用性</a>.</li> 
       <li><b>记录时间：</b> 选择用户是否应以小时或天为单位记录工作项的时间。 有关更多信息，请参阅 <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">配置时间是以小时还是天为单位记录</a>.</li>

   <li> <b>FTE</b>：这是用户的等效全职。 仅当系统级别的资源管理首选项设置为默认计划时，Workfront才使用此数字根据默认计划计算用户可用性。

   <p>FTE表示用户可在工作上花费的时间。 这包括管理费用以及在项目工作上花费的时间。 例如，在会议或培训中花费的时间也包含在FTE中。</p>

   FTE必须是最多为1的小数，并且不能为0。 例如，如果FTE值为0.5，且Workfront中的默认计划为40小时，则用户每周有20小时的空闲时间。

   该字段的默认值为1。

   计划例外情况、休息时间以及工作时间的值可能会影响用户的可用性。

   Workfront会根据设置区域中的资源管理首选项计算用户可用性。

   如果系统级别的资源管理首选项设置为用户调度，则此处指定的值将被忽略，并且会根据用户调度中指定的内容，将用户视为可用。

   有关更多信息，请参阅 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.

   有关在Workfront中创建时间表的详细信息，请参阅 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>.
   </li>

   <li><b>资源池</b>：将用户与资源池关联。 有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">将资源池与用户关联 </a>.</li>

   <li><b>成本率</b>：用户每小时的成本额。
      <p>对于日期有效成本率，请单击 <strong>添加费率</strong>. 输入时间期的成本费率值，并根据需要分配起始日期和终止日期。 成本费率1没有起始日期，最后一个成本费率没有终止日期。</p><p>某些日期会自动添加。 例如，如果成本费率1没有终止日期，并且您添加了“成本费率2”起始日期为2023年5月1日，则终止日期为2023年4月30日，这样成本费率1就不会出现任何差距。</p></li>

   <li><b>记帐费率</b>：用户每小时的计费金额。
      <p>对于日期有效计费率，请单击 <strong>添加费率</strong>. 输入时间期的开单费率值，并根据需要分配起始日期和终止日期。 记帐费率1没有开始日期，最后一个记帐费率没有结束日期。</p> <p>某些日期会自动添加。 例如，如果记帐费率1没有结束日期，而您添加了一个开始日期为2023年5月1日的秒数，则结束日期为2023年4月30日的秒数将添加到记帐费率1，因此不存在间隔。</p><p> <img alt="用户成本和记帐费率" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td><p>将现有用户自定义表单与此用户关联。 您必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 您无权编辑的字段不会显示在单独的自定义表单中。</p> <p><strong>注意：</strong> 高级自定义表单功能(如外部查找字段和Workfront本地字段)仅在您于详细信息页面（而非“编辑用户”对话框）中打开用户记录时可用。 （在用户列表中，单击用户名以打开详细信息。）</p> <p>有关创建自定义表单的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">评论</td> 
      <td>键入要发送给用户的评论以及用户配置文件的更新区域。</td> 
     </tr> 
    </tbody> 
   </table>
