---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 更改Adobe Workfront域
description: 作为Adobe Workfront管理员和授权的Workfront支持联系人，您可以请求Workfront支持团队提供帮助以更改贵组织的Workfront域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 更改Adobe Workfront域

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>要更改您的Adobe Workfront域(如果贵组织已载入Adobe Admin Console)，请参阅 [设置域](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作为Adobe Workfront管理员和授权的Workfront支持联系人，您可以请求Workfront支持团队提供帮助以更改贵组织的Workfront域。

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 请求域更改

1. 单击 **支持** 选项卡，然后开始创建支持案例。
1. 在 **描述** 框中，包含您需要的新域，以及您希望新域上线的时间范围。
1. 完成支持案例的盒子填写，然后单击 **提交**.

您还可以致电Workfront支持，以获取更改域的帮助。

## 如果您是SSO客户，请更新新域

如果贵公司使用单点登录(SSO)，则在更改Workfront域后，需要执行以下步骤。

>[!NOTE]
>
>如果贵组织的Workfront实例通过Adobe IMS启用，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧边栏中，单击 **系统** > **客户信息** 并确保您的域已在客户信息页面上更新。

1. 在左侧边栏中，单击 **系统** > **单点登录(SSO)**.

1. 单击 **下载SAML 2.0元数据**.
1. 下载文件后，将其打开，并确保满足以下条件：

   1. **entityID** 指向新域。
   1. 内的所有位置 **`<md:AssertionConsumerService>`** 指向新域。

1. 将下载的元数据文件提供给您的身份提供程序，以便他们能够在其末尾更新该文件。
1. 确保已针对贵组织使用的所有Workfront集成更新域。
