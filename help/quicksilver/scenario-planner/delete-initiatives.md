---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除Scenario Planner中的计划
description: 您可以删除您创建的计划或他人与您共享的计划中的计划。 无法恢复已删除的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%

---

# 删除[!DNL Scenario Planner]中的计划

您可以删除您创建的计划或他人与您共享的计划中的计划。 无法恢复已删除的计划。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>场景规划程序不可用于新的Workfront Select或Workfront Prime计划。 </p>
   <li><p>当前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td> <p>新增：浅色或更高</p> 
   <p>当前： [！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品* </td> 
   <td> <ul><li><p>对于新的Workfront计划：</p><p> Adobe Workfront</li></p>
   <li><p>对于当前Workfront计划： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>有关详细信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别 </td> 
   <td> <p>[！UICONTROL Edit]访问 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[！UICONTROL Manage]对计划的权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中请求对计划的访问权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅[Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要删除的方案。
1. 执行下列操作之一：

   * 单击计划名称右侧的&#x200B;**[!UICONTROL 更多菜单]** ![](assets/more-menu.png)，然后单击&#x200B;**[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**。

   * 选中计划左侧的框，然后在计划底部显示的浮动菜单上单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，将其删除]**。

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。

### 批量删除计划 {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要删除的方案。
1. 选中要删除的方案左侧的框，然后在计划底部显示的菜单中单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，删除它们]**。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
