---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 启用Outlook以与Workfront和SAML 2.0一起使用
description: 如果您启用SAML 2.0身份验证，并且希望用户能够使用其SAML 2.0凭据从Microsoft Outlook登录Workfront，则必须启用SAML 2.0才能在Office加载项中进行身份验证。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# 启用Outlook以与Workfront和SAML 2.0一起使用

如果您启用SAML 2.0身份验证，并且希望用户能够使用其SAML 2.0凭据从Microsoft Outlook登录Workfront，则必须启用SAML 2.0才能在Office加载项中进行身份验证。

>[!NOTE]
>
>如果贵组织的Workfront实例使用自定义SSO门户，则此功能不可用。>
><!--
>or is enabled with Adobe IMS>
>-->
>如需详细信息，请咨询您的网络或IT管理员。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 启用Outlook以与Workfront和SAML 2.0一起使用

1. 单击 **设置** 在Adobe Workfront的右上角附近。
1. 单击 **系统** > **首选项**.

1. 在 **安全性** 部分，确保 **在Office 365加载项中允许SAML 2.0身份验证**&#x200B;启用。

   此选项仅允许在Iframe中嵌入Office 365加载项的Workfront。 这不会打开点击顶升漏洞，因为不涉及可点击内容。

   默认情况下，此选项处于启用状态。

   >[!NOTE]
   >
   >如果启用选项 **允许在iFrame中嵌入Workfront**，选项 **在Office 365加载项中允许SAML 2.0身份验证** 灰显且处于启用状态。
   >
   >![](assets/if-you-enable.png)

1. 单击&#x200B;**保存**。

   您在此处保存的更改会影响所有用户在Workfront中的体验。
