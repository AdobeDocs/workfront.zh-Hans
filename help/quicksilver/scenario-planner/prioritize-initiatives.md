---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 更新方案计划员中的方案优先级
description: 对倡议进行优先排序很重要，因为倡议按照在计划中列出的顺序从计划中获得工作角色和预算资源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 更新 [!DNL Scenario Planner]

对倡议进行优先排序很重要，因为倡议按照在计划中列出的顺序从计划中获得工作角色和预算资源。

您可以根据您创建的计划或与您共享的计划对计划进行优先级排序。

有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
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

## 更新主动行动优先事项

当您更改方案的优先级时，您会修改计划上计划的列表顺序。

我们建议您在计划的最上方放置更紧急的计划，在计划的最下方放置更多流动的计划 — 这些计划可以随时执行，但只有资源可用时才能执行。

>[!NOTE]
>
>[!DNL Workfront] 按计划中列出的计划顺序，将计划资源分配给计划。
>
>例如，如果计划有3名可用的工程师和计划1以及计划2，每个计划需要2名工程师完成，并且他们都计划在同一时间范围内完成，则Workfront将2名工程师与计划1关联，将剩余的1名可用工程师与计划2关联。 在本例中，方案2显示存在冲突，因为它缺少一个工程师。 有时，改变计划的优先顺序是避免计划冲突的唯一方法。

要更新方案优先级，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   此时将显示计划列表。

1. 单击计划名称以将其打开，然后找到要排定优先级的计划。
1. 单击一个或多个方案名称左侧的框，然后执行下列操作之一：

   * 单击选定方案名称左侧的句柄，然后将其向上或向下拖动到列表中以更改方案的优先级。

      Workfront显示选定方案的数量。

      ![](assets/multi-select-initiative-number.png)

   * 单击 **[!UICONTROL 优先级]** 框，然后从以下选项中进行选择：

      * **[!UICONTROL 顶部]**:将所选方案移到方案列表的顶部。 计划中首先列出了选定的计划。
      * **[!UICONTROL 底部]**:将选定的方案移到方案列表的底部。 计划最后列出了选定的计划。
      * **[!UICONTROL 选择数字]**:在此处指明的方案之后移动选定的方案。

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] 会立即将选定的计划放置在您所指示的位置，并相应更新所有计划的数量。


1. 单击 **[!UICONTROL 保存计划]** 以保存更改。
