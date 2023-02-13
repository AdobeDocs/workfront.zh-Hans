---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在 [!DNL Adobe] Workfront Fusion
description: 在某些情况下，您只需要使用满足特定条件的包。 过滤器允许您选择这些包。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# 在 [!DNL Adobe Workfront Fusion]

在某些情况下，您只需要使用满足特定条件的包。 过滤器允许您选择这些包。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

您可以在两个模块之间添加过滤器，并检查从前一个模块接收的包是否满足特定过滤条件：

* 如果是这样，则包会传递到场景中的下一个模块。
* 如果没有，则对包的处理将终止。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

您必须先将这两个模块添加到方案中，然后才能在它们之间添加过滤器。

## 在两个模块之间添加过滤器：

1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) 在左侧面板中，选择方案以将其打开。
1. 在窗口的右上角，单击 **[!UICONTROL 编辑]**.
1. 单击模块之间的连接线。
1. 在显示的框中，键入 **[!UICONTROL 标签]** 中。
1. 定义过滤器 **[!UICONTROL 条件]**.

   您可以在两个框中输入一个或两个操作数。 如果在两个框中输入操作数，则可以在它们之间的下拉菜单中选择运算符，以指定它们之间的关系。

   >[!TIP]
   >
   >在操作数字段中，您可以像映射它们一样输入值，如 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   例如，如果您希望过滤器在 [!DNL Adobe Workfront] 以XML结尾，并将它们传递到 [!DNL Dropbox]，则在 **[!UICONTROL 文件名]** 和&#x200B;**[!UICONTROL xml]** 在第二个框中。 在它们之间的下拉菜单中，您可以选择 **[!UICONTROL 结束于（不区分大小写）]**. 此过滤器将应用于来自第一个模块(Workfront)的传入包。 只有包含XML文件的包才会传递到下一个模块([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 单击 **[!DNL OK]**.

## 复制过滤器

目前，方案编辑器中没有用于复制过滤器的功能。

>[!NOTE]
>
>如果复制筛选器两侧的模块，则也会复制筛选器。
>
>有关复制模块的更多信息，请参阅 [复制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

要在不复制模块的情况下复制过滤器，您可以使用 [!DNL Google] Chrome提供以下解决方法：

1. 安装 [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 扩展。
1. 在 [!DNL Workfront Fusion]，打开方案。
1. 单击Chrome三点式菜单，然后单击**[!UICONTROL 更多工具*]* > **[!UICONTROL 开发人员工具]**.

1. 在 [!UICONTROL 开发人员工具] 面板，在顶部的菜单栏上单击 [!UICONTROL Workfront Fusion] 选项卡。

   ![](assets/copy-a-filter-350x174.png)

1. 单击 **[!UICONTROL 工具]** 图标 ![](assets/devtools-tools-icon.png) 的上界。

1. 单击 **[!UICONTROL 复制过滤器]**，然后配置 **[!UICONTROL 复制过滤器]** 工具：

   1. 设置 **[!UICONTROL 源模块]** 作为模块。
   1. 设置 **[!UICONTROL 目标模块]** 作为模块。

1. 单击 **[!UICONTROL 运行]**.
