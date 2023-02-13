---
title: 授予用户对特定区域的管理访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别向具有计划许可证管理访问权限的用户授予对系统某些区域的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# 授予用户对特定区域的管理访问权限

<!--Linked in several places, do not rename or change URL.-->

作为Adobe Workfront管理员，您可以使用访问级别向具有计划许可证管理访问权限的用户授予对系统某些区域的访问权限。

>[!NOTE]
>
>这与向用户授予对Workfront的完全管理访问权限不同，详情请参阅 [授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予计划用户对Workfront特定区域的管理访问权限

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后，您可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 （除了“系统管理员”和“外部用户”之外，您可以对每个访问级别执行此操作。）

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **访问级别**.
1. 单击要用于授予用户对Workfront某些区域的管理访问权限的访问级别的名称。
1. 在 **允许对** 复选框，以授予必要的管理访问权限。

   利用这些选项，可授予以下功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td><p>创建并管理审批流程，以便在整个系统中和针对特定组使用。</p><p>如果没有此访问权限，用户只能对他们有权管理的项目创建临时审批流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td><p>在Workfront中添加新公司并编辑现有公司</p>
      <p>如果没有此访问权限，用户只能查看现有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义表单</td> 
      <td><p>在其组内创建和编辑（添加、编辑和删除字段）自定义表单。</p><p>如果没有此访问权限，用户只能将现有表单附加到他们有权访问内容或管理的对象。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">汇率</td> 
      <td> <p>在Workfront中添加新货币。</p> <p>如果没有此访问权限，用户只能将现有货币添加到其创建的项目。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td><p>查看Workfront中对象的所有费用。</p><p>这不允许用户创建新的费用类型。</p><p>如果没有此访问权限，用户只能查看以下内容：</p>
       <ul>
        <li>项目、任务或其管理问题的费用</li>
        <li>自费</li>
        <li>下属的费用</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">职位角色</td> 
      <td> <p>通过此访问权限，用户可以执行以下操作：</p> 
       <ul> 
        <li>查看和编辑现有作业角色</li> 
        <li>添加新作业角色</li> 
        <li>编辑角色开单和成本费率</li> 
       </ul> <p><b>重要信息</b>:如果授予计划员用户对任务角色的管理访问权限，则系统将自动为用户启用“财务数据”访问权限设置“编辑角色开单和成本费率”。 之后，如果您禁用计划员用户对任务角色的管理访问权限，则用户仍可看到任务角色，因为编辑角色开单和成本费率设置仍处于启用状态。 如果发生这种情况，并且您需要删除用户查看作业角色的访问权限，则需要禁用用户的“编辑角色帐单和成本费率”权限设置。 有关说明，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的组中的里程碑</td> 
      <td>在“设置”的“里程碑路径”菜单下查看系统中的所有里程碑路径。 用户还可以编辑或删除属于其任何组的任何里程碑路径。 用户无法管理（编辑或删除）未分配给其任何组的里程碑路径。<br><p>如果没有此访问权限，用户只能查看现有里程碑路径，并将其应用于他们有权管理的项目。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中创建和管理提醒通知。<br>如果没有此访问权限，用户将只能接收和查看通知。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表和小时数</td> 
      <td> <p>允许用户查看Workfront中的所有工时单和工时单。</p> <p>禁用此选项后，用户只能在以下时间查看数小时：</p> 
       <ul> 
        <li>他们管理的项目、任务或问题</li> 
        <li>他们自己的时间表</li> 
        <li>向其报告的人的时间表</li> 
        <li>他们批准的时间表</li> 
       </ul> <p><b>注释</b>:  <p>无论是启用还是禁用此选项，组管理员都可以为他们管理的组和子组创建时间表配置文件，并将其分配给用户配置文件有权编辑的组成员。</p> <p>启用此选项可能会为某些组管理员提供过多的访问权限，因为他们可以查看由系统中所有用户（而不仅仅是他们管理的组中的用户）的时间表配置文件（和小时数）生成的时间表。 对于不需要这么多访问权限的组管理员，您可以禁用此选项。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完成后，单击 **保存**.
1. 将新的访问级别分配给用户，如 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >您可以允许用户拥有用户的管理访问权限。 有关为用户授予管理权限以便他们管理用户帐户的更多信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
