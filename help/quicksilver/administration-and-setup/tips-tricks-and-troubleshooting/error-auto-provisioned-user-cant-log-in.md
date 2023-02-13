---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误：自动配置的用户无法登录”
description: 如果自动配置的用户首次尝试登录，并收到错误，指出系统没有为他们分配访问级别，这可能是因为您的系统缺少与请求许可证相关联的访问级别。 自动配置使用请求许可证类型，因此您可以通过创建与请求许可证关联的访问级别来解决此问题。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 错误：自动配置的用户无法登录

当自动配置的用户首次尝试登录时，他们会收到以下错误：

## 问题

系统不会为新用户分配访问级别。

默认情况下，自动配置使用请求许可证类型。 当不存在具有请求许可证的访问级别时，系统无法为用户分配访问级别。

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

使用请求许可证创建基本访问级别：

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 访问级别]**.

1. 单击 **[!UICONTROL 新访问级别]**.
1. 输入 **[!UICONTROL 名称]**.
1. 在 **[!UICONTROL 许可证类型]** 下拉菜单中，选择“请求”。
1. 单击 **[!UICONTROL 保存更改]**.

使用请求许可证创建访问级别后，让用户使用其SSO凭据登录。
