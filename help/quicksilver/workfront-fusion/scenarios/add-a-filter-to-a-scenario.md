---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 向 [!DNL Adobe] Workfront Fusion中的方案添加筛选器
description: 在某些情况下，您只需要使用满足特定条件的包。 您可以使用过滤器选择这些包。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 将筛选器添加到[!DNL Adobe Workfront Fusion]中的方案

在某些情况下，您只需要使用满足特定条件的包。 您可以使用过滤器选择这些包。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

可以在两个模块之间添加过滤器，并检查从上述模块接收的捆绑包是否满足特定的过滤器条件：

* 如果是，则捆绑包将传递到场景中的下一个模块。
* 如果不存在，则终止对捆绑包的处理。

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
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

## 先决条件

必须先将两个模块添加到方案中，然后才能在它们之间添加过滤器。

## 在两个模块之间添加过滤器：

1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]** ![](assets/scenarios-icon.png)，然后选择方案以将其打开。
1. 在窗口的右上角，单击&#x200B;**[!UICONTROL 编辑]**。
1. 单击模块之间的连接线。
1. 在显示的框中，键入筛选器的&#x200B;**[!UICONTROL 标签]**。
1. 定义筛选器&#x200B;**[!UICONTROL 条件]**。

   可以在两个框中输入一两个操作数。 如果在这两个框中输入操作数，则可以在它们之间的下拉菜单中选择运算符以指定它们之间的关系。

   >[!TIP]
   >
   >在操作数字段中，可以像映射值一样输入值，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块中所述。

   例如，如果您希望筛选器在[!DNL Adobe Workfront]中查找以XML结尾的文件，并将它们传递给[!DNL Dropbox]，则应在第一个框中输入&#x200B;**[!UICONTROL File name]**，然后单击。第二个框中的&#x200B;**[!UICONTROL xml]**。 在它们之间的下拉菜单中，选择&#x200B;**[!UICONTROL 结尾为（不区分大小写）]**。 此过滤器将应用于来自第一个模块(Workfront)的传入包。 只有包含XML文件的包才会传递到下一个模块([!DNL Dropbox])。

   ![](assets/set-up-filter-box-350x368.jpg)

1. 单击 **[!DNL OK]**。

## 复制筛选器

目前，场景编辑器不包括用于复制过滤器的功能。

>[!NOTE]
>
>如果复制过滤器两侧的模块，则也会复制过滤器。
>
>有关复制模块的详细信息，请参阅[复制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)中的模块或方案

要在不复制模块的情况下复制筛选器，您可以使用[!DNL Google] Chrome来采取以下解决方法：

1. 安装[!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome]扩展。
1. 在[!DNL Workfront Fusion]中，打开方案。
1. 单击Chrome三点菜单，然后单击**[!UICONTROL 更多工具*]* > **[!UICONTROL 开发人员工具]**。

1. 在显示的[!UICONTROL Developer tools]面板中，在顶部的菜单栏上单击[!UICONTROL Workfront Fusion]选项卡。

   ![](assets/copy-a-filter-350x174.png)

1. 单击左侧栏中的&#x200B;**[!UICONTROL 工具]**&#x200B;图标![](assets/devtools-tools-icon.png)。

1. 单击&#x200B;**[!UICONTROL 复制筛选器]**，然后在右侧面板中配置&#x200B;**[!UICONTROL 复制筛选器]**&#x200B;工具：

   1. 在要复制的筛选器之后，将&#x200B;**[!UICONTROL Source模块]**&#x200B;设置为模块。
   1. 将&#x200B;**[!UICONTROL 目标模块]**&#x200B;设置为要复制的筛选器之前的模块。

1. 单击&#x200B;**[!UICONTROL 运行]**。
