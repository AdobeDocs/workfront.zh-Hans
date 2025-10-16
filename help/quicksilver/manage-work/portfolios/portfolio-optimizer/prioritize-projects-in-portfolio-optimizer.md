---
title: 在Portfolio Optimizer中排定项目优先级
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: 您可以在Portfolio Optimizer中安排项目的优先顺序，以确立项目的完成顺序。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 在[!UICONTROL Portfolio Optimizer]中排定项目优先级

您可以在[!UICONTROL Portfolio Optimizer]中安排项目的优先顺序，以确立项目的完成顺序。

使用[!UICONTROL Portfolio优化器]时，请考虑以下事项：

* 位于[!UICONTROL Portfolio Optimizer]顶部的项目被认为比底部列出的项目更重要。 您需要按照项目在[!UICONTROL Portfolio优化器]中的优先级完成项目才能优化Portfolio。
* [!UICONTROL Portfolio优化器]中项目的优先级与项目的[!UICONTROL 项目详细信息]选项卡上的[!UICONTROL 优先级]字段无关。

  [!UICONTROL 项目详细信息]选项卡上的[!UICONTROL 优先级]字段是一个可视标志，您可以手动指定该标志以了解项目的重要性。

* Portfolio Optimizer中的项目优先级在[!DNL Resource Planner]中可见（如果在那里启用）。 在[!DNL Resource Planner]中，项目接收资源的顺序是其[!UICONTROL 资源规划者]优先级，而不是[!UICONTROL Portfolio优先级]优先级。

  有关在[!UICONTROL 资源规划程序]中排列项目优先顺序的信息，请参阅文章[在[!UICONTROL 资源规划程序]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排列项目优先顺序。

* 默认情况下，**[!UICONTROL Portfolio优化器]**&#x200B;的[!UICONTROL 项目优先顺序]区域按[!UICONTROL 计划开始日期]和[!UICONTROL 净值]的顺序显示项目。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>Workfront Prime或更高版本</p>
      <p>工作流Prime或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对[！UICONTROL项目组合]和[！UICONTROL项目]的访问权限</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合的[！UICONTROL Manage]权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## 更改[!UICONTROL Portfolio优化器]中项目的优先级

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)。

1. 单击&#x200B;**[!UICONTROL 项目组合]**。
1. （可选）在&#x200B;**[!UICONTROL 筛选器]**&#x200B;下拉菜单中选择正确的筛选器，以查看项目组合的正确列表。
1. 单击项目组合名称以将其打开。
1. 单击左侧面板中的&#x200B;**[!UICONTROL Portfolio优化]**。
1. 在[!UICONTROL 项目优化]区域，更改项目的优先级，方法是按优先级的顺序拖动项目，然后将其放到所需的显示位置。

   具有项目的![Portfolio优化器](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   完成项目重新排列后，在项目优化区域单击&#x200B;**[!UICONTROL 设置优先级]**。 项目将收到基于新订单的新编号。

1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以在[!UICONTROL Portfolio优化器]中保存新的项目优先级。 优先级在数字&#x200B;**#**&#x200B;列中列为数字。

   >[!TIP]
   >
   >这不一定会更改[!UICONTROL Portfolio优化器]中项目的顺序，因为项目列表可能会按&#x200B;**#**&#x200B;列以外的列排序。 单击&#x200B;**#**&#x200B;列标题可按项目优先级对列表进行排序。

   通过启用资源规划者中的[!UICONTROL 显示Portfolio优先级]设置，您可以看到项目在资源规划者的&#x200B;**[!UICONTROL Portfolio优化器]**&#x200B;中的优先级。

   有关在[!UICONTROL 资源规划程序]中排列项目优先顺序的信息，请参阅文章[在[!UICONTROL 资源规划程序]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排列项目优先顺序。
