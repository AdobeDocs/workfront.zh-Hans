---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置电子邮件允许列表
description: 如果贵组织使用WorkfrontEnterprise计划，则可以创建Workfront电子邮件允许列表，以控制允许哪些电子邮件域接受来自Workfront的电子邮件以及哪些电子邮件域可以位于用户在其用户配置文件中指定的电子邮件地址中。 如果贵组织的安全策略限制用户将存储在Workfront中的数据发送到外部电子邮件地址，则此策略非常有用，因为您只能在“”中包允许列表含您的内部公司域，以确保遵循此策略。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 配置电子邮件允许列表

如果贵组织使用WorkfrontEnterprise计划，则可以创建Workfront电子邮件允许列表以控制：

* 允许哪些电子邮件域接受来自Workfront的电子邮件。
* 哪些电子邮件域可以位于用户在其用户配置文件中指定的电子邮件地址中。

如果贵组织的安全策略限制用户将存储在Workfront中的数据发送到外部电子邮件地址，则此策略非常有用，因为您只能在“”中包允许列表含您的内部公司域，以确保遵循此策略。

>[!IMPORTANT]
>
>您的IT团队应确保从 `notifications@my.workfront.com` 在您组织的系统中未被阻止。
>
>所有来自Workfront的电子邮件都从该地址发送，以增加成功的电子邮件投放，并消除电子邮件欺骗。 这包括自动警报和用户与用户的通信。
>
>例如，您从名为Joan Harris的用户那里收到的Workfront电子邮件中的“发件人”行将如下所示：
>
```
>Joan Harris <notifications@my.workfront.com>
>```

有关配置贵组织的防火墙以打开环境与Adobe Workfront服务器之间的通信的信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td> <p>您必须是Workfront管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 其他允许列表

如果贵组织具有企业计划，则可以配置Adobe Workfront IP允许列表，以将对Workfront的访问限制为您指定的45个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。 有关更多信息，请参阅 [按IP地址限制对Adobe Workfront的访问](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

此外，如果防火墙或邮件服务器配置为仅允许访问某些供应商，则必须将某些IP地址添加到其允许列表。 这将打开您的环境与Adobe Workfront服务器之间的通信。 有关该信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 配置电子邮件允许列表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **客户信息**.

1. 在 **电子邮件允许列表** 选择 **启用域允许列表**，然后单击 **添加域**.
1. 在显示的框中，键入要允许的域，例如 `ourcompany.com`，然后单击 **添加域**.

1. 重复上一步骤以添加任何其他要允许的域。
1. 完成后，单击 **保存**.
