---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置电子邮件允许列表
description: 如果您的组织使用WorkfrontEnterprise计划，您可以创建一个Workfront电子邮件允许列表，以控制允许哪些电子邮件域接受来自Workfront的电子邮件，以及哪些电子邮件域可以位于用户在其用户配置文件中指定的电子邮件地址中。 如果贵组织的安全策略限制用户将Workfront中存储的数据发送到外部电子邮件地址，则可以使用此功能；为确保遵循此策略，可以在允许列表中仅包含您的内部公司域。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 配置电子邮件允许列表

如果您的组织使用Workfront企业计划，则可以创建Workfront电子邮件允许列表来控制：

* 允许哪些电子邮件域接受来自Workfront的电子邮件。
* 用户在用户配置文件中指定的电子邮件地址中可以包含哪些电子邮件域。

如果贵组织的安全策略限制用户将Workfront中存储的数据发送到外部电子邮件地址，则可以使用此功能；为确保遵循此策略，可以在允许列表中仅包含您的内部公司域。

>[!IMPORTANT]
>
>您的IT团队应确保`notifications@my.workfront.com`传入的电子邮件在您的组织系统中未被阻止。
>
>来自Workfront的所有电子邮件都从该地址发送，以提高电子邮件的成功投放并消除电子邮件的欺骗。 这包括自动警报和用户到用户的通信。
>
>例如，您从名为Joan Harris的用户那里收到的Workfront电子邮件中的“发件人”行如下所示：
>`Joan Harris <notifications@my.workfront.com>`

有关配置组织的防火墙以打开环境与Adobe Workfront服务器之间的通信的信息，请参阅[配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。 有关详细信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 其他允许列表

如果贵组织拥有企业计划，则可以配置Adobe Workfront 列入允许列表 IP，将对Workfront的访问权限限制为您指定的45个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。 有关详细信息，请参阅[通过IP地址限制对Adobe Workfront的访问](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)。

此外，如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须将某些IP地址添加到其IP允许列表。 这将打开环境与Adobe Workfront服务器之间的通信。 有关信息，请参阅[配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 配置电子邮件允许列表

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **客户信息**。
1. 列入允许列表 列入允许列表在&#x200B;**电子邮件**&#x200B;部分中，选择&#x200B;**启用域**，然后单击&#x200B;**添加域**。
1. 在显示的框中，键入要允许的域，如`ourcompany.com`，然后单击&#x200B;**添加域**。
1. 重复上一步骤以添加任何其他要允许的域。
1. 完成后，单击&#x200B;**保存**。
