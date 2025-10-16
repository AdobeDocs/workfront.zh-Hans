---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中更新计划优先级
description: 优先安排各项举措非常重要，因为各项举措按照其在计划中的列出顺序，从计划中接收工作角色和预算资源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

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

<!--<table style="table-layout:auto"> 
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
</table>-->

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
