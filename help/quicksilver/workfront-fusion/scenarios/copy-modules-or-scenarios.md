---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 复制 [!DNL Adobe Workfront Fusion]
description: 复制 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 复制 [!DNL Adobe Workfront Fusion]

您可以复制 [!DNL Adobe Workfront Fusion]. 此功能允许您重复使用方案或部分方案，而无需再次构建它们

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

您必须先将模块添加到方案中，然后才能复制它们。

## 复制模块或一组模块

复制模块时，复制会保留原始模块的所有字段值和设置。

您可以将一个或多个模块粘贴到同一方案的其他区域，或粘贴到其他方案中。

在将模块粘贴到其他方案时，请考虑以下事项。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 从您未复制的其他模块中提取信息的任何字段值将无法再访问该信息。 您必须设置这些字段，以便从新方案中提取信息。
* 如果将模块粘贴到另一个团队或组织拥有的方案中，则所有连接都必须更新为拥有新方案的组或组织拥有的连接。

### 复制模块

复制一组模块与复制单个模块类似。

1. 右键单击要复制的模块。

   >[!NOTE]
   >
   >通过按住 [!UICONTROL shift] 并单击要复制的模块。 复制一组模块还会复制它们之间的任何连接线、过滤器或路由逻辑。

1. 选择 **[!UICONTROL 复制模块]**.
1. 将光标移到方案中希望复制该方案的区域。
1. 右键单击，然后选择 **[!UICONTROL 粘贴]**.
1. 通过将粘贴的模块拖动到方案中的相应位置，将它们连接到方案。

   您还可以使用键盘快捷键复制并粘贴。

## 通过克隆复制方案

克隆方案将创建方案的副本，然后您可以对其进行编辑。

1. 打开方案详细信息页面：

   1. 单击 **[!UICONTROL 方案]** 选项卡，然后单击要详细了解的方案。

      或

      如果您正在处理 [中的方案编辑器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)，单击左箭头 ![](assets/exit-editing-arrow.png) 在窗子的左上角附近。

1. 右键单击 **[!UICONTROL 选项]** 的双曲余切值。
1. 选择 **[!UICONTROL 克隆]**.
1. （可选）输入新方案的名称。
1. （可选）启用 **[!UICONTROL 使任何新模块的状态与复制的模块的状态相同]** 要确保复制的方案还包含有关由原始方案处理的最近记录的信息。
1. 单击 **[!UICONTROL 保存]** 以创建方案。

## 使用Blueprint复制方案

方案蓝图表示给定方案在给定时间点的排列、映射和字段值。 您可以将方案Blueprint导出到计算机上的JSON文件中，然后在创建新方案时将其导入。 可以编辑从方案Blueprint导入的方案。

方案Blueprint表示整个方案。 如果您只想从场景中复制某些模块，请参阅 [复制模块或一组模块](#copy-a-module-or-a-group-of-modules) 在本文中。

>[!NOTE]
>
>关于 [!DNL Adobe Workfront]，请参阅 [Blueprint概述](../../administration-and-setup/blueprints/blueprints-overview.md).

### 导出方案Blueprint

1. 在方案中，单击 **[!UICONTROL 更多]** 菜单。
1. 单击 **[!UICONTROL 导出Blueprint]**.

   将创建JSON文件并将其下载到您的计算机。 您可以在 [!DNL Downloads] 文件夹。

### 导入Blueprint

>[!IMPORTANT]
>
>如果将Blueprint导入现有方案，则方案Blueprint将替换现有方案。 不能将Blueprint附加到现有方案。

1. 开始创建新方案。
1. 在方案中，单击 **[!UICONTROL 更多]** 菜单。
1. 单击 **[!UICONTROL 导入Blueprint]**.
1. 在出现的对话框中，单击 **[!UICONTROL 浏览]**
1. 导航到要导入的Blueprint，然后单击 **[!UICONTROL 打开]**.
1. 单击&#x200B;**[!UICONTROL 保存]**。

   将创建JSON文件并将其下载到您的计算机。 您可以在 [!UICONTROL 下载] 文件夹。

## 使用模板复制和重复使用方案

您可以创建模板作为 [!DNL Workfront Fusion] 方案。 从模板创建方案时，您可以修改方案而不修改模板。 字段值未保存在模板中。

有关创建和使用模板的更多信息，请参阅 [方案模板](../../workfront-fusion/scenarios/templates/fusion-templates.md).
