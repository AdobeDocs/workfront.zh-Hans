---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 防止欺骗并添加 [!DNL Adobe Workfront] SPF记录
description: 如果用户没有收到 [!DNL Adobe Workfront] 电子邮件通知，则需要将 [!DNL Workfront] SPF记录添加到防火墙。 您必须与IT团队合作以添加SPF记录。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 防止欺骗并添加[!DNL Adobe Workfront]个SPF记录

## 问题

如果用户没有收到[!DNL Adobe Workfront]电子邮件通知，则需要将[!DNL Workfront]个SPF记录添加到防火墙。 您必须与IT团队合作以添加SPF记录。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是[!DNL Workfront]管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

如果您已按照[配置防火墙的允许列表 列入允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)中的说明将IP地址添加到生产环境的，用户仍不会收到电子邮件：

1. 将以下SPF记录添加到防火墙：

   *spf.workfront.com*

   列入允许列表这会自动将所有[!DNL Workfront]个IP地址添加到防火墙上的中，并允许所有垃圾邮件过滤器（使用SPF记录）将[!DNL Workfront]服务器验证为您的域的有效发件人。

   >[!NOTE]
   >
   > SPF记录是属于DNS区域文件一部分的TXT记录。 不支持修改您的DNS区域文件。

1. 必须指定需要配置的SPF记录类型。 以下是SPF记录的有效类型：

   * 全部(https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * 存在(https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   例如，“v=spf1 a mx include： spf.workfront.com -all”

如果由于公司策略而无法将SPF记录添加到防火墙，请与您的[!DNL Workfront]支持代表合作。
