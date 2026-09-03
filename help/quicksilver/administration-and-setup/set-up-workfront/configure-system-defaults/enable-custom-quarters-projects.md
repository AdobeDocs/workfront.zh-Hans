---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 启用自定义季度
description: 出于报告目的，如果贵组织的季度基于日历日期以外的特定标准（如工作日或购物日），则可能需要创建自定义季度。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: 902
ht-degree: 2%

---

# 启用自定义季度

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


出于报告目的，如果贵组织的季度基于日历日期以外的特定标准（如工作日或购物日），则可能需要创建自定义季度。

根据贵公司已购买的产品，您可以在Workfront设置区域中配置以下季度数：

* 仅购买[!DNL Workfront]的客户最多可以为其[!DNL Adobe Workfront]系统配置八个自定义季度。
* 购买[!DNL Workfront]和[!DNL Workfront Planning]的客户可以为其[!DNL Workfront]系统配置最多100个季度，这些季度也在[!DNL Planning]中提供。

<div class="preview">

* 购买[!DNL Workfront]和[!DNL Workfront Planning]的客户可以为每个自定义季度配置自定义周数。 自定义周在[!DNL Planning]时间线视图中可见。

</div>

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL Workflow Standard]或[！UICONTROL Workfront Plan]许可证</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## 为您的[!DNL Workfront]系统设置自定义季度

根据您使用的环境，设置自定义季度会有所不同。

### 在生产环境中为[!DNL Workfront]系统设置自定义季度

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 自定义季度]**。

1. 选择&#x200B;**[!UICONTROL 启用自定义季度]**。

1. 键入自定义季度的名称，如“Fiscal Q1 2021”。
1. 选择自定义季度的开始和结束日期。

   ![自定义季度](assets/custom-quarters-nwe.png)

1. （可选）单击&#x200B;**[!UICONTROL 添加自定义季度]**&#x200B;可向系统中添加其他自定义季度。

   >[!IMPORTANT]
   >
   > 如果贵公司购买了[!DNL Workfront Planning]，并且各季度之间存在间隔或重叠，则无法保存自定义季度。
   >![带有重叠警告的自定义季度](assets/custom-quarters-with-overlap-warning.png)
   >季度之间的间隔和重叠仅允许[!DNL Workfront]个客户使用。

1. （可选且有条件）如果贵公司只购买了[!DNL Workfront]，而没有购买[!DNL Workfront Planning]，请创建引用会计季度的报表元素。

   **示例：**&#x200B;为[!UICONTROL 项目]列表创建过滤器，并包含引用自定义季度项目的计划完成日期。

   ![包含自定义季度的“项目”筛选器](assets/example-of-project-filter-with-custom-quarters.png)

   对“本季度”、“下一季度”和“上一季度”的引用将替换为对自定义季度的新引用。

   有关报表元素的信息，请参阅[报表元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   有关创建筛选器的信息，请参阅[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中创建或编辑筛选器。
1. （可选且有条件）如果您的公司购买了Workfront Planning并且您有权访问[!DNL Workfront Planning]，请转到记录类型页面并打开时间线视图。 视图将显示新的自定义季度。
有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

<div class="preview">

### 在预览环境中为[!DNL Workfront]系统设置自定义季度

>[!NOTE]
>
>如果贵组织购买了除工作流包之外的Planning包，或者如果贵组织购买了Workfront Planning作为独立包，则除了自定义季度之外，您还可以配置自定义周数。
> 
>自定义周数不适用于Workfront报表和列表。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 自定义季度]**。

1. 选择&#x200B;**[!UICONTROL 启用自定义季度]**。

1. 键入自定义季度名称。 例如，“2021年第一季度财政年度。”
1. 选择自定义季度的开始和结束日期。

1. （可选）选择&#x200B;**开始新的自定义周序列**&#x200B;选项。

   选择此选项后，在Planning时间线视图中，将自定义季度的开始设置为季度的第一个自定义周的开始。
1. （可选）在&#x200B;**自定义周标签格式**&#x200B;区域，为自定义周标签选择&#x200B;**格式**。 从以下选项中进行选择：

   * **W1、W2、W3 ...** 。 这是默认格式。
   * **FW1、FW2、FW3...**
   * **第1周，第2周，第3周……**
   * **自定义**

1. （视情况而定）如果您为&#x200B;**Format**&#x200B;字段选择&#x200B;**Custom**，请键入&#x200B;**Custom label**&#x200B;以标识自定义周。

   自定义周显示在Planning时间线视图中。

   >[!TIP]
   >
   >添加自定义标签时，最多可键入100个字符。
   >
   >您可以指定第一周的名称，以下几周将使用相同的标签，后跟一个序列号。
   >
   >例如，“财政周”的&#x200B;**自定义标签**&#x200B;将添加“财政周1、财政周2、财政周3...”的标签 接下来的几周。

1. （可选）单击&#x200B;**[!UICONTROL 添加自定义季度]**&#x200B;可向系统中添加其他自定义季度。

   >[!IMPORTANT]
   >
   > 如果贵公司购买了[!DNL Workfront Planning]，并且各季度之间存在间隔或重叠，则无法保存自定义季度。
   >![带有重叠警告的自定义季度](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >季度之间的间隔和重叠仅允许[!DNL Workfront]个客户使用。

1. （可选且视情况而定）要在Workfront中查看自定义季度，请创建引用自定义季度的报表元素。

   **示例：**&#x200B;为[!UICONTROL 项目]列表创建过滤器，并包含引用自定义季度项目的计划完成日期。

   ![包含自定义季度的“项目”筛选器](assets/example-of-project-filter-with-custom-quarters.png)

   对“本季度”、“下一季度”和“上一季度”的引用将替换为对自定义季度的新引用。

   有关报表元素的信息，请参阅[报表元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   有关创建筛选器的信息，请参阅[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中创建或编辑筛选器。
1. （可选且视情况而定）要在Workfront Planning中查看自定义季度和周，请转到记录类型页面并打开时间线视图。 该视图显示新的自定义季度和周。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

</div>
