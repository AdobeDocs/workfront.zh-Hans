---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 按IP地址限制对Adobe Workfront的访问
description: 您可以配置Adobe Workfront 列入允许列表 IP，将对Workfront的访问限制为您指定的75个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 65121fae364683373d2bc9abbe6672755d0cd09c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# 按IP地址限制对Adobe Workfront的访问

>[!IMPORTANT]
>
>此功能当前不适用于已载入Adobe Admin Console的组织。 它将在未来版本的Adobe Admin Console中提供。

您可以配置Adobe Workfront 列入允许列表 IP，将对Workfront的访问限制为您指定的75个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。

这些IP地址或IP地址范围应由网络管理员提供。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 其他允许列表

列入允许列表如果您的防火墙或邮件服务器配置为仅允许某些供应商访问，则必须将某些IP地址添加到其。 这将打开环境与Adobe Workfront服务器之间的通信。 有关信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

此外，如果贵组织使用企业计划，则可以配置Workfront电子邮件允许列表，以控制允许哪些电子邮件域接受来自Workfront的电子邮件，以及哪些电子邮件域可以位于用户在其Workfront用户配置文件中指定的电子邮件地址中。 有关详细信息，请参阅[配置电子邮件允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。

## 将IP地址添加到允许列表

将IP地址添加到Workfront 列入允许列表后，只能使用这些IP地址来访问Workfront。 尝试从其他IP地址访问Workfront的用户会收到错误消息，指示其IP地址被阻止。

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **客户信息。**

1. 列入允许列表 列入允许列表在&#x200B;**IP**&#x200B;部分中，选择&#x200B;**启用IP。**

   默认禁用此选项。

1. 指定当前用于访问Workfront系统的IP地址。

   或

   指定一个IP地址范围，其中包含您当前用于访问Workfront系统的IP地址。

   在启用Workfront之前，必须将用于访问列入允许列表列入允许列表的IP地址添加到。

1. 单击&#x200B;**添加IP范围，**，然后指定您希望能够访问Workfront的IP地址或IP地址范围。
1. （可选）重复上一步以添加其他IP地址或IP地址范围。

   您最多可以添加75个地址或范围。

1. 单击&#x200B;**保存。**
