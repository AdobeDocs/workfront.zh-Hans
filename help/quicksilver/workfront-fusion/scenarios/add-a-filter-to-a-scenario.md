---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 将过滤器添加到中的方案 [!DNL Adobe] Workfront Fusion
description: 在某些情况下，您只需要使用符合特定条件的包。 利用过滤器，可选择这些包。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 将过滤器添加到中的方案 [!DNL Adobe Workfront Fusion]

在某些情况下，您只需要使用符合特定条件的包。 利用过滤器，可选择这些包。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

可以在两个模块之间添加过滤器，并检查从上述模块收到的捆绑包是否满足特定的过滤器条件：

* 如果是，则捆绑包将传递到场景中的下一个模块。
* 如果失败，则终止对捆绑包的处理。

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td>    </tr> 
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

## 先决条件

必须先将两个模块都添加到方案中，然后才能在它们之间添加过滤器。

## 在两个模块之间添加过滤器：

1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) 然后，在左侧面板中选择场景以将其打开。
1. 在窗口的右上角，单击 **[!UICONTROL 编辑]**.
1. 单击模块之间的连接线。
1. 在显示的框中，键入 **[!UICONTROL 标签]** 用于筛选条件。
1. 定义过滤器 **[!UICONTROL 条件]**.

   可以在两个框中输入一个或多个操作数。 如果在这两个框中输入操作数，则可以在它们之间的下拉菜单中选择一个运算符，以指定它们之间的关系。

   >[!TIP]
   >
   >在操作数字段中，您可以按照映射这些值的相同方式输入值，如中所述 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   例如，如果您希望过滤器在中查找文件 [!DNL Adobe Workfront] 以XML结尾，并将它们传递给 [!DNL Dropbox]，您可以输入 **[!UICONTROL 文件名]** 在第一个框中输入和。**[!UICONTROL xml]** 在第二个方框中。 在它们之间的下拉菜单中，您可以选择 **[!UICONTROL 结尾为（不区分大小写）]**. 此过滤器将应用于来自第一个模块(Workfront)的传入包。 只有包含XML文件的包才会传递到下一个模块([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 单击 **[!DNL OK]**.

## 复制筛选器

目前，场景编辑器不包括用于复制过滤器的功能。

>[!NOTE]
>
>如果复制过滤器两侧的模块，则也会复制过滤器。
>
>有关复制模块的详细信息，请参见 [在中复制模块或方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

要在不复制模块的情况下复制过滤器，您可以使用 [!DNL Google] 使用Chrome解决以下问题：

1. 安装 [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 扩展。
1. In [!DNL Workfront Fusion]，打开场景。
1. 单击Chrome三个圆点菜单，然后单击**[!UICONTROL 更多工具*]* > **[!UICONTROL 开发人员工具]**.

1. 在 [!UICONTROL 开发人员工具] 面板，单击顶部菜单栏上的 [!UICONTROL Workfront Fusion] 选项卡。

   ![](assets/copy-a-filter-350x174.png)

1. 单击 **[!UICONTROL 工具]** 图标 ![](assets/devtools-tools-icon.png) 左侧栏中。

1. 单击 **[!UICONTROL 复制筛选器]**，然后配置 **[!UICONTROL 复制筛选器]** 工具：

   1. 设置 **[!UICONTROL 源模块]** 作为模块，紧跟在要复制的过滤器之后。
   1. 设置 **[!UICONTROL 目标模块]** 作为模块，位于要复制的过滤器之前。

1. 单击 **[!UICONTROL 运行]**.
