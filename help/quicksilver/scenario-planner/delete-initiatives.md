---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除Scenario Planner中的计划
description: 您可以删除您创建的计划或他人与您共享的计划中的计划。 无法恢复已删除的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 1%

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
   <td> <p>[!DNL Adobe Workfront] 包</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>注释</b></p>
<p>如果您拥有其他Workfront软件包，请与您的Workfront代表联系。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证</p> </td> 
   <td> <p>[!UICONTROL Light]或更高版本</p> 
   <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
    <tr> 
   <td>访问级别配置</td> 
   <td> <p>[!UICONTROL Edit]访问 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[!UICONTROL Manage]对计划的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关访问Scenario Planner的详细信息，请参阅[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的访问权限。

有关Workfront访问要求的信息，请参阅[Workfront访问要求文档](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

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

   * 单击计划名称右侧的&#x200B;**[!UICONTROL 更多菜单]** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**。

   * 选中计划左侧的框，然后在计划底部显示的浮动菜单上单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，将其删除]**。

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。

### 批量删除计划 {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要删除的方案。
1. 选中要删除的方案左侧的框，然后在计划底部显示的菜单中单击&#x200B;**[!UICONTROL 删除]**，然后单击&#x200B;**[!UICONTROL 是，删除它们]**。

   ![管理计划菜单](assets/bottom-manage-initiative-menu-350x45.png)

   计划及其工作角色和成本信息将从计划中删除。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
