---
title: 授予用户对特定区域的管理访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别授予拥有计划许可证的用户对系统的某些区域的管理访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 2%

---

# 授予用户对特定区域的管理访问权限

<!--Linked in several places, do not rename or change URL.-->

作为Adobe Workfront管理员，您可以使用访问级别授予拥有计划许可证的用户对系统的某些区域的管理访问权限。

>[!NOTE]
>
>这与授予用户对Workfront的完全管理访问权限不同，在[授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)中对此进行了说明&#x200B;。

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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 授予计划用户对Workfront某些区域的管理访问权限

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 (您可以对每个访问级别（系统管理员和外部用户除外）执行此操作。)

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**访问级别**。
1. 单击要用于授予用户对Workfront特定区域的管理访问权限的访问权限级别的名称。
1. 在&#x200B;**允许**&#x200B;的管理访问权限部分中，选中复选框以授予必要的管理访问权限。

   利用这些选项，可授予以下功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td><p>创建和管理审批流程以用于整个系统和特定组。</p><p>如果没有此访问权限，用户只能对其有权管理的项目创建临时审批流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td><p>在Workfront中添加新公司和编辑现有公司</p>
      <p>如果没有此访问权限，用户只能查看现有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td><p>在其组中创建和编辑（添加、编辑和删除字段）自定义表单。</p><p>如果没有此访问权限，用户只能将现有表单附加到他们有权贡献或管理的对象。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">汇率</td> 
      <td> <p>在Workfront中添加新货币。</p> <p>如果没有此访问权限，用户只能向其创建的项目添加现有货币。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td><p>查看Workfront中对象的所有费用。</p><p>这不允许用户创建新的费用类型。</p><p>如果没有此访问权限，用户只能查看以下内容：</p>
       <ul>
        <li>他们管理的项目、任务或问题的费用</li>
        <li>他们自己的费用</li>
        <li>他们下属的开支</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作角色</td> 
      <td> <p>凭借此访问权限，用户可以执行以下操作：</p> 
       <ul> 
        <li>查看和编辑现有工作角色</li> 
        <li>添加新工作角色</li> 
        <li>编辑角色计费和成本率</li> 
       </ul> <p><b>重要信息</b>：如果您授予Planner用户工作角色的管理访问权限，则将自动为用户启用财务数据访问权限设置“编辑角色帐单和成本费率”。 之后，如果您禁用Planner用户对工作角色的管理访问权限，则工作角色仍对用户可见，因为编辑角色计费和成本费率设置仍处于启用状态。 如果发生这种情况，并且您需要删除用户查看工作角色的访问权限，则需要禁用用户的“编辑角色计费和成本费率”权限设置。 有关说明，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的组中的里程碑</td> 
      <td>在“设置”中的“里程碑路径”菜单下查看系统中的所有里程碑路径。 用户还可以编辑或删除属于其任何组的任何里程碑路径。 用户无法管理（编辑或删除）未分配给其任何组的里程碑路径。<br><p>如果没有此访问权限，用户只能查看现有的里程碑路径，并将它们应用于他们有权管理的项目。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中创建和管理提醒通知。<br>如果没有此访问权限，用户只能接收和查看通知。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表和小时数</td> 
      <td> <p>允许用户查看Workfront中的所有小时和时间表。</p> <p>禁用此选项后，用户只能在以下日期查看小时数：</p> 
       <ul> 
        <li>他们管理的项目、任务或问题</li> 
        <li>他们自己的时间表</li> 
        <li>向他们报告的人员的工时表</li> 
        <li>他们批准的工时表</li> 
       </ul> <p><b>注释</b>：  <p>无论此选项是启用还是禁用，组管理员都可以为其管理的组和子组创建时间表配置文件，并将它们分配给有权编辑其用户配置文件的组成员。</p> <p>启用此选项可能会为某些组管理员提供过多的访问权限，因为他们可以查看系统中所有用户（而不只是他们管理的组中的用户）的由时间表配置文件生成的时间表（以及小时数）。 您可以为不需要太多访问权限的组管理员禁用此选项。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完成后，单击&#x200B;**保存**。
1. 将新访问级别分配给用户，如[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)中所述。

   >[!NOTE]
   >
   >您可以允许用户具有管理访问权限。 有关授予用户管理权限以便他们能够管理用户帐户的更多信息，请参阅[授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
