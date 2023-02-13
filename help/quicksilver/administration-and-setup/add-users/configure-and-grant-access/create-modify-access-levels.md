---
title: 创建或修改自定义访问级别
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以创建自定义访问级别并将其应用于用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 6%

---

# 创建和修改自定义访问级别

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help.-->

作为Adobe Workfront管理员，您可以创建自定义访问级别并将其应用于用户，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

在使用访问级别时，务必要了解它们如何与用户在彼此共享对象时授予的对象权限一起使用。 有关更多信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后，您可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 （除了“系统管理员”和“外部用户”之外，您可以对每个访问级别执行此操作。）

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="#" class="MCXref xref selected">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建或编辑自定义访问级别

{{step-1-to-setup}}

1. 单击 **访问级别** 中。
1. 选择要复制和自定义的访问级别，然后单击 **复制**.

   或

   如果您正在编辑现有访问级别（您之前复制的访问级别），请单击其名称。

1. 在显示的框中，执行以下任一操作以开始配置自定义访问级别：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>键入访问级别的名称。 </p> <p>如果您刚刚复制了访问级别以创建新访问级别，则默认名称为访问级别名称（副本），其中访问级别名称是您复制的访问级别。</p> <p><strong>笔尖</strong>:我们建议您在副本名称中包含访问级别的原始名称。 例如，在ACME公司，计划员访问层的副本可以命名为ACME计划员。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述 </td> 
      <td>键入访问级别的描述。 在此处列出具有此访问级别的用户将能够访问哪些内容将非常有用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">许可证类型</td> 
      <td>确保此处选择的许可证与您创建或编辑的访问级别类型最为相关。 所选许可证决定哪些设置可用于访问级别。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果 **计划** 的 **许可证类型** 框中，滚动到部分 **允许对** 并为将具有此访问权限级别的用户选择管理访问权限。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td>创建并管理审批流程，以便在整个系统中和针对特定组使用。<p>如果没有此访问权限，用户只能对他们有权管理的项目创建临时审批流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>在Workfront中添加新公司并编辑现有公司。<br><p>如果没有此访问权限，用户只能查看现有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>创建并管理其组中的所有自定义表单。 <br><p>如果没有此访问权限，用户只能将现有表单附加到他们有权访问或管理的对象。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">汇率</td> 
      <td> <p>在Workfront中添加新货币。</p> <p>如果没有此访问权限，用户只能将现有货币添加到其创建的项目。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>查看Workfront中对象的所有费用。<p>如果没有此访问权限，用户只能查看以下内容：</p>
       <ul>
        <li>项目、任务或其管理问题的费用</li>
        <li>自费</li>
        <li>下属的费用</li>
       </ul><p><b>注意</b>:这不允许用户创建新的费用类型。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">职位角色</td> 
      <td> <p>通过此访问权限，用户可以执行以下操作：</p> 
       <ul> 
        <li>查看和编辑现有作业角色</li> 
        <li>添加新作业角色</li> 
        <li>编辑角色开单和成本费率</li> 
       </ul> 
       <p>有关对具有管理权限的计划员用户有权访问任务角色的财务数据的访问权限的重要信息，请参阅 <a href="#planner-users-with-administrative-access-to-job-roles">具有作业角色管理访问权限的计划员用户</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的组中的里程碑</td> 
      <td>在“设置”的“里程碑路径”菜单下查看系统中的所有里程碑路径。 用户还可以编辑或删除属于其任何组的任何里程碑路径。 用户无法管理（编辑或删除）未分配给其组的里程碑路径。<p>如果没有此访问权限，用户只能查看现有里程碑路径，并将其应用于他们有权管理的项目。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中创建和管理提醒通知。<p>如果没有此访问权限，用户将只能接收和查看通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表和小时数</td> 
      <td> <p>组管理员可以将工时单配置文件分配给他们管理的组和子组中的用户。</p> <p>如果未启用此选项，组管理员将无法将工时单配置文件分配给其管理的组和子组中的其他用户，但他们可以创建工时单配置文件。</p> <p>拥有计划许可证的所有其他用户都可以在Workfront中查看所有小时和工时单。</p> <p>如果未启用此选项，则用户只能在以下时间查看小时：</p> 
       <ul> 
        <li>他们管理的项目、任务或问题</li> 
        <li>他们自己的时间表</li> 
        <li>向其报告的人的时间表</li> 
        <li>他们批准的时间表</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **设置其他限制**，然后为访问级别设置以下任何限制。

   >[!IMPORTANT]
   >
   >对于外部用户(例如供应商（不在您组织中的任何人），我们建议您限制对任务、项目、更新、公告、其他公司、团队和组的访问。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">不要给分派任务或问题的整个项目授予访问权限</td> 
      <td> 阻止分配给任务或问题的用户也获得父项目的权限，即使项目权限允许也是如此。<p>有关配置项目权限的更多信息，请参阅部分 <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> 在文章中 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">编辑项目</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">不要从项目、任务、问题等...继承文档访问权限</td> 
      <td>阻止文档继承其父对象上设置的权限。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">视图仅在已将他们包含在会话中的位置上更新</td> 
      <td> <p>允许用户仅查看已包含其名称或团队名称的评论。</p> <p> <p><b>注意</b>:这会阻止用户订阅Workfront中的项目。 有关订阅项目的更多信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">添加用户</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">切勿允许用户删除评论 </td> 
      <td> <p>阻止用户删除他们对项目所做的评论。 </p> <p><b>注意</b>:任何人都不能删除其他用户的评论。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">仅查看他们属于的公司、组和团队</td> 
      <td>允许用户仅查看项目并与其所属的公司、组和团队共享项目。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">绝不允许计划小时数或实际小时数可见</td> 
      <td>阻止用户查看他们有权访问的工作项的计划小时数和实际小时数。 但是，他们可以查看自己记录的实际小时数，或由向他们报告的人员记录的小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允许用户删除公告</td> 
      <td>阻止用户删除公告中心中的公告。 有关更多信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">发送公告</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定和可选）如果为属于多个公司的用户设置了Workfront系统，则会根据其在部分中所属的公司，将可见性限制为其他用户 **其他公司中的用户只能查看**.

   您可以限制用户仅查看来自其自己公司或您指定为主要公司的公司的用户。 有关主公司的详细信息，请参阅 [创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >如果两个用户属于两个不同的公司，但他们都可以查看来自主公司的用户，则他们可以看到与主公司关联的更新区域。

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 单击&#x200B;**保存**。

   创建访问级别后，您可以将其分配给用户（除非该用户是系统管理员访问级别）。

   有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   有关Adobe管理员如何为用户分配系统管理员访问级别的信息，请参阅 [授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## 具有作业角色管理访问权限的计划员用户 {#planner-users}

如果您授予计划员用户对任务职责的管理访问权限，系统将自动为用户启用“编辑职责开单和成本费率”设置。

之后，如果您禁用对用户作业角色的管理访问，则用户仍可看到作业角色，因为“编辑角色帐单和成本费率”设置仍处于启用状态。

如果发生这种情况，并且您需要删除用户查看作业角色的访问权限，则需要禁用用户的“编辑角色帐单和成本费率”权限设置。 有关说明，请参阅 [授予对财务数据的访问权限](grant-access-financial.md).
