---
product-area: enterprise-scenario-planner-product-area
keywords: 计划，权限，共享，方案，方案，方案
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案计划员中共享计划
description: 您可以与其他用户共享在Adobe Workfront方案规划器中创建的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# 在中共享计划 [!DNL Scenario Planner]

您可以在 [!DNL Adobe Workfront Scenario Planner] 与其他用户协作，以便他们能够与您协作的相同工作。

>[!TIP]
>
>如果您向其他人发送指向计划的链接，则还必须与他们共享计划，以便他们能够查看计划。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 计划*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 许可证*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>对的[!UICONTROL编辑]访问权限 [!DNL Scenario Planner]</p> <p>如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p> [!UICONTROL管理]计划的权限
     <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Request]对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 授予计划权限的用户必须有权访问 [!DNL Scenario Planner] 访问级别中的区域(由 [!DNL Workfront] 管理员，以便接收计划的权限。

   例如， [!UICONTROL 请求者] 无法查看、创建或编辑计划。 在与拥有请求者许可证的用户共享计划时，应牢记这一点。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

有关访问 [!DNL Scenario Planner] 有关各种许可证类型，请参阅 [授予访问 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## 关于计划共享的注意事项

* 您可以共享单个计划，也可以批量共享多个计划。
* 您无法查看未创建或未与您共享的计划。
* 您只能与其他用户共享计划。 您无法与组、团队或公司共享计划。
* 必须先保存计划，然后才能共享计划。
* 您可以与其他用户共享计划的URL。 如果用户没有至少查看计划的权限，则在收到URL时，他们可以请求其他用户访问计划。 有关请求访问计划的信息，请参阅 [请求对 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* 在共享多个已与他人共享的计划时，您与之共享的用户不会替换，而是会添加到您选择的每个计划的现有用户中。

## 共享计划

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **[!UICONTROL 方案]**.
1. 单击计划的名称以将其打开

   或

   选择多个计划以批量共享它们。

   >[!TIP]
   >
   >您可以通过单击计划标题右上角与其共享计划的用户的变量来共享计划。

1. （视情况而定）如果您打开了计划，请单击 **[!UICONTROL 更多]** 图标 ![](assets/more-icon.png) 权利 [!UICONTROL 计划] 名称，然后单击 **[!UICONTROL 共享]**

   或

   如果您选择了多个计划以批量共享它们，请单击 **[!UICONTROL 共享]** 图标 ![](assets/share-icon-26x26.png) 打开 [!UICONTROL 计划] 访问框。

   >[!TIP]
   >
   >* 对您选择的所有计划拥有权限的用户将显示在 [!UICONTROL 计划] 访问框。
   >* 任何其他用户都会添加到中，并且不会替换所有选定计划上的现有用户。


1. 在 **[!UICONTROL 授予计划访问权限]** 字段中，开始键入要与之共享计划的用户名称，然后在列表中显示时选择这些用户。
1. 从用户名右侧的权限下拉菜单中，选择要授予计划的权限级别。
1. 从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL视图]</td> 
      <td>与您共享计划的用户将有权查看计划。 他们无法编辑计划、添加方案、方案或发布方案的信息。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL管理]</td> 
      <td> <p>您与共享计划的用户有权管理计划，包括编辑信息、添加方案、方案和发布计划。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >您只能在创建计划后删除计划。 您无法删除与您共享的计划。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   计划现已与您指定的用户共享。

   您可以在计划列表或计划题头右上角的“与我共享”列中查看对计划拥有权限的用户。

   >[!TIP]
   >
   >您可以通过应用 [!UICONTROL 与我共享] 在计划列表中筛选。

## 计划权限选项

下表列出了在共享计划时可授予的权限。 有关用户根据其许可证获得的访问权限的更多信息，请参阅 [授予访问 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>操作</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL管理]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL视图]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>查看计划 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看计划 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>查看方案</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>查看作业角色</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>查看成本和预算信息*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>管理成本和预算信息*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>创建计划</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>创建方案</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>删除方案或方案</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>复制方案</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>发布方案**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必须拥有财务数据的访问权限，才能查看或管理有关计划的财务信息，即使您拥有计划的管理权限也是如此。 有关访问金融数据的信息，请参阅 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**您必须拥有创建权限和管理项目的权限，才能发布方案。

有关项目访问级别的信息，请参阅 [授予对项目的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

有关项目权限的信息，请参阅 [在中共享项目 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
