---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的路由器模块
description: 路由器模块允许您将流量分为多条路由，并以不同的方式处理每条路由中的数据。 路由器模块收到捆绑包后，会按照路由连接到路由器模块的顺序将其转发到每个连接的路由。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的[!UICONTROL 路由器]模块

[!UICONTROL 路由器]模块允许您将流量分为多条路由，并以不同的方式处理每条路由中的数据。 一旦[!UICONTROL 路由器]模块收到捆绑包，它会按照路由连接到[!UICONTROL 路由器]模块的顺序将其转发到每个连接的路由。

>[!NOTE]
>
>* 要验证路由的顺序，可以单击[!UICONTROL 自动对齐]图标，该图标将按照从上到下的顺序排列路由。
>
>  要更改顺序，请删除[!UICONTROL 路由器]模块，并按所需顺序重新连接路由。
>
>* 路由是按顺序处理的，而不是并行处理的。 直到上一路由完全处理完某个捆绑包后，该捆绑包才会发送到下一路由。
>



## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 将[!UICONTROL 路由器]模块添加到方案

可以通过以下方式之一将[!UICONTROL 路由器]添加到方案中：

* 如果要在某个模块后连接[!UICONTROL Router]模块，请单击该模块的右手柄，开始键入&#x200B;**[!UICONTROL router]**&#x200B;进行搜索，然后在显示的模块列表中选择&#x200B;**[!UICONTROL 流量控制]** > **[!UICONTROL 路由器]**。

  ![](assets/connect-the-router-350x108.png)

* 如果要在两个模块之间插入[!UICONTROL 路由器]模块，请单击连接两个模块的路由下面的扳手图标（或右键单击该路由），然后从菜单中选择&#x200B;**[!UICONTROL 添加路由器]**。

  ![](assets/insert-router-350x191.png)

* 您可以自动插入[!UICONTROL 路由器]模块。 例如，在下图中，要将右下角的模块连接到左上角的模块（已连接到右上角的模块），请将右下角的左侧手柄拖放到左上角的模块。

  ![](assets/insert-router-automatically-350x379.png)

## 过滤器

您可以在[!UICONTROL 路由器]模块之后的路由上放置过滤器，以像在任何其他路由上一样过滤包：

1. 单击路由中的一个点。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 在显示的&#x200B;**[!UICONTROL 设置筛选器]**&#x200B;框中，添加条件，然后单击&#x200B;**[!UICONTROL 确定]**&#x200B;以保存筛选器设置。

   ![](assets/set-up-a-filter-2-350x242.png)

有关详细信息，请参阅[将筛选器添加到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)中的方案。

## 后备路由

[!UICONTROL 路由器]模块之后的路由上的过滤器设置包含一个特殊选项：回退路由：

![](assets/fallback-route-350x260.png)

启用后，此路由用于包无法通过任何其他路由从[!UICONTROL 路由器]模块继续运行的情况，因为其他路由上的筛选器已将其过滤掉。

回退路由在[!UICONTROL 路由器]模块内使用不同的箭头符号进行区分：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

备用路由的典型使用情形是，如果满足条件，则使用一条路由继续流，如果不满足条件，则使用另一条路由，如以下步骤所示：

1. 在场景中插入[!UICONTROL 路由器]模块。
1. 将两条路由都连接到[!UICONTROL 路由器]模块。
1. 单击第一条路由并指定条件：

   ![](assets/set-up-a-filter-2-350x242.png)

1. 单击第二个路由并启用[!UICONTROL 备用路由]选项：

   ![](assets/enable-fallback-route-option-350x238.png)
