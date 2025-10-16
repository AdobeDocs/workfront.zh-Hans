---
title: 创建和修改自定义访问级别
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以创建自定义访问级别并将其应用于用户。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 6%

---

# 创建和修改自定义访问级别

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

作为Adobe Workfront管理员，您可以创建自定义访问级别并将其应用于用户。 当您使用访问级别时，了解它们如何与用户在彼此共享对象时授予的对象权限一起工作很重要。 有关访问级别的详细信息，请参阅：

* [新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 您可以对每个访问级别（系统管理员和外部用户除外）执行此操作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建或编辑自定义访问级别

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**访问级别**。
1. &#x200B;
   * 在生产环境中：
选择要复制和自定义的访问级别，然后单击&#x200B;**复制**。

     或

     如果您正在编辑现有的访问级别（您之前复制过的），请单击其名称。

   * 在预览环境中<span class="preview">：</span>

     <span class="preview">选择要复制和自定义的访问级别，然后单击&#x200B;**复制**&#x200B;图标![复制图标](assets/copy-icon.png)。</span>

     <span class="preview">或</span>

     <span class="preview">如果您正在编辑现有的访问级别，请通过单击该访问级别左侧的框选择访问级别，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。</span>

1. 在显示的框中，执行以下任一操作以开始配置自定义访问级别：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>键入访问级别的名称。 </p> <p>如果您刚刚复制了一个访问级别以创建新访问级别，则默认名称为“访问级别名称（复制）”，其中“访问级别名称”是您复制的访问级别。</p> <p><strong>提示</strong>：我们建议您在副本的名称中包含访问级别的原始名称。 例如，在ACME公司，标准访问级别的副本可能命名为ACME Standard。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述 </td> 
      <td>键入访问级别的描述。 在此处列出具有此访问级别的用户能够访问的内容会很有帮助。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">许可证类型</td> 
      <td>请确保此处选择的许可证与您创建或编辑的访问级别类型最相关。 所选许可证确定访问级别可用的设置。 有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新许可证概述</a>或<a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">许可证概述</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果在&#x200B;**许可证类型**&#x200B;框中选择了&#x200B;**标准**&#x200B;或&#x200B;**计划**，请滚动到&#x200B;**允许**&#x200B;的管理访问权限，并为将拥有此访问级别的用户选择管理访问权限。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td>创建和管理审批流程以用于整个系统和特定组。<p>如果没有此访问权限，用户只能对其有权管理的项目创建临时审批流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>在Workfront中添加新公司和编辑现有公司。<br><p>如果没有此访问权限，用户只能查看现有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td>创建和管理其组中的所有自定义表单。 <br><p>如果没有此访问权限，用户只能将现有表单附加到他们有权贡献或管理的对象。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">汇率</td> 
      <td> 在Workfront中添加新货币。 <p>如果没有此访问权限，用户只能将现有货币添加到他们创建的项目。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>查看Workfront中对象的所有费用。<p>如果没有此访问权限，用户只能查看以下内容：</p>
       <ul>
        <li>他们管理的项目、任务或问题的费用</li>
        <li>他们自己的费用</li>
        <li>他们下属的开支</li>
       </ul><p><b>注意</b>：不允许用户创建新的费用类型。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作角色</td> 
      <td> 凭借此访问权限，用户可以执行以下操作： 
       <ul> 
        <li>查看和编辑现有工作角色</li> 
        <li>添加新工作角色</li> 
        <li>编辑角色计费和成本率</li> 
       </ul> 
       <p>有关对工作角色具有管理访问权限的Standard或Planner用户可用以访问财务数据的重要信息，请参阅<a href="#standard-or-planner-users-with-administrative-access-to-job-roles">对工作角色具有管理访问权限的Standard或Planner用户</a>。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的组中的里程碑</td> 
      <td>在“设置”中的“里程碑路径”菜单下查看系统中的所有里程碑路径。 用户还可以编辑或删除属于其任何组的任何里程碑路径。 用户无法管理（编辑或删除）未分配给其组的里程碑路径。<p>如果没有此访问权限，用户只能查看现有的里程碑路径，并将它们应用于他们有权管理的项目。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中创建和管理提醒通知。<p>如果没有此访问权限，用户将只能接收和查看通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表和小时数</td> 
      <td> 组管理员可以将时间表配置文件分配给其管理的组和子组中的用户。 <p>如果未启用此选项，组管理员无法将时间表配置文件分配给他们管理的组和子组中的其他用户，尽管他们可以创建这些用户档案。</p> <p>所有其他拥有Standard或Plan许可证的用户都可以在Workfront中查看所有小时和工时表。</p> <p>如果未启用此选项，用户只能在以下日期查看小时数：</p> 
       <ul> 
        <li>他们管理的项目、任务或问题</li> 
        <li>他们自己的时间表</li> 
        <li>向他们报告的人员的工时表</li> 
        <li>他们批准的工时表</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**设置其他限制**，然后为访问级别设置以下任何限制。

   >[!IMPORTANT]
   >
   >对于供应商（不属于您组织的任何人）等外部用户，我们建议您限制对任务、项目、更新、公告、其他公司、团队和组的访问权限。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">不要给分派任务或问题的整个项目授予访问权限</td> 
      <td> 阻止分配给任务或问题的用户也获得父项目的权限，即使项目权限允许这样做。<p>有关配置项目权限的详细信息，请参阅文章<a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a>编辑项目<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">中的部分</a>。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">不要从项目、任务、问题等...继承文档访问权限</td> 
      <td>阻止文档继承在其父对象上设置的权限。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">视图仅在已将他们包含在会话中的位置上更新</td> 
      <td> 允许用户仅查看包含其名称或团队名称的注释。 <p> <p><b>注意</b>：这将阻止用户订阅Workfront中的项目。 有关订阅项目的详细信息，请参阅<a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">在Adobe Workfront中订阅项目</a>。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">切勿允许用户删除评论 </td> 
      <td> 阻止用户删除他们对项目所做的评论。  <p><b>注意</b>：没有人可以删除其他用户的评论。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">仅查看他们属于的公司、组和团队</td> 
      <td>允许用户仅查看项目并与他们所属的公司、组和团队共享项目。<p><strong>注意</strong>：具有请求者或参与者许可证的用户无法查看他们不属于的公司，即使选择了此选项也是如此。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">绝不允许计划小时数或实际小时数可见</td> 
      <td>阻止用户查看他们有权访问的工作项的计划和实际小时数。 但是，他们可以查看自己登录的实际小时数，或他们下属人员记录的小时数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允许用户删除公告</td> 
      <td>防止用户删除公告中心中的公告。 有关详细信息，请参阅<a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">发送公告</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. （有条件，可选）如果您的Workfront系统设置为属于多个公司的用户，请根据其他用户在部分&#x200B;**中所属的公司来限制其他用户的可见性。其他公司的人员应仅查看来自**&#x200B;的用户。

   您可以限制用户仅查看其公司或您指定为主要公司的公司的用户。 主要公司通常表示您的大多数用户工作的Workfront帐户。 有关主要公司的详细信息，请参阅[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

   >[!NOTE]
   >
   >如果两个用户属于两个不同的公司，但他们都可以看到来自主要公司的用户，则他们可以看到与主要公司关联的“更新”区域。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 单击&#x200B;**保存**。

   创建访问级别后，您可以将其分配给用户（除非是系统管理员访问级别）。

   有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

   有关Adobe管理员如何为用户分配系统管理员访问权限级别的信息，请参阅[授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)。

## 对工作角色具有管理访问权限的标准或Planner用户 {#planner-users}

如果您向“标准”或“规划者”用户授予工作角色的管理访问权限，则将自动为用户启用“编辑角色计费和成本费率”设置。

之后，如果您为用户禁用工作角色的管理访问权限，则用户仍可看到工作角色，因为编辑角色计费和成本费率设置仍处于启用状态。

如果发生这种情况，并且您需要删除用户查看工作角色的访问权限，则需要禁用用户的“编辑角色计费和成本费率”权限设置。 有关说明，请参阅[授予对财务数据的访问权限](grant-access-financial.md)。



