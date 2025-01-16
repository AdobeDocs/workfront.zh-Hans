---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: connections-annd-webhooks
title: 创建与 [!DNL Adobe Workfront Fusion] 的连接 — 基本说明
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [创建连接 — 基本说明](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-fusion-general.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 创建连接

要在[!DNL Workfront Fusion]模块内创建连接，请执行以下操作：

1. 单击[!UICONTROL 连接]框旁边的&#x200B;**[!UICONTROL 添加]**&#x200B;以打开&#x200B;**[!UICONTROL 创建连接]**&#x200B;面板。
1. （可选）更改默认&#x200B;**[!UICONTROL 连接名称]**。
1. （有条件）如果应用程序需要高级连接设置（如ID、密钥或[!UICONTROL 密钥]），请输入该信息。

   您可能需要单击&#x200B;**[!UICONTROL 显示高级设置]**&#x200B;以显示可在其中输入此类信息的字段。

1. 单击&#x200B;**[!UICONTROL 继续]**。
1. 在显示的登录窗口中，输入您的凭据以登录应用程序（如果尚未登录）。
1. （视情况而定）如果显示&#x200B;**[!UICONTROL 允许]**&#x200B;按钮，请检查连接器能够执行的操作，然后单击按钮以将应用程序连接到[!DNL Workfront Fusion]。

   >[!NOTE]
   >
   >某些Microsoft应用程序使用相同的连接，该连接与单个用户权限相关联。 因此，在创建连接时，权限同意屏幕除了显示当前应用程序所需的任何新权限外，还会显示以前授予此用户连接的任何权限。
   >
   >例如，如果用户拥有通过Excel Connector授予的“读取表”权限，然后在Outlook Connector中创建连接以读取电子邮件，则权限同意屏幕将显示已授予的“读取表”权限和新要求的“写入电子邮件”权限。