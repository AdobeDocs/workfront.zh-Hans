---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 防止欺骗和添加 [!DNL Adobe Workfront] SPF记录
description: 如果用户未收到 [!DNL Adobe Workfront] 电子邮件通知，您需要添加 [!DNL Workfront] SPF记录到防火墙。 您必须与IT团队合作以添加SPF记录。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 防止欺骗和添加 [!DNL Adobe Workfront] SPF记录

## 问题

如果用户未收到 [!DNL Adobe Workfront] 电子邮件通知，您需要添加 [!DNL Workfront] SPF记录到防火墙。 您必须与IT团队合作以添加SPF记录。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

如果您已经将IP地址添加到生产环允许列表境的，如 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 且用户仍然无法接收电子邮件：

1. 将以下SPF记录添加到防火墙：

   *spf.workfront.com*

   这会自动添加所有 [!DNL Workfront] 您防火墙上的允许列表的IP地址，并允许所有垃圾邮件过滤器（使用SPF记录）进行验证 [!DNL Workfront] 服务器作为域的有效发件人。

   >[!NOTE]
   >
   > SPF记录是DNS区域文件的一部分的TXT记录。 我们不支持修改您的DNS区域文件。

1. 必须指定需要配置的SPF记录类型。 这些是SPF记录的有效类型：

   * all(https://dmarcian.com/spf-syntax-table/#all)
   * ip4(https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6(https://dmarcian.com/spf-syntax-table/#ip6)
   * a(https://dmarcian.com/spf-syntax-table/#a)
   * mx(https://dmarcian.com/spf-syntax-table/#mx)
   * ptr(https://dmarcian.com/spf-syntax-table/#ptr)
   * 存在(https://dmarcian.com/spf-syntax-table/#exists)
   * 包括(https://dmarcian.com/spf-syntax-table/#include)

   例如，“v=spf1 a mx包括： [spf.workfront.com](http://spf.workfront.com/) -all”

如果由于公司策略而无法将SPF记录添加到防火墙，请与 [!DNL Workfront] 支持代表。
