---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 更改自动配置用户的密码
description: 通常，当新用户尝试更改其临时密码时，他们会输入其电子邮件地址，并收到错误的用户名。 他们必须输入系统分配的用户名，即其全局唯一标识符(GUID)。 由于GUID难以记住和使用，因此我们建议您将新用户的用户名更改为其Workfront邮件地址，然后允许他们更改其密码。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 更改自动配置用户的密码

通过自动配置创建用户时，Adobe Workfront会为用户名分配GUID（全局唯一标识符）。 GUID是随机数和字母的唯一字符串，例如， *5489cb430012526e1ea635e8c29f377f*.

通常，当新用户尝试更改其临时密码时，他们会输入其用户名的电子邮件地址，并收到错误的用户名。 为了让用户更改其密码，他们必须输入系统分配的用户名(GUID)。

由于GUID用户名可能难以使用，因此我们建议您先将用户的用户名更改为其Workfront邮件地址，然后允许他们更改其密码。

>[!TIP]
>
>您可以通过以下方式找到用户的GUID:
>
>* 转到用户的配置文件，并从浏览器的URL复制GUID。
>
>  例如，在URL中 `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`，则需要复制最后两个正斜杠之间的数字和字母字符串： `61941ab1000af22d7104628efa1c738b`.
>
>  有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* 使用“用户”>“GUID”列创建用户报表。 有关更多信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* 查询Workfront API。
>


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

## 更改自动配置用户的密码

1. 通过传递API请求确定用户的GUID用户名，如以下示例所示：

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` 其中 *`<domain>`* 是您公司的域和 *`<ID of User>`* 是用户的Workfront ID。

   您会收到类似于以下内容的响应：

   ![](assets/get-guid.png)

   “username”的返回值是用户的GUID。

1. 使用其GUID作为用户名，更改用户的密码。

   有关更改密码的详细信息，请参阅 [重置密码](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   如果贵组织使用SSO系统，则只有Workfront系统管理员才能更改用户的密码。 有关更多信息，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. 用户登录Workfront后，导航至：

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. 在 **您的登录电子邮件地址** 框中，验证用户的电子邮件地址是否正确，然后单击 **更新帐户**.

   ![](assets/guidusername-350x272.png)

   用户的用户名将更改为其Workfront电子邮件地址。

>[!TIP]
>
>要查找用户的ID，请执行以下操作：
>
>1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).
>
>1. 选择用户。
>
>   此时会打开用户的配置文件页面，其用户ID会显示在URL中。
