---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 基于平台的管理差异(Adobe Workfront/Adobe业务平台)
description: 如果贵组织已载入Adobe业务平台，则用户可使用Adobe业务平台访问Adobe Workfront。 这意味着用户管理主要通过Adobe Admin Console完成，而单点登录(SSO)则通过Adobe业务平台而不是Workfront进行处理。 作为Adobe Workfront管理员，您的管理职责和程序因贵组织是否已载入Adobe业务平台而异。 本文列出了必须以不同方式处理的过程，以及指向Workfront和Adobe Admin Console说明的链接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# 基于平台的管理差异(Adobe Workfront/Adobe业务平台)

如果贵组织已载入Adobe业务平台，则用户可使用Adobe业务平台访问Adobe Workfront。 这意味着：

* 用户管理主要通过Adobe Admin Console完成
* 单点登录(SSO)通过Adobe业务平台进行处理，而不是通过Workfront进行处理

作为Adobe Workfront管理员，您的管理职责和程序因贵组织是否已载入Adobe业务平台而异。 本文列出了必须以不同方式处理的过程，以及指向Workfront和Adobe Admin Console说明的链接。

## 用户

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>操作</th> 
   <th>有关Workfront中的说明，请参阅</th> 
   <th>有关Adobe管理控制台中的说明，请参阅</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">授予用户管理员访问权限</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>中的“编辑用户详细信息”部分 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">单独管理用户</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">将用户添加到Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">添加用户</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">在Adobe Admin Console中管理用户</a> </p> </li> 
     <li> <p>中的“添加用户”部分 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">单独管理用户</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">停用用户</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新激活用户</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">单独管理用户</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">删除用户</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">删除用户</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>中的“永久删除用户”部分 <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">管理目录用户</a>
     </p><p>注意：从 [!DNL Adobe Admin Console] 停用 [!DNL Workfront]，但不会从中删除它们 [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">编辑用户配置文件</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">单独管理用户</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">批量编辑用户配置文件</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">批量编辑用户配置文件</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>中的“编辑用户详细信息”部分 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">批量CSV上传</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">导入用户 </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">导入用户</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>中的“添加用户”部分 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">批量CSV上传</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">以其他用户身份登录</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">以其他用户身份登录</a> </p> </li> 
    </ul> </td> 
   <td>不可用</td> 
  </tr> 
  <tr> 
   <td role="rowheader">续订SAML证书</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">续订Adobe Workfront SAML 2.0元数据证书</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>“SAML响应中的数字签名未验证……”部分 in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">疑难解答Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO（单点登录）

由于Adobe业务平台控制用户的单点登录(SSO)，因此以下操作和功能可通过Adobe业务平台自动处理。 如果贵组织尚未载入Adobe业务平台，则必须在Workfront中执行这些操作。


* [使用SAML 2.0配置Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [使用ADFS使用SAML 2.0配置Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [停用Adobe Workfront中的单点登录](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [在您的身份提供程序中更新SAML 2.0元数据](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [更新用户以进行单点登录](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [配置密码策略以进行身份验证](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [配置系统安全首选项](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
