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
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# 按IP地址限制对Adobe Workfront的访问

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release. -->

您可以配置Adobe Workfront 列入允许列表 IP，将对Workfront的访问限制为您指定的75个IP地址或IP地址范围。 这为Workfront应用程序提供了额外的安全层。

这些IP地址或IP地址范围应由网络管理员提供。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
