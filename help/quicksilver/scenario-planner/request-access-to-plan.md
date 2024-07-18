---
product-area: enterprise-scenario-planner-product-area
keywords: 计划、权限、共享、计划、方案、方案、方案
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中请求对计划的访问权限
description: 当您共享指向计划的链接时，您可以在Adobe Workfront Scenario Planner中请求对计划的访问权限。
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 请求访问[!DNL Scenario Planner]中的计划

当计划的链接与您共享时，您可以在[!DNL Adobe Workfront Scenario Planner]中请求对计划的访问权限。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>计划*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>许可证*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]、[！UICONTROL Work]或[！UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td><strong>产品*</strong> </td> 
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[！UICONTROL Scenario Planner]所需的访问权限</a>。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>查看对的访问权限或更高 [!DNL Scenario Planner]</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您拥有什么计划、许可证类型或访问权限，或者贵公司已购买[!DNL Workfront Scenario Planner]，请联系您的[!DNL Workfront]管理员。

## 先决条件

在[!DNL Scenario Planner]中请求访问计划之前，您必须具备以下条件：

* 指向计划的链接。

>[!NOTE]
>
>如果您没有[!DNL Scenario Planner]的访问权限级别权限，并尝试从链接访问计划，则无法请求对该计划的访问权限。 而是显示一个屏幕，通知您联系[!DNL Workfront]管理员。

## 请求访问[!DNL Workfront Scenario Planner]中的计划

如果您还没有对某个计划的权限，并且从与您共享的链接导航到该计划，则会显示一个屏幕，通知您无权查看该计划。 系统会提示您向计划创建者请求权限。

>[!TIP]
>
>您只能向计划的所有者或创建者请求权限。 您无法向也有权访问该计划的其他用户请求权限。

要请求权限，请执行以下操作：

1. 单击指向计划的链接。

   ![](assets/request-access-to-plan-350x277.png)

1. 在&#x200B;**[!UICONTROL 请求访问]**&#x200B;下拉菜单中，指示您希望授予的权限级别。 从以下项中选择：

   * [!UICONTROL 视图]
   * [!UICONTROL 管理]

   您不能请求高于您对[!DNL Scenario Planner]的访问权限级别的权限。 例如，如果您对[!DNL Scenario Planner]具有查看访问权限，则无法请求[!UICONTROL 管理]权限。

   有关不同权限级别的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)中共享计划。

   有关Workfront管理员可以管理对[!DNL Scenario Planner]的访问权限的信息，请参阅[授予对 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的访问权限。

1. （可选）在&#x200B;**[!UICONTROL 留下评论框]**&#x200B;中输入评论或请求，然后单击&#x200B;**[!UICONTROL 请求访问]**。

   会发生以下情况：

   * [!DNL Workfront]向计划所有者发送电子邮件通知，以便他们授予所请求的权限。\
     ![](assets/request-access-to-plan-email-350x156.png)

   * 在计划所有者授予所请求的权限后，如果您的[!DNL Workfront]管理员在您的系统中启用了对象共享到用户通知，并且在您的配置文件中启用了[!UICONTROL 其他人与我共享对象]电子邮件通知，您将收到一封电子邮件，指出已授予权限。

     ![](assets/access-granted-to-plan-email-350x172.png)

   * 您还可以从[!UICONTROL 主页]区域和[!DNL Workfront]移动应用程序向计划授予权限。

   有关启用系统通知的信息，请参阅[为系统中的每个人配置事件通知](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

   有关在配置文件中启用通知的信息，请参阅[通知：其他信息](../workfront-basics/using-notifications/notifications-misc-information.md)。
