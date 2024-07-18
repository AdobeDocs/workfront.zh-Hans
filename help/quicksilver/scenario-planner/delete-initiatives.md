---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除Scenario Planner中的计划
description: 您可以删除您创建的计划或他人与您共享的计划中的计划。 无法恢复已删除的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 删除[!DNL Scenario Planner]中的计划

您可以删除您创建的计划或他人与您共享的计划中的计划。 无法恢复已删除的计划。

## 访问要求

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
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。 </p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[！UICONTROL Scenario Planner]所需的访问权限</a>。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[！UICONTROL Edit]或更高版本对 [!DNL Scenario Planner]</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[！UICONTROL Manage]对计划的权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中请求对计划的访问权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 删除计划

删除计划时，请考虑以下事项：

* 删除方案会从计划中删除所需的工作角色数量以及与方案关联的成本信息。
* 删除通过导入项目创建的计划不会删除与该计划关联的项目。
* 删除已发布到项目中的计划至少一次会导致以下结果：

   * 计划已从方案中删除，但[!DNL Scenario Planner]区域仍保留在[!UICONTROL 项目详细信息]部分中。
   * 如果您删除的方案是方案中唯一发布的方案，则也会删除已发布计划的指示器。

     有关将计划发布到项目的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

     有关通过导入项目创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中将项目导入计划。

您可以一次删除一个计划，也可以批量删除多个计划。

* [删除一个计划](#delete-one-initiative)
* [批量删除计划](#delete-initiatives-in-bulk)

### 删除一个计划 {#delete-one-initiative}

1. 单击&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击[!UICONTROL 方案]。

   此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要删除的方案。
1. 执行下列操作之一：

   * 单击计划名称右侧的&#x200B;**[!UICONTROL 更多菜单]** ![](assets/more-menu.png)，然后单击&#x200B;**[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**。

   * 选中计划左侧的框，然后在计划底部显示的浮动菜单上单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，将其删除]**。

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。

### 批量删除计划 {#delete-initiatives-in-bulk}

1. 单击&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击[!UICONTROL 方案]。

   此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要删除的方案。
1. 选中要删除的方案左侧的框，然后在计划底部显示的菜单中单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，删除它们]**。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
