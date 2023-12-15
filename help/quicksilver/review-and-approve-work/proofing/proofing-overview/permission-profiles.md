---
content-type: overview
product-area: documents
keywords: 验证，权限
navigation-topic: proofing-overview
title: 校对权限配置文件概述
description: 验证权限配置文件确定用户在您帐户的所有验证中拥有的整体权限。 验证权限配置文件会分配给其用户配置文件中的用户。 验证权限配置文件与验证角色不同。
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# 校对权限配置文件概述

<!--Audited: 12/2023-->

验证权限配置文件确定用户在您帐户的所有验证中拥有的整体权限。 验证权限配置文件会分配给其用户配置文件中的用户。

验证权限配置文件与验证角色不同。 有关校对角色的更多信息，请参阅 [验证角色概述](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>如果您是管理员，则可以为组织中的用户创建自定义配置文件。 有关更多信息，请参阅 [在Workfront Proof中配置自定义配置文件](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## 校对权限配置文件

下表显示每个验证权限配置文件的可用权限。

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>拥有的项目</strong>
   </td>
   <td colspan="3" ><strong>其他用户的项目</strong>
   </td>
   <td><strong>管理员</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>添加</strong>
   </td>
   <td><strong>视图</strong>
   </td>
   <td><strong>编辑</strong>
   </td>
   <td><strong>删除</strong>
   </td>
   <td><strong>视图</strong>
   </td>
   <td><strong>编辑</strong>
   </td>
   <td><strong>删除</strong>
   </td>
   <td><strong>编辑和删除</strong>
   </td>
  </tr>
  <tr>
   <td>管理员
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>监督人
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>管理器
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### 管理员

管理员有权访问 [帐户设置](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) 并具有以下权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>管理员可以：</td> 
   <td>管理员无法：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>创建校样、上传文件和创建文件夹</p> </li> 
     <li> <p>查看、编辑和删除校样及其创建的文件</p> </li> 
     <li> <p>查看、编辑和删除由组织中的所有用户创建的验证和文件</p> </li> 
     <li> <p>删除其他用户的公共文件夹</p> </li> 
     <li> <p>编辑帐户中创建的所有验证</p> </li> 
     <li> <p>被设置为Dropzone所有者*</p> </li> 
     <li> <p>访问“帐户设置”页面并编辑帐户详细信息</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
     <li> <p>添加、编辑和删除用户</p> </li> 
     <li> <p>创建组并添加新联系人</p> </li> 
     <li> <p>删除联系人</p> </li> 
     <li> <p>如果校样上没有回复，则编辑校样</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>编辑校对回复。</p> </li> 
     <li> <p>删除其他用户的专用文件夹</p> </li> 
     <li> <p>访问“计费”页面或编辑计费详细信息</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;仅在Workfront Proof独立产品中可用。

### 监督人

主管具有以下权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>主管可以：</td> 
   <td>主管不能：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>创建校样、上传文件和创建文件夹</p> </li> 
     <li> <p>查看、编辑和删除校样及其创建的文件</p> </li> 
     <li> <p>查看、编辑和删除由组织中的所有用户创建的验证和文件</p> </li> 
     <li> <p>删除其他用户的公共文件夹</p> </li> 
     <li> <p>编辑帐户中创建的所有验证</p> </li> 
     <li> <p>创建组并添加新联系人</p> </li> 
     <li> <p>删除联系人</p> </li> 
     <li> <p>如果校样上没有回复，则编辑校样</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>编辑校对回复。</p> </li> 
     <li> <p>删除其他用户的专用文件夹</p> </li> 
     <li> <p>访问“计费”页面或编辑计费详细信息</p> </li> 
     <li> <p>添加、编辑或删除用户</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 管理器

经理具有以下权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>经理可以：</td> 
   <td>经理不能：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>创建校样、上传文件和创建文件夹</p> </li> 
     <li> <p>查看、编辑和删除校样及其创建的文件</p> </li> 
     <li> <p>查看、审阅和批准其他用户明确与其共享的验证（对共享文件夹中所有内容的只读权限）</p> </li> 
     <li> <p>编辑帐户中创建的所有验证</p> </li> 
     <li> <p>创建组并添加新联系人</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>查看、编辑或删除由组织中的其他用户创建的验证和文件。 </p> </li><li><p>编辑校对回复。</p> </li> 
     <li> <p>删除其他用户的专用或公共文件夹</p> </li> 
     <li> <p>访问“计费”页面或编辑计费详细信息</p> </li> 
     <li> <p>添加、编辑或删除用户</p> </li> 
     <li> <p> 删除联系人</p> </li> 
     <li> <p>清空垃圾桶</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
