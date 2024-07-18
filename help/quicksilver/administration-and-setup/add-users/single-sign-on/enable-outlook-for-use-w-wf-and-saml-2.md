---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 启用Outlook以用于Workfront和SAML 2.0
description: 如果启用SAML 2.0身份验证，并且希望用户能够使用其SAML 2.0凭据从Microsoft Outlook登录到Workfront，则必须启用SAML 2.0以在Office加载项中进行身份验证。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 启用Outlook以用于Workfront和SAML 2.0

如果启用SAML 2.0身份验证，并且希望用户能够使用其SAML 2.0凭据从Microsoft Outlook登录到Workfront，则必须启用SAML 2.0以在Office加载项中进行身份验证。

>[!NOTE]
>
>如果您组织的Workfront实例使用自定义SSO门户，则此项不可用。>
><!--
>or is enabled with Adobe IMS>
>-->
>如果需要更多信息，请咨询您的网络或IT管理员。

## 访问要求

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 启用Outlook以用于Workfront和SAML 2.0

1. 单击全局导航栏上Adobe Workfront右上角附近的&#x200B;**设置**。
1. 单击&#x200B;**系统** > **首选项**。

1. 在&#x200B;**安全性**&#x200B;部分中，确保在Office 365加载项中启用了&#x200B;**允许SAML 2.0身份验证**。

   此选项允许将Workfront嵌入到仅适用于Office 365加载项的Iframe中。 这不会打开点击劫持漏洞，因为其中没有可点击内容。

   此选项默认处于启用状态。

   >[!NOTE]
   >
   >如果启用选项&#x200B;**允许在iframe中嵌入Workfront**，则选项&#x200B;**在Office 365加载项中允许SAML 2.0身份验证**&#x200B;将变暗并启用。
   >
   >![](assets/if-you-enable.png)
   >

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响Workfront中所有用户的体验。
