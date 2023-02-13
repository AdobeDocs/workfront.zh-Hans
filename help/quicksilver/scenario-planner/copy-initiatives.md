---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 复制方案规划器中的方案
description: 您可以通过复制现有方案来创建方案。 您可以复制您创建的计划或与您共享的计划中的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 复制 [!DNL Scenario Planner]

您可以通过复制现有方案来创建方案。 您可以复制您创建的计划或与您共享的计划中的方案。

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
   <td> <p>[!DNL Adobe Workfront]<b> 许可证</b>*</p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 复制计划

复制计划时请考虑以下事项：

* 复制方案会将副本放置在与原始方案相同的计划上。
* 复制方案副本并将以下信息从原始方案添加到新方案：

   * [!UICONTROL 持续时间]
   * [!UICONTROL 职位角色]
   * [!UICONTROL 人员] 和 [!UICONTROL 固定成本]
   * [!UICONTROL 计划收益]

* 如果原始方案上存在信息，则复制方案可以修改计划的以下信息：

   * 所需数量的作业角色
   * [!UICONTROL 成本]
   * [!UICONTROL 计划利用率]
   * 作业角色利用
   * [!UICONTROL 净值]

* 复制通过导入项目创建的或已至少一次发布到项目的方案，会产生以下影响：

   * 它不会复制与方案关联的项目。
   * 它不会将复制的方案连接到项目。
   * 它不会修改 [!DNL Scenario Planner] 中，用于至少发布一次的项目。

   有关将方案发布到项目的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   有关通过导入项目创建方案的信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## 复制计划

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   此时将显示计划列表。

1. 单击计划名称以将其打开，然后找到要复制的方案。
1. 选中要复制的方案或方案左侧的框，然后单击 **[!UICONTROL 复制]** 菜单。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] 立即复制计划，并将其置于最后选定计划之下。

   复制的方案的名称为 *[!UICONTROL 副本]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >根据您插入新方案的位置，现有方案的数量可能会发生变化。

1. 更新复制的方案的名称。

   >[!TIP]
   >
   >我们建议您始终更新方案的名称，以避免造成混淆，以防您再次复制。

1. （可选）更新新创建计划的优先级。

   有关优先排定各项倡议的信息，请参阅 [更新 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. 单击 **[!UICONTROL 保存计划]** 以保存更改。
