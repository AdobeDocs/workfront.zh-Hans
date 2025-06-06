---
title: '为Outlook启用 [!DNL Adobe Workfront] '
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 在用户可以开始使用 [!DNL Adobe Workfront] for Outlook之前，首先需要为您的系统启用它。
author: Lisa, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: be523b27-191f-46ca-9a87-d512f9a15a1e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# 启用 [!DNL Adobe Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。
>
>* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**
>
>作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**


在用户可以开始使用[!DNL Adobe Workfront for Outlook]之前，您首先需要为您的系统启用它。

有关启用后如何使用[!DNL Workfront for Outlook]的信息，请参阅[[!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/workfront-for-outlook.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

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
   <td>[!UICONTROL 计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。 有关[!DNL Workfront]管理员的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

+++

## 启用[!DNL Workfront] [!DNL Outlook]加载项

1. 以管理员身份登录到[!DNL Workfront]。

{{step-1-to-setup}}

1. 展开&#x200B;**[!UICONTROL 系统]**，然后单击&#x200B;**[!UICONTROL 首选项]**。

1. 确保&#x200B;**[!UICONTROL 允许人员使用Workfront的移动应用程序，并且已选择[!DNL Workfront] [!DNL Outlook]加载项]**。\
   除了允许使用[!DNL Workfront]移动设备应用程序之外，此设置还允许使用[!DNL Workfront] [!DNL Outlook]加载项。

   此选项默认处于启用状态。

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 正在安装[!DNL Workfront] [!DNL Outlook]加载项

有关为[!DNL Outlook]使用[!DNL Workfront]加载项的系统要求的信息，请参阅[为 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)设置Adobe Workfront中的[系统要求](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#system-requirements-and-prerequisites)。

有关如何为[!DNL Outlook]安装[!DNL Workfront]加载项的信息，请参阅[设置 [!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)中的[安装加载项](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#downloading-and-installing-the-add-in)。
