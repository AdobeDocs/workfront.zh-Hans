---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 从Web服务接收Webhook
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 从Web服务接收Webhook

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [为没有连接器的Web服务配置webhook](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

如果Web服务当前未在[!DNL Adobe Workfront Fusion]中作为应用程序实施，但它支持发送Webhook，则可以将服务添加到使用自定义Webhook模块作为即时触发器的方案中。

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

## 接收webhook

1. 将&#x200B;**[!UICONTROL Webhook] >[!UICONTROL 自定义webhook]**&#x200B;模块添加到您的方案中。
1. 单击&#x200B;**[!UICONTROL 添加]**，在显示的框中键入&#x200B;**[!UICONTROL Webhook名称]**，然后单击&#x200B;**[!UICONTROL 保存]**。

1. 单击&#x200B;**[!UICONTROL 将地址复制到剪贴板]**，然后单击&#x200B;**[!UICONTROL 确定]**。

1. 登录到Web服务，并在该处执行以下操作：

   1. 在Web服务的[!UICONTROL 设置]区域中，创建一个webhook。
   1. 在步骤3中将您复制的地址粘贴到剪贴板。
   1. 选择将触发webhook的事件。

1. 在[!DNL Workfront Fusion]方案中，指定要触发[!UICONTROL 自定义webhook]模块的一个或多个事件。
1. 运行方案。

   发生一个或多个事件时，[!UICONTROL 自定义webhook]模块将触发并运行方案。
