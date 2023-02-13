---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 按IP地址限制对Adobe Workfront的访问
description: 您可以配置Adobe Workfront IP，允许列表以将对Workfront的访问限制为您指定的45个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 按IP地址限制对Adobe Workfront的访问

您可以配置Adobe Workfront IP，允许列表以将对Workfront的访问限制为您指定的45个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。

这些IP地址或IP地址范围应由网络管理员提供。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>企业</p> </td> 
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

## 其他允许列表

如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须向其添加特定IP地允许列表址。 这将打开您的环境与Adobe Workfront服务器之间的通信。 有关该信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

此外，如果贵组织使用企业计划，则可以配置Workfront电子邮件允许列表，以控制允许哪些电子邮件域接受来自Workfront的电子邮件，以及哪些电子邮件域可以位于用户在其Workfront用户配置文件中指定的电子邮件地址中。 有关更多信息，请参阅 [配置电子邮件允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## 向添加IP地允许列表址

将IP地址添加到Workfront允许列表后，只能使用这些IP地址访问Workfront。 尝试从其他IP地址访问Workfront的用户会收到一条错误消息，指示其IP地址被阻止。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **客户信息。**

1. 在 **IP允许列表** 选择 **启用IP允许列表。**

   默认情况下，此选项处于禁用状态。

1. 指定您当前用于访问Workfront系统的IP地址。

   或

   指定IP地址范围，其中包括您当前用于访问Workfront系统的IP地址范围。

   必须先将您用于访问Workfront的IP地址添加到允许列表，然后才允许列表能启用该。

1. 单击 **添加IP范围、** 然后，指定您希望能够访问Workfront的IP地址或IP地址范围。
1. （可选）重复上一步骤以添加其他IP地址或IP地址范围。

   您最多可以添加45个地址或范围。

1. 单击 **保存。**
