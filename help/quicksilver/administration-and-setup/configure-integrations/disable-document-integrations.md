---
title: 禁用文档集成
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作为 [!DNL anAdobe] [!DNL Workfront] 管理员，您可以禁用Workfront与任何第三方文档提供程序之间的连接。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 禁用文档集成

作为 [!DNL Adobe] [!DNL Workfront] 管理员，您可以禁用 [!DNL Workfront] 和任何第三方文档提供商。

当您禁用 [!DNL Workfront] 和文档提供商，指向文档的链接会从 [!DNL Workfront]. 用户无法再看到链接的文档，无法通过 [!DNL Workfront] 链接，则无法向该提供商添加更多文档。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 禁用云提供商集成

要禁用 [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. 登录到 [!DNL Workfront] as a [!DNL Workfront] 管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 文档]** > **[!UICONTROL 云提供商]**.

1. 取消选择要断开与的任何云提供程序 [!DNL Workfront].
1. 单击&#x200B;**[!UICONTROL 保存]**。

   用户无法连接到您禁用的特定云提供程序，并且他们无法再将文档从该云提供程序关联到Workfront。

## 禁用 [!DNL SharePoint] 集成

1. 登录到 [!DNL Workfront] as a [!DNL Workfront] 管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 展开 **[!UICONTROL 文档]**，然后单击 **[!UICONTROL [!DNL SharePoint]集成]**.
1. 选择 [!DNL SharePoint] 集成。
1. 单击 **[!UICONTROL 禁用]**.\
   用户无法连接到 [!DNL SharePoint] 网站，且他们无法再链接 [!DNL SharePoint] to [!DNL Workfront].

## 禁用自定义集成

1. 登录到 [!DNL Workfront] 作为管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 文档]** > **[!UICONTROL 自定义集成]**.
1. 选择要禁用的自定义集成。
1. 单击 **[!UICONTROL 禁用]**.

   用户无法连接到您禁用的第三方文档提供程序，并且他们无法再将该云提供程序中的文档链接到 [!DNL Workfront].
