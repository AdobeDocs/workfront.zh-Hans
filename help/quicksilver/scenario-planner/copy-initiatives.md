---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中复制计划
description: 您可以通过复制现有计划来创建计划。 您可以复制您创建的计划或他人与您共享的计划中的计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# 复制[!DNL Scenario Planner]中的计划

<!--Audited: 07/2024-->

您可以通过复制现有计划来创建计划。 您可以复制您创建的计划或他人与您共享的计划中的计划。

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

## 复制计划

复制计划时，请考虑以下事项：

* 复制计划会将副本放置在与原始计划相同的计划上。
* 复制计划会将以下信息从原始计划复制并添加到新计划中：

   * [!UICONTROL 持续时间]
   * [!UICONTROL 职位角色]
   * [!UICONTROL 人员]和[!UICONTROL 固定成本]
   * [!UICONTROL 计划的收益]

* 如果原始计划中存在计划信息，则复制计划可以修改计划的以下信息：

   * 所需的工作角色数量
   * [!UICONTROL 成本]
   * [!UICONTROL 计划利用率]
   * 工作角色利用率
   * [!UICONTROL 净值]

* 复制通过导入项目创建的计划或已发布到项目中的计划至少一次，具有以下影响：

   * 它不会复制与计划关联的项目。
   * 它不会将复制的计划连接到项目。
   * 对于已发布至少一次的项目，它不会修改项目中的[!DNL Scenario Planner]部分。

  有关将计划发布到项目的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

  有关通过导入项目创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中将项目导入计划。

## 复制计划

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要复制的计划。
1. 选中要复制的一个或多个计划左侧的框，然后在计划底部显示的菜单中单击&#x200B;**[!UICONTROL 复制]**。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront]立即复制计划并将其放在最后一个选择的计划下。

   所复制计划的名称为] `<Name of original initiative>`*的*[!UICONTROL &#x200B;副本。

   >[!NOTE]
   >
   >根据插入新计划的位置，现有计划的数量可能会发生更改。

1. 更新所复制计划的名称。

   >[!TIP]
   >
   >我们建议您始终更新计划的名称，以避免在需要再次复制它们时产生混淆。

1. （可选）更新新创建计划的优先级。

   有关为计划设置优先顺序的信息，请参阅[更新 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md)中的计划优先顺序。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
