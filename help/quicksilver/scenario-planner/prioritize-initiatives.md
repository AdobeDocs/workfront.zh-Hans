---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在场景规划器中更新计划优先级
description: 优先安排各项举措非常重要，因为各项举措按照其在计划中的列出顺序，从计划中接收工作角色和预算资源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 更新[!DNL Scenario Planner]中的计划优先级

优先安排各项举措非常重要，因为各项举措按照其在计划中的列出顺序，从计划中接收工作角色和预算资源。

您可以根据您创建的计划或他人与您共享的计划来排列计划的优先级。

有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

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
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
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

## 更新计划优先级

更改方案的优先级时，可修改其在计划中的列表顺序。

我们建议您把更紧急的举措放在计划的顶端，把更灵活的举措放在计划的底部 — 这些举措可以随时执行，并且只有在资源充足的情况下才能执行。

>[!NOTE]
>
>[!DNL Workfront]按计划上列出的顺序将计划资源分配给计划。
>
>例如，如果计划有3名可用的工程师和计划1和计划2，每位都需要2名工程师来完成，并且他们都计划在相同的时间范围内工作，则Workfront会将2名工程师与计划1关联，并将剩余1名可用的工程师与计划2关联。 在本例中，方案2显示存在冲突，因为它缺少一个工程师。 有时，更改计划的优先级是避免计划冲突的唯一方法。

要更新计划优先级，请执行以下操作：

1. 单击&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击[!UICONTROL 方案]。

   此时将显示计划列表。

1. 单击计划的名称以将其打开，然后找到要优先处理的计划。
1. 单击一个或多个计划名称左侧的框，然后执行以下操作之一：

   * 单击其中一个选定计划名称左侧的手柄，然后在列表中将其向上或向下拖动以更改计划的优先级。

     Workfront显示选定计划的数量。

     ![](assets/multi-select-initiative-number.png)

   * 单击计划底部的&#x200B;**[!UICONTROL 优先级]**&#x200B;框，然后从以下选项中进行选择：

      * **[!UICONTROL 前]**：将所选计划移到计划列表的顶部。 选定的计划首先在计划中列出。
      * **[!UICONTROL 底部]**：将所选计划移动到计划列表的底部。 选定的计划列在计划的最后。
      * **[!UICONTROL 选择一个数字]**：将所选计划移动到您在此处指定的计划之后。

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront]会立即将您指示的选定计划放置在其中，并且所有计划的数量会相应地更新。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。
