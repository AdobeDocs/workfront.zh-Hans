---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 访问级别中缺少外部用户许可证类型
description: 在“设置”的“访问级别”下，我无法再看到“外部用户”许可证类型。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 访问级别中缺少外部用户许可证类型

## 问题

在“设置”的“访问级别”下，我无法再看到“外部用户”许可证类型。

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

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**.

1. 在 **[!UICONTROL 安全性]** 部分，确保选项 **[!UICONTROL 使用Workfront帐户以外的人员的电子邮件地址与他们协作]** 启用。

   如果未启用此选项，则外部用户不会显示在访问级别设置中。
