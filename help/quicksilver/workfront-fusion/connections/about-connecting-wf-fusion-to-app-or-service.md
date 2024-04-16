---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 连接概述
description: 对于大多数应用程序，需要创建一个连接，通过它 [!DNL Adobe Workfront Fusion] 可根据特定场景的设置与给定的第三方服务进行通信。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 连接概述

<!-- Audited: 3/2024-->

对于大多数应用程序， [!DNL Workfront Fusion] 需要连接，通过该连接可以根据特定场景的设置与给定的第三方服务通信。

例如，如果要创建一个方案，以从中检索信息 [!DNL Workfront]，则必须授予访问权限 [!DNL Workfront Fusion] 以访问 [!DNL Workfront] 帐户。

连接表示Fusion用于访问应用程序的授权和权限。 您可以为每个应用程序创建一个或多个连接，并可以在多个模块或方案中使用相同的连接。

大多数连接只用于单个应用程序。 例如， [!DNL Workfront] 连接不能用于 [!UICONTROL Salesforce] 模块。 部分 [!DNL Adobe] 应用程序可以共享连接。 有关详细信息，请参阅中列出的这些应用程序的文章 [应用程序及其模块](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

连接是在团队级别管理的。 团队的所有成员都可以访问团队的连接，而团队外部的用户无权访问团队的连接。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p><p>或</p><p>当前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 计划：您的组织必须购买 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 计划： [!DNL Workfront Fusion] 中包含。</li></ul>
   <p>或</p>
   <p>当前：您的组织必须购买 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 访问权限

对于每一个连接， [!DNL Workfront Fusion] 仅需要那些成功完成给定方案所需的访问权限。 例如，如果您创建一个方案以列出文档 [!DNL Google Docs]， [!DNL Workfront Fusion] 不要求获取文档内容的权限。 之后，如果您发现您需要访问文档的内容，则可以更新连接或创建一个可访问该内容的新连接。

并非所有服务都允许您限制对特定任务的访问。 在这些情况下， [!DNL Workfront Fusion] 必须要求完全访问权限。 有关如何限制的详细信息 [!DNL Workfront Fusion] 访问您在这些服务上注册的帐户，请参阅中列出的特定于应用程序的文档 [应用程序及其模块](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## 管理连接

您可以从以下位置管理所有连接： [!UICONTROL 连接] 区域。

>[!NOTE]
>
>连接由团队拥有。 如果找不到要查找的连接，请检查您查看的是正确的团队。
>
>要选择新团队，请执行以下操作：
>
>* 单击左侧导航中的团队名称并选择新团队。
>
>    或
>
>* 单击左侧导航中的团队概述，然后单击页面顶部附近的团队名称旁边的下拉箭头。 选择新团队。

1. 打开 [!UICONTROL 连接] 区域，单击 <b>[!UICONTROL 连接]</b> 在左侧导航中。
1. （可选）单击环境和类型下拉列表并选择一个选项，以指示连接的环境和类型。
1. （可选）查看授予哪些权限 [!DNL Workfront Fusion] 对于连接，单击查看图标 ![查看连接权限](assets/view-connection-permissions.png) 用于该连接。
1. （可选）要重命名连接，请突出显示连接名称并键入新名称。
1. （可选）要重新授权连接，请单击 **重新授权** 用于该连接。
1. （可选）要删除连接，请单击 **删除** 用于该连接。
1. （可选）要验证是否成功建立了与服务的连接，请单击 **验证** 用于连接。



## 续订连接

[!DNL Workfront Fusion] 通常会在无限制的时段内获得对给定服务的访问权限。 某些应用程序要求在一定时间段后续订访问权限。 在这些情况下， [!DNL Workfront Fusion] 在访问权限过期前不久，通过电子邮件通知您。

要续订连接，请执行以下操作：

1. 单击 **[!UICONTROL 重新授权]** 中的按钮 **[!UICONTROL 连接]** 区域。
