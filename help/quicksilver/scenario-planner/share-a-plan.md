---
product-area: enterprise-scenario-planner-product-area
keywords: 计划、权限、共享、计划、方案、方案、方案
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中共享计划
description: 您可以将在Adobe Workfront Scenario Planner中创建的计划与其他用户共享。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 在[!DNL Scenario Planner]中共享计划

您可以与其他用户共享[!DNL Adobe Workfront Scenario Planner]中的计划，这样他们便可以就您所做的相同工作进行协作。

>[!TIP]
>
>如果您将指向计划的链接发送给其他人，则还必须与他们共享该计划，以便他们能够查看该计划。

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
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[！UICONTROL Edit]访问 [!DNL Scenario Planner]</p> <p>如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p> [！UICONTROL Manage]对计划的权限
     <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[！UICONTROL请求]对[!DNL Scenario Planner]</a>中计划的访问权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 授予计划权限的用户必须有权访问其访问级别中的[!DNL Scenario Planner]区域（由您的[!DNL Workfront]管理员授予），才能获得对计划的权限。

  例如，[!UICONTROL 请求者]无法查看、创建或编辑计划。 在与拥有请求者许可证的用户共享计划时，您应牢记这一点。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

有关各种许可证类型对[!DNL Scenario Planner]的访问权限的详细信息，请参阅[授予对 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的访问权限。

## 有关计划共享的注意事项

* 您可以共享单个计划，也可以批量共享多个计划。
* 您无法查看未创建或未与您共享的计划。
* 您只能与其他用户共享计划。 您无法与组、团队或公司共享计划。
* 必须先保存计划，然后才能共享它。
* 您可以与其他用户共享计划的URL。 如果用户没有权限至少查看计划，则可以在收到URL时向其他用户请求对计划的访问权限。 有关请求访问计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)中请求访问计划。
* 在共享已与其他人共享的多个计划时，与您共享的用户不会替换，而是会添加到您选择的每个计划的现有用户。

## 共享计划

1. 单击Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 方案]**。
1. 单击计划的名称以将其打开

   或

   选择多个计划以批量共享它们。

   >[!TIP]
   >
   >您可以通过单击在计划标题右上角与计划共享的用户头像来共享计划。

1. （视情况而定）如果您打开了计划，请单击[!UICONTROL 计划]名称右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;图标![](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 共享]**

   或

   如果选择多个计划来批量共享它们，请单击计划列表顶部的&#x200B;**[!UICONTROL 共享]**&#x200B;图标![](assets/share-icon-26x26.png)以打开[!UICONTROL 计划]访问框。

   >[!TIP]
   >
   >* 对您选择的所有计划具有权限的用户将显示在[!UICONTROL 计划]访问框中。
   >* 任何其他用户都会添加到所有选定计划中，而不会替换现有用户。

1. 在&#x200B;**[!UICONTROL 将计划访问权限授予]**&#x200B;字段中，开始键入要与其共享计划的用户的名称，然后在用户出现在列表中时将其选定。
1. 从用户名右侧的权限下拉菜单中，选择要向计划授予的权限级别。
1. 从以下项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL视图]</td> 
      <td>与共享计划的用户将有权查看计划。 他们无法编辑有关计划的信息、添加计划、方案或发布方案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL管理]</td> 
      <td> <p>您共享计划的用户具有管理计划的权限，其中包括编辑信息、添加计划、方案和发布计划。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >只有在创建计划后，您才可以删除计划。 不能删除与您共享的计划。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   计划现在与您指定的用户共享。

   您可以在计划列表或与我共享列或计划标题右上角查看对计划具有权限的用户。

   >[!TIP]
   >
   >您可以通过在计划列表中应用[!UICONTROL 与我共享]筛选器来查看与您共享的计划。

## 计划权限选项

下表列出了共享计划时可以授予的权限。 有关用户根据其许可证获得的访问权限的详细信息，请参阅[授予访问权限 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>操作</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL管理]</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL视图]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>查看计划 </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看计划 </p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>查看方案</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ <span style="font-weight: normal;"></span> </td> 
  </tr> 
  <tr> 
   <td>查看职位角色</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>查看成本和预算信息*</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 } </td> 
  </tr> 
  <tr> 
   <td>管理成本和预算信息*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>创建计划</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>创建方案</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>删除计划或方案</p> </td> 
   <td> <p>✓ {\f13 }</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>复制方案</td> 
   <td>✓ {\f13 } </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publish方案**</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必须具有财务数据访问权限才能查看或管理计划的财务信息，即使您对计划具有管理权限。 有关访问财务数据的信息，请参阅[授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

**您必须具有创建权限和管理项目的权限才能发布方案。

有关项目访问级别的信息，请参阅[授予项目访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

有关项目权限的信息，请参阅[在 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)中共享项目。
