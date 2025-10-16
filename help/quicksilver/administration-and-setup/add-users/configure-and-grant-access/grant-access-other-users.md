---
title: 授予用户访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中其他用户的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 2%

---


# 授予用户访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中其他用户的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

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
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置对用户的访问权限

您可以使用默认访问级别或您创建的自定义访问级别，管理用户可为其他用户查看和编辑的信息。 具有默认“计划”和“工作”许可证的用户可以查看其他用户的联系信息。 以下任何用户可以创建和编辑其他用户：

* Workfront管理员。

  有关详细信息，请参阅[授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)。

* 具有默认计划许可证的用户，也可以访问用户，如本文所述。

  仅限于查看其公司或主要公司用户的用户有权仅编辑其能够查看的用户。 有关详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 具有默认“计划”许可证的用户，该用户也被指定为另一个用户的经理。

  如果用户被授予其访问级别的用户的“编辑”访问权限，则可以管理向其报告的用户。 有关管理用户的信息，请参阅[查看组织结构图](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)。

* 具有默认计划许可证的用户创建用户后，可以停用、删除或编辑他们创建的用户。 有关创建新用户的信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 配置用户的访问权限以使用自定义访问级别编辑用户

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 要更改拥有计划或工作许可证的用户查看其他用户配置文件的能力，请执行以下操作：

   1. 单击![](assets/gear-icon-settings.png)用户&#x200B;**右侧的**&#x200B;查看&#x200B;**按钮上的齿轮图标**。

   1. 禁用&#x200B;**查看联系信息**，然后单击X以关闭&#x200B;**微调设置**&#x200B;框。

      ![优化用户设置](assets/fine-tune-users.png)

1. 要修改具有计划许可证访问权限的用户编辑其他用户的能力，请单击![](assets/gear-icon-settings.png)用户&#x200B;**右侧的**&#x200B;编辑&#x200B;**按钮上的齿轮图标**，然后选择要授予的功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>创建</strong> </td> 
      <td> <p>允许用户创建用户。<br>默认启用此选项。</p> 
     <p><b>注意</b>：如果您的组织已登记到Adobe Admin Console，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。</p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>删除</strong> </td> 
      <td> <p> 允许用户删除他们自己创建的用户。<br>默认启用此选项。</p> <p><b>注意</b>：如果您的组织已登记到Adobe Admin Console，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>用户管理员（所有用户）</strong> </td> 
      <td> <p>允许用户对Workfront中的任意用户执行以下操作：</p> 
       <ul> 
        <li>编辑、删除或停用用户</li> 
        <li>以用户身份登录<p><b>注意</b>：您无法作为系统管理员的任何用户登录。</p></li> 
        <li>重置用户密码</li> 
       </ul> <p>默认禁用此选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>用户管理员（组用户）</strong> </td> 
      <td> <p>允许用户为其管理的组中的任何用户执行以下操作： 
        <ul>
         <li><p>编辑、删除或停用用户</p></li>
         <li>以用户身份登录</li>
         <li><p>重置用户密码</p><p><b>注意</b>：组管理员无法以Workfront管理员身份登录或重置密码。</p></li>
        </ul><p>默认禁用此选项。</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您不想向组管理员授予他们管理的组的所有成员的访问权限，请禁用上述两个“用户管理员”选项。 组管理员仍可以访问他们添加到Workfront的组成员或在Workfront中向他们报告的组成员。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

## 按许可证类型访问用户

有关每个访问级别中的用户可以对用户执行哪些操作的信息，请参阅[适用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users)一文中的[用户](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)部分。
