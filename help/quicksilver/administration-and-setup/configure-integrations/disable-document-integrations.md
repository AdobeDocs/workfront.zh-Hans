---
title: 禁用文档集成
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作为 [!DNL anAdobe] [!DNL Workfront]管理员，您可以禁用Workfront与任何第三方文档提供商之间的连接。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 2%

---

# 禁用文档集成

作为[!DNL Adobe] [!DNL Workfront]管理员，您可以禁用[!DNL Workfront]与任何第三方文档提供商之间的连接。

当您禁用[!DNL Workfront]与文档提供程序之间的连接时，指向文档的链接从[!DNL Workfront]中消失。 用户无法再查看链接的文档，也无法通过[!DNL Workfront]链接对文档进行任何更改，也无法向该提供程序添加更多文档。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table>
  <tr>
   <td>Adobe Workfront包
   </td>
   <td> <p>Prime或Ultimate</p>
    <p>工作流 Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront许可证
   </td>
   <td><p>标准</p>
   <p>规划</p>
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td>您必须是[!DNL Workfront]管理员。
   </td>
  </tr>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 禁用云提供程序集成

要禁用[!UICONTROL Workfront DAM]、[!DNL Box]、[!DNL Dropbox]、[!DNL Google Drive]、[!DNL Microsoft OneDrive]、[!DNL WebDAM]的文档集成：

1. 以[!DNL Workfront]管理员身份登录[!DNL Workfront]。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 云提供商]**。

1. 取消选择您要从[!DNL Workfront]断开连接的任何云提供程序。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   用户无法连接到您禁用的特定云提供商，并且他们无法再将来自该云提供商的文档链接到Workfront。

## 禁用[!DNL SharePoint]集成

1. 以[!DNL Workfront]管理员身份登录[!DNL Workfront]。

{{step-1-to-setup}}

1. 展开&#x200B;**[!UICONTROL 文档]**，然后单击&#x200B;**[!UICONTROL [!DNL SharePoint]集成]**。
1. 选择要禁用的[!DNL SharePoint]集成。
1. 单击&#x200B;**[!UICONTROL 禁用]**。\
   用户无法连接到您已禁用的[!DNL SharePoint]站点，并且他们不能再将文档从[!DNL SharePoint]链接到[!DNL Workfront]。

## 禁用自定义集成

1. 以管理员身份登录到[!DNL Workfront]。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 自定义集成]**。
1. 选择要禁用的自定义集成。
1. 单击&#x200B;**[!UICONTROL 禁用]**。

   用户无法连接到您禁用的第三方文档提供商，并且他们无法再从该云提供商将文档链接到[!DNL Workfront]。
