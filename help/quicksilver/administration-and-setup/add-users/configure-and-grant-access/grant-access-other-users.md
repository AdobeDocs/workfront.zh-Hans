---
title: 授予用户访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中其他用户的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# 授予用户访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中其他用户的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## 配置用户访问权限

您可以使用您创建的默认访问级别或自定义访问级别管理用户可以查看和编辑的其他用户的信息。 具有默认“计划”和“工作”许可证的用户可以查看其他用户的联系信息。 以下任何用户都可以创建和编辑其他用户：

* Workfront管理员。

   有关更多信息，请参阅 [授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* 具有默认计划许可证且也有权访问用户的用户，如本文所述。

   限制为仅查看其公司或主要公司用户的用户，则只能编辑他们能够查看的用户。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 具有默认计划许可证的用户，也被指定为其他用户的经理。

   在其访问级别授予用户编辑访问权限的用户可以管理向其报告的用户。 有关管理用户的信息，请参阅 [查看组织图](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* 具有默认计划许可证的用户如果创建了用户，则可以停用、删除或编辑他们创建的用户。 有关创建新用户的信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 配置用户的访问权限以使用自定义访问级别编辑用户

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 要更改具有计划或工作许可证的用户查看其他用户配置文件的功能，请执行以下操作：

   1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 按钮 **用户**.

   1. 禁用 **查看联系信息**，然后单击X以关闭 **优化设置** 框中。

1. 要修改具有计划许可证访问权限的用户编辑其他用户的功能，请单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **编辑** 按钮 **用户**，然后选择要授予的功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>创建</strong> </td> 
      <td> <p>允许用户创建用户。<br>默认情况下，此选项处于启用状态。</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">请确保在解除这2个注释之前进行此更改。 在3/29上，请求文档说，这取决于调查结果。</p>

       &lt;p>&lt;b>注意&lt;/b>:如果贵组织已载入Adobe Admin Console，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>删除</strong> </td> 
      <td> <p> 允许用户删除自己创建的用户。<br>默认情况下，此选项处于启用状态。</p> <p><b>注意</b>:如果贵组织已载入Adobe Admin Console，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>用户管理员 (所有用户)</strong> </td> 
      <td> <p>允许用户在Workfront中为任何用户执行以下操作：</p> 
       <ul> 
        <li>编辑、删除或停用用户</li> 
        <li>以用户身份登录</li> 
        <li>重置用户的密码</li> 
       </ul> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>用户管理员（组用户）</strong> </td> 
      <td> <p>允许用户对其管理的组中的任何用户执行以下操作： 
        <ul>
         <li><p>编辑、删除或停用用户</p></li>
         <li>以用户身份登录</li>
         <li><p>重置用户的密码</p><p><b>注意</b>:群组管理员无法以登录身份登录或重置Workfront管理员的密码。</p></li>
        </ul><p>默认情况下，此选项处于禁用状态。</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您不想授予群组管理员对其所管理群组的所有成员的访问权限，请禁用上述两个“用户管理”选项。 群组管理员仍可以访问添加到Workfront或在Workfront中向其报告的群组成员。

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

## 按许可证类型访问用户

有关每个访问级别的用户可以对用户执行的操作的信息，请参阅部分 [用户](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
