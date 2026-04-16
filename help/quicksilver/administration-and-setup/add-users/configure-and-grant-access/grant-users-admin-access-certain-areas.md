---
title: 授予用户对特定区域的管理访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别授予拥有计划许可证的用户对系统的某些区域的管理访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 5%

---

# 授予用户对特定区域的管理访问权限

<!--Linked in several places, do not rename or change URL.-->

作为Adobe Workfront管理员，您可以使用访问级别授予具有“标准”或“计划”许可证的用户对系统的某些区域的管理访问权限。

>[!NOTE]
>
>这与授予用户对Workfront的完全管理访问权限不同，在[授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)中对此进行了说明&#x200B;。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 向Standard或Plan用户授予对Workfront特定区域的管理访问权限

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


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->
