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
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '2245'
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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。 </p> </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <img src="assets/gear-icon-in-access-levels.png">下至少启用<b>用户管理员</b>选项之一。 </p> <p>在这两个选项中，如果启用了用户<b>管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> <p>有关访问级别中<b>用户</b>设置的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 批量编辑用户帐户

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**用户** ![](assets/users-icon-in-main-menu.png)。

1. 选择多个用户，然后单击编辑图标![](assets/edit-icon.png)。

1. 在出现的&#x200B;**编辑用户**&#x200B;框中，更改以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">首选项</td> 
      <td> 
       <ul> 
        <li><b>时区：</b>用户的时区。</li> 
        <li><b>区域设置</b>：用户首选的区域设置。 这会影响来自Workfront的电子邮件中数字和日期的格式。</li> 
        <li><b>将我分配给自己的工作发送到我的“正在处理”选项卡</b>：如果您希望用户分配给自己的所有内容直接显示在其“正在处理”选项卡上，请选中此选项。 默认设置在用户的工作请求选项卡上列出分配给用户的所有内容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>选择应为新用户启用的电子邮件通知。<p>您可以选择即时通知和每日摘要通知。 所有选定用户的每日摘要通知将在同一时间后发送。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">为系统中的每个人配置事件通知</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问权限</td> 
      <td> 
       <ul> 
        <li><b>处于活动状态：</b>选择此字段以指示用户是否处于活动状态。 活动用户使用Workfront许可证。 取消选择该字段将停用用户。</li> 
        <li> 
        <p><b>访问级别：</b>选择要分配给这些用户的访问级别。 所有选定用户都将具有相同的访问级别。
        </p> 
        <p>当用户分配访问级别时，您可以分配等于或低于您自己的访问级别的级别。 （例如，如果您的访问级别是“规划者”，则不能分配“管理员”访问级别。） </p>
        <p>但是，如果Workfront管理员对访问级别启用了您自己未启用的权限，则无法分配低于您自己的访问级别（通过“微调”设置，如<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>中所述）。</p> 
        <p>有关访问级别的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问</a>。</p> 
         </li> 
        <li> 
        <p><b>布局模板</b>：为用户选择布局模板。 分配给用户的布局模板将优先于分配给其主组、主团队或主要工作角色的任何布局模板。 有关布局模板的分配优先级的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>。</p> 
        <p><b>注意</b>：在此字段中可用的布局模板列表取决于您的访问权限：
          <ul>
           <li>作为Workfront管理员，您可以查看所有系统级和组级布局模板。</li>
           <li>作为组管理员，您可以查看系统级布局模板以及与您管理的组关联的模板。</li>
           <li><p>作为具有Planner许可证和编辑用户访问权限的用户，您只能查看系统级布局模板。 </p>
           <p>有关组级布局模板的信息，请参阅<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>。</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组织</td> 
      <td> 
       <ul> 
        <li><b>公司</b>：用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中只显示有效的公司。 有关创建公司的信息，请参阅了解和管理公司。</li> 
        <li><b>主团队</b>：指定用户的主团队。 用户只能有一个主团队。 </li> 
        <li><b>其他团队</b>：用户可以属于多个团队。 </li> 
        <li> <p><b>主组：</b>选择适当的组以将用户分配为其主组。 这使用户能够访问与组共享的对象。</p> <p><b>注意</b>：这是必填字段。 不能将用户与主组关联。</p> <p>仅当出现以下情况时，才可以为用户分配组：</p> 
         <ul> 
          <li>您是Workfront管理员。</li> 
          <li>您是该组的管理员。</li> 
          <li>该团体是公开的。</li> 
         </ul> </li> 
        <li> <p><b>其他组</b>：用户可以属于多个组。 仅在以下情况下才能将组分配给用户：</p> 
         <ul> 
          <li>您是Workfront管理员。</li> 
          <li>您是该组的管理员。</li> 
          <li> <p>该团体是公开的。 </p> 
          <p>有关公用组的详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建组</a>。</p> 
          <p>有关组的详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">组概述</a>。</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源规划</td> 
      <td> 
       <ul>

   <li>
       <b>工作时间</b>：表示用户可用于实际工作的相当于全职(FTE)时间的百分比，不包括开销。 工作时间必须为最多为1的小数，不得为0。 例如，实际工作的20%可用性为0.2。

   该字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。

   系统使用此数字来计算用户是否可用于实际的项目相关工作。

   有关在Workfront中创建计划的详细信息，请参阅<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>。

   安排例外和休息时间也可能会影响用户容量。

   Workfront会根据设置区域中的资源管理首选项计算用户可用性。 有关详细信息，请参阅<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>。

   <b>提示</b>

   将“工作时间”值设置为1，表示用户可用于其整个全职等效项目相关工作。
   </li>

   <li><b>计划停用</b>：如果要计划在一段时间后停用用户，请选中此框。</li> 
       <li><b>计划的停用日期</b>：停用用户后的日期。 有关安排用户停用的详细信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>中的<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">安排用户停用</a>部分。</li> 
       <li> <p><b>主要角色</b>：这是用户在Workfront中的主要工作角色。 默认情况下，分配给用户的每个任务和问题也会分配给此工作角色。 工作角色在资源管理中至关重要。 有关工作角色的更多信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理工作角色</a></p> <p>只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</p> </li> 
       <li>（视情况而定）如果您选择了<b>主要角色</b>，则会显示<b>FTE可用性百分比</b>字段。 指定将用户计划的时间百分比分配给此工作角色。 主角色的FTE可用性百分比的默认值为100%。</li> 
       <li> <p><b>其他角色</b>：用户在Workfront中可以有多个工作角色。 工作角色在资源管理中至关重要。 用户可以履行的工作角色数量没有限制。 但是，我们建议不要将一位用户分配给过多的工作角色，因为对于这些用户而言，资源管理可能变得过于复杂。</p> <p>有关工作角色的更多信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理工作角色</a>。</p> <p>只有在您拥有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>。</p> </li> 
       <li> <p>（视情况而定）如果您选择了一个或多个<b>其他角色</b>，则将为每个角色显示<b>FTE可用性百分比</b>字段。 指定将用户计划的时间百分比分配给每个工作角色。 其他角色的FTE可用性百分比的默认值为0%。</p> <p><b>注释</b>：  
       <ul> 
       <li>如果其他角色的FTE可用性为0%，则它们不会显示在Resource Planner中，除非将用户分配给这些角色中的任务。</li> 
       <li> <p>所有角色的FTE可用性的所有百分比的总和必须等于100%。 每个FTE可用百分比计算资源规划者中每个用户的每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。</p> <p>Workfront会根据Workfront管理员在资源管理首选项中选择用于计算FTE的方法，计算用户的可用时间。</p> <p>有关计算用户可用性的详细信息，请参阅<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">计算资源规划者中用户和角色的小时和FTE的概述</a>。</p> <p>有关配置资源管理首选项的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>。</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>计划</b>：将计划与用户关联。 用户调度计算用户所分配任务的时间线。</p> <p>Workfront管理员或组管理员必须先创建计划，然后才能将其与用户关联。</p> <p>选择系统级别或组计划以将其分配给所选用户。</p> <p>有关系统级别和组计划的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>。</p> <p><b>重要信息</b>：仅当“计算资源可用性”设置设为“用户的计划”时，Workfront才会使用用户的计划。 有关使用计算资源可用性设置如何影响用于资源管理的计划的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>。</p> </li> 
       <li> <p><b>时间表配置文件</b>：将时间表配置文件与用户关联。 这可确保自动为用户生成时间表。</p> 
       <p><b>注释</b>：  
       <ul> 
       <li>在此字段中可用的时间表用户档案列表取决于您的访问权限：
       <ul>
       <li>作为Workfront管理员，您可以查看所有系统级别和组级别的时间表配置信息。</li>
       <li><p>作为组管理员，您可以查看系统级时间表配置文件，以及与您管理的组相关联的时间表配置文件。</p></li>
       <li><p>作为具有Planner许可证和编辑用户访问权限的用户，您只能看到系统级时间表配置文件。</p></li>
       </ul></li> 
       <li>如果您是组管理员，则您编辑的所有用户都必须是您管理的组的成员。</li> 
       </ul> </p> </li> 
       <li><b>默认小时类型</b>：为用户选择默认小时类型。 这是用户记录时间时默认使用的小时类型。</li> 
       <li> <p><b>可用小时类型</b>：选择用户应可用的小时类型。 这些小时类型在Workfront中用户可以记录时间的任意位置均可见。 用户只能看到在项目级别以及用户级别启用的小时类型。</p> 
       <p>有关用户可用的小时类型的详细信息，请参阅<a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定义小时类型和可用性</a>。</p> 
       </li> 
       <li> <b>FTE</b>：这是该用户的等效全职。 仅当系统级别的资源管理首选项设置为默认计划时，Workfront才使用此数字根据默认计划计算用户可用性。

   <p>FTE表示用户可在工作上花费的时间。 这包括管理费用以及在项目工作上花费的时间。 例如，在会议或培训中花费的时间也包含在FTE中。</p>

   FTE必须是最多为1的小数，并且不能为0。 例如，如果FTE值为0.5，且Workfront中的默认计划为40小时，则用户每周有20小时的空闲时间。

   该字段的默认值为1。

   计划例外情况、休息时间以及工作时间的值可能会影响用户的可用性。

   Workfront会根据设置区域中的资源管理首选项计算用户可用性。

   如果系统级别的资源管理首选项设置为用户调度，则此处指定的值将被忽略，并且会根据用户调度中指定的内容，将用户视为可用。

   有关详细信息，请参阅<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>。

   有关在Workfront中创建计划的详细信息，请参阅<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>。
   </li> 
       <li> <p><b>资源池</b>：将用户与资源池关联。</p> <p><b>注意</b>：只有所有选定用户通用的资源池才会显示在此字段中。 如果所选用户没有共享资源池，则此字段为空。 如果此字段为空，则在此处指定的资源池将覆盖其各自的资源池。</p> 
       <p>有关资源池的详细信息，请参阅<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">资源池概述</a>。</p> </li> 
       <li><b>每小时成本</b>：用户每小时的成本金额。 </li> 
       <li><b>按小时计费</b>：用户每小时的计费金额。</li> 
       <li><b>自定义Forms</b>：将现有用户自定义表单与用户关联。 您必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>。</li> 
       <li><b>注释</b>：在提供的字段中输入注释。 所有选定用户都将收到应用程序内通知以及包含您评论的电子邮件通知。 该注释显示在用户配置文件的更新选项卡中。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在&#x200B;**自定义Forms**&#x200B;部分中，选择&#x200B;**重新计算自定义表达式**&#x200B;选项，以确保附加到所选用户的自定义表单中的所有已计算自定义字段都是最新的。

1. 单击&#x200B;**保存更改**。
