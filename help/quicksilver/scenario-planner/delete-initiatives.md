---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 删除方案计划器中的方案
description: 您可以删除您创建的计划或与您共享的计划中的方案。 您无法恢复已删除的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# 删除 [!DNL Scenario Planner]

您可以删除您创建的计划或与您共享的计划中的方案。 您无法恢复已删除的方案。

## 访问要求

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
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。 </p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!UICONTROL Scenario Planner]所需的访问权限</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 删除计划

删除计划时请考虑以下事项：

* 删除方案将从计划中删除与方案关联的任务职责和成本信息的所需数量。
* 删除通过导入项目创建的方案时，不会删除与该方案关联的项目。
* 删除至少一次已发布到项目的方案时，会导致以下结果：

   * 该方案将从方案中删除，但 [!DNL Scenario Planner] 区域仍在 [!UICONTROL 项目详细信息] 中。
   * 如果删除的方案是方案中唯一已发布的方案，则也会删除已发布计划的指标。

      有关将方案发布到项目的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      有关通过导入项目创建方案的信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

您可以一次删除一个方案，也可以批量删除多个方案。

* [删除一个方案](#delete-one-initiative)
* [批量删除计划](#delete-initiatives-in-bulk)

### 删除一个方案 {#delete-one-initiative}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   此时将显示计划列表。

1. 单击计划名称以将其打开，然后找到要删除的方案。
1. 执行下列操作之一：

   * 单击 **[!UICONTROL “更多”菜单]** ![](assets/more-menu.png) 在方案名称的右侧，单击 **[!UICONTROL 删除]** > **[!UICONTROL 是，删除它]**.

   * 选中方案左侧的框，然后单击 **[!UICONTROL 删除]** 在位于计划底部的浮动菜单上，单击 **[!UICONTROL 是，删除它]**.

   从计划中删除该方案及其职务角色和费用信息。

1. 单击 **[!UICONTROL 保存计划]** 以保存更改。

### 批量删除计划 {#delete-initiatives-in-bulk}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   此时将显示计划列表。

1. 单击计划名称以将其打开，然后找到要删除的方案。
1. 选中要删除的方案左侧的复选框，然后单击 **[!UICONTROL 删除]** 在计划底部的菜单中，单击 **[!UICONTROL 是，删除它们]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   计划中删除了这些举措及其工作职责和费用信息。

1. 单击 **[!UICONTROL 保存计划]** 以保存更改。
