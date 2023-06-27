---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的路由器模块
description: 使用Router模块，您可以将流量分为多条路由，并在每条路由中以不同的方式处理数据。 路由器模块收到捆绑包后，会按照将路由连接到路由器模块的顺序将其转发到每个连接的路由。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL 路由器] 中的模块 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 路由器] 模块允许您将流量分为多条路由，并在每条路由中以不同的方式处理数据。 一次 [!UICONTROL 路由器] 模块接收一个捆绑，然后按照将路由附加到的顺序将其转发到每个连接的路由。 [!UICONTROL 路由器] 模块。

>[!NOTE]
>
>* 要验证路由的顺序，可以单击 [!UICONTROL 自动对齐] 图标，将根据从上到下的顺序排列路由。
>
>  要更改顺序，请删除 [!UICONTROL 路由器] 模块并按所需顺序重新连接路由。
>
>* 路由是按顺序处理的，而不是并行处理。 直到前一路由完全处理完某个包后，才会将其发送到下一路由。
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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 添加 [!UICONTROL 路由器] 模块到场景

A [!UICONTROL 路由器] 可以通过以下方式之一添加到方案中：

* 如果要连接 [!UICONTROL 路由器] 模块后，单击模块的右手柄，开始键入 **[!UICONTROL 路由器]** 以搜索它，然后选择 **[!UICONTROL 流量控制]** > **[!UICONTROL 路由器]** 在显示的模块列表中。

  ![](assets/connect-the-router-350x108.png)

* 如果要插入 [!UICONTROL 路由器] 模块之间，单击连接两个模块的路由下方的扳手图标（或右键单击路由），然后选择 **[!UICONTROL 添加路由器]** 从菜单中。

  ![](assets/insert-router-350x191.png)

* 您可以插入 [!UICONTROL 路由器] 模块自动。 例如，在下图中，要将右下角的模块连接到左上角的模块（已连接到右上角的模块），请将右下角的左侧手柄拖放到左上角的模块。

  ![](assets/insert-router-automatically-350x379.png)

## 过滤器

您可以在路径之后放置过滤器 [!UICONTROL 路由器] 模块，用于像其他任何路由一样筛选包：

1. 单击路由中的一个点。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 在 **[!UICONTROL 设置过滤器]** 框，添加条件，然后单击 **[!UICONTROL 确定]** 以保存过滤器设置。

   ![](assets/set-up-a-filter-2-350x242.png)

有关更多信息，请参阅 [将过滤器添加到中的方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## 后备路由

路由上的过滤器设置 [!UICONTROL 路由器] 模块包含一个特殊选项：回退路由：

![](assets/fallback-route-350x260.png)

启用后，当捆绑包无法从继续时，将使用此路由。 [!UICONTROL 路由器] 模块，因为其他路由上的过滤器已将其过滤掉。

回退路由在 [!UICONTROL 路由器] 模块：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

备用路由的典型用例是：如果满足条件，则使用一条路由继续流；如果不满足，则使用另一条路由，如下面的步骤所示：

1. 插入 [!UICONTROL 路由器] 模块。
1. 将两条路由都连接到 [!UICONTROL 路由器] 模块。
1. 单击第一条路由并指定条件：

   ![](assets/set-up-a-filter-2-350x242.png)

1. 单击第二条路由，然后启用 [!UICONTROL 后备路由] 选项：

   ![](assets/enable-fallback-route-option-350x238.png)
