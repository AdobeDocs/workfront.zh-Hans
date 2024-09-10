---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误：自动设置的用户无法登录”
description: 如果自动配置用户尝试首次登录并收到系统未为他们分配访问级别的错误，这可能是因为您的系统缺少与请求许可证关联的访问级别。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 错误：自动设置的用户无法登录

当自动设置用户尝试首次登录时，他们收到以下错误：

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 问题

系统未为新用户分配访问级别。

默认情况下，自动资源调配使用请求许可证类型。 当不存在具有请求许可证的访问级别时，系统无法为用户分配访问级别。

## 访问要求

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
   <td>[！UICONTROL系统管理员]</td>  
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

使用请求许可证创建基本访问级别：

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 访问级别]**。

1. 单击&#x200B;**[!UICONTROL 新建访问级别]**。
1. 输入&#x200B;**[!UICONTROL 名称]**。
1. 在&#x200B;**[!UICONTROL 许可证类型]**&#x200B;下拉菜单中，选择请求。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。

使用请求许可证创建访问级别后，请让用户使用其SSO凭据登录。


