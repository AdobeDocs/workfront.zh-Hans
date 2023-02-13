---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 批量编辑用户配置文件
description: 作为Adobe Workfront管理员，您可以批量编辑用户帐户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# 批量编辑用户配置文件

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中编辑用户配置文件的说明，请参阅文章中的“编辑用户详细信息”部分 [批量上传用户](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 或联系Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以批量编辑用户帐户。 在批量编辑用户时，只有您专门选择的字段才会更新，并使用与所有选定用户相同的信息。 您未选中的所有其他字段对于每个用户都保持相同，即使每个用户的字段不同也是如此。

>[!NOTE]
>
>* 您无法批量编辑用户配置文件的“个人信息”部分，因为该信息对于每个用户都必须是唯一的。
>* 为确保数据的准确性和最佳性能，我们建议您一次最多选择2000个用户，以便进行批量编辑。
>


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

## 批量编辑用户帐户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择多个用户，然后单击编辑图标 ![](assets/edit-icon.png).

1. 在 **编辑用户** 框中，更改以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">首选项</td> 
      <td> 
       <ul> 
        <li><b>时区：</b> 用户的时区。</li> 
        <li><b>区域设置</b>:用户的首选区域设置。 这会影响来自Workfront的电子邮件中的数字和日期格式。</li> 
        <li><b>显示更新状态完成百分比</b>:如果要在所有用户的任务更新流中显示一个完成百分比栏，请勾选此选项。</li> 
        <li><b>将我分配给自己的工作发送到我的工作选项卡</b>:如果您希望用户分配给自己的所有内容都直接显示在其“工作原因”选项卡中，请勾选此选项。 默认设置是在用户的“工作请求”选项卡上列出分配给用户的所有内容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>选择应为新用户启用的电子邮件通知。<p>您可以选择即时通知和每日摘要通知。 对于所有选定的用户，所有每日摘要通知会在同一时间之后的某个时间发送。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">为系统中的每个人配置事件通知</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">访问权限</td> 
      <td> 
       <ul> 
        <li><b>处于活动状态：</b> 选择此字段可指示用户是否处于活动状态。 活动用户使用Workfront许可证。 取消选择该字段会停用用户。</li> 
        <li> 
        <p><b>访问级别：</b> 选择要分配给这些用户的访问级别。 所有选定的用户都将具有相同的访问级别。
        </p> 
        <p>在为用户分配访问级别时，您可以分配等于或小于您自己的访问级别的级别。 （例如，如果您的访问级别是“计划员”，则您无法分配“管理员”访问级别。） </p>
        <p>但是，如果Workfront管理员在访问级别上启用了您自己未启用的权限，则您不能分配低于您自己的访问级别(通过“微调”设置，如 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>)。</p> 
        <p>有关访问级别的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">配置对Adobe Workfront的访问权限</a>.</p> 
         </li> 
        <li> 
        <p><b>布局模板</b>:为用户选择布局模板。 分配给用户的布局模板将优先于分配给其“主组”、“主组”或“主作业”角色的任何布局模板。 有关布局模板的分配优先级的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> 
        <p><b>注意</b>:您在此字段中可用的布局模板列表取决于您的访问权限：
          <ul>
           <li>作为Workfront管理员，您可以查看所有系统级别和组级别布局模板。</li>
           <li>作为组管理员，您可以查看系统级别的布局模板，以及与您管理的组关联的布局模板。</li>
           <li><p>作为具有计划员许可证的用户并有权编辑用户，您只能看到系统级别的布局模板。 </p>
           <p>有关组级别布局模板的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组织</td> 
      <td> 
       <ul> 
        <li><b>公司</b>:用户的公司。 用户只能与一个公司关联。 必须先创建公司，然后才能将其与用户关联。 列表中仅显示活动的公司。 有关创建公司的信息，请参阅了解和管理公司。</li> 
        <li><b>主队</b>:为用户指定主团队。 用户只能有一个主团队。 </li> 
        <li><b>其他团队</b>:用户可以属于多个团队。 </li> 
        <li> <p><b>主页组：</b> 选择相应的组以将用户分配为其“主页”组。 这允许用户访问与组共享的对象。</p> <p><b>注意</b>:这是必填字段。 不能有未与主页组关联的用户。</p> <p>您只能在以下情况下将群组分配给用户：</p> 
         <ul> 
          <li>您是Workfront管理员。</li> 
          <li>您是该组的管理员。</li> 
          <li>该群是公开的。</li> 
         </ul> </li> 
        <li> <p><b>其他组</b>:用户可以属于多个组。 您只能在以下情况下将群组分配给用户：</p> 
         <ul> 
          <li>您是Workfront管理员。</li> 
          <li>您是该组的管理员。</li> 
          <li> <p>该群是公开的。 </p> 
          <p>有关公共群组的更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">创建群组</a>.</p> 
          <p>有关群组的更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群组概述</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源规划</td> 
      <td> 
       <ul> 
        <li><b>计划停用</b>:如果要计划在一段时间后停用用户，请选中此框。</li> 
        <li><b>计划停用日期</b>:在此日期之后，用户将被停用。 有关计划用户停用的更多信息，请参阅部分 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">计划用户停用</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a>.</li> 
        <li> <p><b>主要角色</b>:这是用户在Workfront中拥有的主要作业角色。 默认情况下，分配给用户的每个任务和问题也会分配给此作业角色。 作业角色在资源管理中是必不可少的。 有关作业角色的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a></p> <p>仅当您具有具有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
        <li>（视情况而定）如果您选择了 <b>主要角色</b>, <b>FTE可用性百分比</b> 字段。 指定将用户计划的时间百分比分配给此作业角色。 主角色的FTE可用性百分比的默认值为100%。</li> 
        <li> <p><b>其他角色</b>:用户在Workfront中可以具有多个作业角色。 作业角色在资源管理中是必不可少的。 用户可以履行的作业角色数量没有限制。 但是，我们建议不要为一个用户分配过多的作业角色，因为对于这些用户而言，资源管理可能变得过于复杂。</p> <p>有关作业角色的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> <p>仅当您具有具有管理用户访问权限的计划许可证，或者您是Workfront管理员时，才能更新此字段。 有关设置具有管理用户访问权限的用户的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
        <li> <p>（视情况而定）如果您选择了一个或多个 <b>其他角色</b>, <b>FTE可用性百分比</b> 字段。 指定将用户计划的时间百分比分配给每个作业角色。 其他角色的FTE可用性百分比的默认值为0%。</p> <p><b>注释</b>:  
          <ul> 
           <li>如果其他角色具有0% FTE可用性，则它们不会显示在资源计划器中，除非将用户分配到这些角色中的任务。</li> 
           <li> <p>所有角色的FTE可用性的所有百分比总和必须等于100%。 每个FTE可用性百分比计算资源计划器中每个用户每个角色的可用小时数。 每个用户每个角色的可用小时数取决于用户的可用时间。</p> <p>用户的可用时间由Workfront计算，具体取决于Workfront管理员在“资源管理首选项”中选择的用于计算FTE的方法。</p> <p>有关计算用户可用性的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.</p> <p>有关配置资源管理首选项的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>计划</b>:将计划与用户关联。 用户的计划将计算用户分配到的任务的时间线。</p> <p>Workfront管理员或组管理员必须先创建计划，然后才能将其与用户关联。</p> <p>选择系统级别或组计划，将其分配给选定的用户。</p> <p>有关系统级别和组计划的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p><b>重要信息</b>:Workfront仅在将“使用计算资源可用性”设置设置为“用户的计划”时才使用用户的计划。 有关“使用计算资源可用性”设置如何影响用于资源管理的计划的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> </li> 
        <li> <p><b>时间表配置文件</b>:将时间表配置文件与用户关联。 这可确保为用户自动生成工时单。</p> 
        <p><b>注释</b>:  
          <ul> 
           <li>此字段中可用的时间表配置文件列表取决于您的访问权限：
            <ul>
             <li>作为Workfront管理员，您可以查看所有系统级别和组级别的时间表配置文件。</li>
             <li><p>作为组管理员，您可以查看系统级别的时间表配置文件，以及与您管理的组关联的时间表配置文件。</p></li>
             <li><p>作为具有计划员许可证并有权编辑用户的用户，您只能查看系统级别的时间表配置文件。</p></li>
            </ul></li> 
           <li>如果您是群组管理员，则您编辑的所有用户都必须是您所管理群组的成员。</li> 
          </ul> </p> </li> 
        <li><b>默认小时类型</b>:为用户选择默认的小时类型。 这是用户记录时间时默认使用的小时类型。</li> 
        <li> <p><b>可用小时类型</b>:选择用户应可用的小时类型。 这些小时类型在Workfront中的任意位置都可见，用户可以在其中记录时间。 用户只能查看在项目级别和用户级别启用的小时类型。</p> 
        <p>有关用户可使用的小时类型的更多信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定义工时单的工时类型和可用性</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>:只有在系统级别的“资源管理首选项”设置为 <b>默认计划</b>.</p> 
        <p>例如，如果FTE值为0.5，而默认计划为40小时，则用户每周可工作20小时。 有关在选择“默认计划”时计划例外或关闭时间如何影响用户可用性的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>. </p> 
        <p>如果系统级别的“资源管理首选项”设置为 <b>用户的计划</b>，则此处指定的值将被忽略，用户将根据其计划中指定的内容被视为可用。 在这种情况下，资源计划员用户的FTE通过以下公式计算：</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>有关计算用户FTE的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>.</p> <p>有关在Workfront中创建计划的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> <p>有关配置资源管理首选项的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置资源管理首选项</a>.</p> 
        </li> 
        <li> <p><b>资源池</b>:将用户与资源池关联。</p> <p><b>注意</b>:只有所有选定用户共有的资源池才会显示在此字段中。 如果选定的用户没有共享资源池，则此字段为空。 如果此字段为空，则此处指定的资源池将覆盖其各个资源池。</p> 
        <p>有关资源池的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 资源池概述 </a>.</p> </li> 
        <li><b>每小时成本</b>:用户每小时的成本金额。 </li> 
        <li><b>每小时计费</b>:用户每小时的账单金额。</li> 
        <li><b>自定义Forms</b>:将现有用户自定义表单与用户关联。 必须先创建自定义表单，然后才能将其与用户关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</li> 
        <li><b>注释</b>:在提供的字段中输入评论。 选定的所有用户都将收到应用程序内通知以及包含您的评论的电子邮件通知。 该评论显示在用户配置文件的更新选项卡中。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在 **自定义Forms** 选择 **重新计算自定义表达式** 选项，以确保附加到选定用户的自定义表单中所有计算量度的自定义字段都是最新的。

1. 单击 **保存更改**.
