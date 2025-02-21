---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在场景规划器中更新计划优先级
description: 优先安排各项举措非常重要，因为各项举措按照其在计划中的列出顺序，从计划中接收工作角色和预算资源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# 更新[!DNL Scenario Planner]中的计划优先级

优先安排各项举措非常重要，因为各项举措按照其在计划中的列出顺序，从计划中接收工作角色和预算资源。

您可以根据您创建的计划或他人与您共享的计划来排列计划的优先级。

有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td> <ul></li>
   <li><p>新增功能：Ultimate </p></li>
   <p>Scenario Planner不可用于新的Workfront Select或Workfront Prime计划。 </p>
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

## 更新计划优先级

更改方案的优先级时，可修改其在计划中的列表顺序。

我们建议您把更紧急的举措放在计划的顶端，把更灵活的举措放在计划的底部 — 这些举措可以随时执行，并且只有在资源充足的情况下才能执行。

>[!NOTE]
>
>[!DNL Workfront]按计划上列出的顺序将计划资源分配给计划。
>
>例如，如果计划有3名可用的工程师和计划1和计划2，每位都需要2名工程师来完成，并且他们都计划在相同的时间范围内工作，则Workfront会将2名工程师与计划1关联，并将剩余1名可用的工程师与计划2关联。 在本例中，方案2显示存在冲突，因为它缺少一个工程师。 有时，更改计划的优先级是避免计划冲突的唯一方法。

要更新计划优先级，请执行以下操作：

{{step1-to-scenario-planner}}

此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要优先处理的计划。
1. 单击一个或多个计划名称左侧的框，然后执行以下操作之一：

   * 单击其中一个选定计划名称左侧的手柄，然后在列表中将其向上或向下拖动以更改计划的优先级。

     Workfront显示选定计划的数量。

     ![多选计划编号](assets/multi-select-initiative-number.png)

   * 单击计划底部的&#x200B;**[!UICONTROL 优先级]**&#x200B;框，然后从以下选项中进行选择：

      * **[!UICONTROL 前]**：将所选计划移到计划列表的顶部。 选定的计划首先在计划中列出。
      * **[!UICONTROL 底部]**：将所选计划移动到计划列表的底部。 选定的计划列在计划的最后。
      * **[!UICONTROL 选择一个数字]**：将所选计划移动到您在此处指定的计划之后。

        ![优先处理计划](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront]会立即将您指示的选定计划放置在其中，并且所有计划的数量会相应地更新。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
