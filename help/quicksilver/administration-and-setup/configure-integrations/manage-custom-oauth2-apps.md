---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: 查看和管理自定义OAuth2应用程序
description: 作为Adobe Workfront管理员，您可以查看和管理Workfront实例的OAuth2应用程序，这些应用程序允许其他应用程序访问Workfront。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# 查看和管理自定义OAuth2应用程序

作为 [!DNL Adobe Workfront] 管理员，您可以查看和管理实例的OAuth2应用程序 [!DNL Workfront]，允许其他应用程序访问 [!UICONTROL Workfront].

>[!NOTE]
>
>* 在OAuth2的上下文中，“Oauth2应用程序”是指应用程序和服务器之间的此类访问链接，例如 [!DNL Workfront]. 有关更多信息，请参阅 [创建OAuth2应用程序 [!DNL Workfront] 集成](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* 您一次最多可以拥有10个OAuth2应用程序。

* 有关创建自定义OAuth2应用程序的信息，请参阅 [创建OAuth2应用程序 [!DNL Workfront] 集成](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* 有关通过用户凭据（授权代码流）配置和使用OAuth2应用程序的说明，请参阅 [使用授权代码流配置并使用贵组织的自定义OAuth 2应用程序](../../wf-api/api/oauth-app-code-token-flow.md).
* 有关使用服务器身份验证（JWT流）配置和使用OAuth2应用程序的说明，请参阅 [使用JWT流配置和使用贵组织的自定义OAuth 2应用程序](../../wf-api/api/oauth-app-jwt-flow.md).
* 有关使用PKCE配置和使用OAuth2应用程序的说明，请参阅 [使用PKCE流程配置和使用贵组织的自定义OAuth 2应用程序](../../wf-api/api/oauth-app-pkce-flow.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL Plan]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 您必须是 [!DNL Workfront] 管理员。 </p>
    <p>有关的信息 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

您必须创建 [!UICONTROL OAuth2] 您组织的应用程序，然后才能查看或管理它们。

有关更多信息，请参阅 [创建OAuth2应用程序 [!DNL Workfront] 集成](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 管理自定义OAuth2应用程序

* [查看和编辑自定义OAuth2应用程序](#view-and-edit-custom-oauth2-applications)
* [删除自定义OAuth2应用程序](#delete-custom-oauth2-applications)

### 查看和编辑自定义OAuth2应用程序 {#view-and-edit-custom-oauth2-applications}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧导航面板中，单击 **[!UICONTROL 系统]**，然后选择 **[!UICONTROL OAuth应用程序]**.
1. 单击 **[!UICONTROL 创建应用程序集成]**.
1. 将鼠标悬停在应用程序上，然后单击 **[!UICONTROL 编辑]** ![](assets/edit-icon.png) 出现在最右边的时候。
1. （可选）编辑应用程序的任何详细信息。

   有关与OAuth2和JWT应用程序相关的字段，请参阅 [创建OAuth2应用程序 [!DNL Workfront] 集成](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### 删除自定义OAuth2应用程序 {#delete-custom-oauth2-applications}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧导航面板中，单击 **[!UICONTROL 系统]**，然后选择 **[!UICONTROL OAuth应用程序]**.
1. 单击** **。
1. 将鼠标悬停在应用程序上，然后单击 **[!UICONTROL 删除]** ![](assets/delete.png) 出现在最右边的时候。

## 在OAuth2应用程序中管理客户端密钥

* [查看客户端密码详细信息](#view-client-secret-details)
* [添加或编辑客户端密钥注释](#add-or-edit-notes-for-client-secret)
* [删除客户端密码](#delete-client-secret)

### 查看客户端密码详细信息 {#view-client-secret-details}

>[!IMPORTANT]
>
>您无法查看客户端密钥本身。 如果您丢失了客户端密钥，则必须将其删除并创建一个新密钥。
>
>* 要删除客户端密钥，请参阅 [删除客户端密码](#delete-client-secret) 本文章中。
>* 要创建新的客户端密钥，请参阅 [创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) 在 [创建OAuth2应用程序 [!DNL Workfront] 集成](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. 单击 *[!UICONTROL *主菜单]**图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧导航面板中，单击 **[!UICONTROL 系统]**，然后选择 **[!UICONTROL OAuth应用程序]**.
1. 将鼠标悬停在应用程序上，然后单击 **[!UICONTROL 编辑]** 图标（当它出现在最右侧时）。
1. 在“客户端密钥”区域查看详细信息：

   * 创建日期
   * 上次使用日期
   * 注释

     要将注释添加到客户端密钥，请参阅 [添加或编辑客户端密钥注释](#add-or-edit-notes-for-client-secret).

### 添加或编辑客户端密钥注释 {#add-or-edit-notes-for-client-secret}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧导航面板中，单击 **[!UICONTROL 系统]**，然后选择 **[!UICONTROL OAuth应用程序]**.
1. 单击 **[!UICONTROL 创建应用程序集成]**.
1. 将鼠标悬停在应用程序上，然后单击 **[!UICONTROL 编辑]** 图标（当它出现在最右侧时）。
1. 找到要添加或编辑注释的客户端密钥。
1. 单击包含客户端密钥详细信息的框。

   您现在可以添加注释文本或编辑现有的注释文本。

   >[!NOTE]
   >
   >注释文本最多可包含64个字符。

1. 单击开箱即用或按 **[!UICONTROL 输入]** 以保存注释文本。

### 删除客户端密码 {#delete-client-secret}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧导航面板中，单击 **[!UICONTROL 系统]**，然后选择 **[!UICONTROL OAuth应用程序]**.
1. 单击 **[!UICONTROL 创建应用程序集成]**.
1. 将鼠标悬停在应用程序上，然后单击 **[!UICONTROL 编辑]** 图标（当它出现在最右侧时）。
1. 找到要删除的客户端密钥。
1. 单击 **[!UICONTROL 删除]** 图标 ![](assets/delete.png) 客户端密码旁边。
