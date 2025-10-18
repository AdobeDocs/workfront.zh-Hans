---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 更改自动设置用户的密码
description: 建议您将新用户的用户名更改为其Workfront邮件地址，然后允许他们更改密码。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 更改自动设置用户的密码

通过自动配置创建用户时，Adobe Workfront会为用户名分配一个GUID（全局唯一标识符）。 GUID是随机数字和字母的唯一字符串，例如&#x200B;*5489cb430012526e1ea635e8c29f377f*。

通常，当新用户尝试更改其临时密码时，他们会输入其电子邮件地址作为用户名，并收到错误用户名消息。 用户要更改密码，必须输入系统分配的用户名（即GUID）。

由于GUID用户名可能很难使用，因此我们建议您先将用户的用户名更改为其Workfront邮件地址，然后允许他们更改密码。

>[!TIP]
>
>您可以通过以下方式查找用户的GUID：
>
>* 转到用户的配置文件，然后从浏览器的URL中复制GUID。
>
>  例如，在URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`中，您应该复制最后两个正斜杠`61941ab1000af22d7104628efa1c738b`之间的数字和字母字符串。
>
>  有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。
>
>* 创建包含用户> GUID列的用户报告。 有关详细信息，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。
>
>* 查询Workfront API。
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 更改自动设置用户的密码

1. 通过传递API请求确定用户的GUID用户名，如以下示例所示：

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>`其中&#x200B;*`<domain>`*&#x200B;是您公司的域，*`<ID of User>`*&#x200B;是用户的Workfront ID。

   您会收到类似于以下内容的响应：

   ![获取GUID](assets/get-guid.png)

   返回“username”即是用户的GUID。

1. 使用其GUID作为用户名，更改用户的密码。

   有关更改密码的详细信息，请参阅[重置密码](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md)。

   如果您的组织使用SSO系统，则只有Workfront系统管理员可以更改用户的密码。 有关详细信息，请参阅[Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. 用户登录Workfront后，导航至：

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. 在&#x200B;**登录电子邮件地址**&#x200B;框中，验证用户的电子邮件地址是否正确，然后单击&#x200B;**更新帐户**。

   ![用户名](assets/guidusername-350x272.png)

   用户的用户名已更改为其Workfront电子邮件地址。

>[!TIP]
>
>要查找用户的ID，请执行以下操作：
>
>1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**用户** ![用户图标](assets/users-icon-in-main-menu.png)。
>
>1. 选择用户。
>
>   此时，将打开用户的配置文件页面，并在该URL中显示其用户ID。
>
