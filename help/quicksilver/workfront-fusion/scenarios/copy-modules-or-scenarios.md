---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中复制模块或方案 [!DNL Adobe Workfront Fusion]
description: 在中复制模块或方案 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# 在中复制模块或方案 [!DNL Adobe Workfront Fusion]

您可以在中复制模块、模块组或整个方案 [!DNL Adobe Workfront Fusion]. 此功能允许您重复使用场景或部分场景，而无需再次构建它们

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

必须先将模块添加到方案中，然后才能复制它们。

## 复制一个模块或一组模块

复制模块时，复制操作会保留原始模块的所有字段值和设置。

您可以将一个或多个模块粘贴到同一场景的另一个区域或另一个场景中。

将模块粘贴到其他方案时，请考虑以下事项。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 从您未复制的其他模块中提取信息的任何字段值无法再访问该信息。 您必须设置这些字段以从新方案中提取信息。
* 如果将模块粘贴到另一个团队或组织拥有的方案中，则必须将所有连接更新为拥有新方案的组或组织所拥有的连接。

### 复制模块

复制一组模块与复制单个模块类似。

1. 右键单击要复制的模块。

   >[!NOTE]
   >
   >您可以通过按住选择多个模块 [!UICONTROL shift] 并单击要复制的模块。 复制模块组还可以复制它们之间的任何连接线、过滤器或路由逻辑。

1. 选择 **[!UICONTROL 复制模块]**.
1. 将光标移动到要复制方案的方案区域。
1. 右键单击，然后选择 **[!UICONTROL 粘贴]**.
1. 通过将粘贴的模块拖动到场景中的适当位置，将其连接到场景。

   您还可以使用键盘快捷键进行复制和粘贴。

## 通过克隆复制方案

克隆场景会创建场景的副本，然后可以对其进行编辑。

1. 打开方案详细信息页：

   1. 单击 **[!UICONTROL 方案]** 选项卡，然后单击要了解其详细信息的方案。

      或

      如果您使用的是 [中的方案编辑器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)，单击向左箭头 ![](assets/exit-editing-arrow.png) 靠近窗子的左上角。

1. 右键单击 **[!UICONTROL 选项]** 页面右上角的。
1. 选择 **[!UICONTROL 克隆]**.
1. （可选）输入新方案的名称。
1. （可选）启用 **[!UICONTROL 使任何新模块的状态与正在复制的模块状态相同]** 以确保复制的场景也包含有关原始场景处理的最近记录的信息。
1. 单击 **[!UICONTROL 保存]** 以创建方案。

## 使用Blueprint复制方案

场景Blueprint表示给定场景在给定时间点的排列、映射和字段值。 您可以将方案Blueprint导出到计算机上的JSON文件中，然后在创建新方案时导入它。 可以编辑从方案Blueprint导入的方案。

方案Blueprint表示整个方案。 如果只想从场景中复制某些模块，请参见 [复制一个模块或一组模块](#copy-a-module-or-a-group-of-modules) 本文章中。

>[!NOTE]
>
>有关上下文中的Blueprint的信息 [!DNL Adobe Workfront]，请参见 [Blueprint概述](../../administration-and-setup/blueprints/blueprints-overview.md).

### 导出方案Blueprint

1. 在场景中，单击 **[!UICONTROL 更多]** “方案设置”区域中的菜单。
1. 单击 **[!UICONTROL 导出Blueprint]**.

   将创建一个JSON文件并下载到您的计算机。 您可以在 [!DNL Downloads] 文件夹。

### 导入Blueprint

>[!IMPORTANT]
>
>如果将Blueprint导入现有方案，则方案Blueprint将替换现有方案。 不能将Blueprint附加到现有方案上。

1. 开始创建新方案。
1. 在场景中，单击 **[!UICONTROL 更多]** “方案设置”区域中的菜单。
1. 单击 **[!UICONTROL 导入Blueprint]**.
1. 在出现的对话框中，单击 **[!UICONTROL 浏览]**
1. 导航到要导入的Blueprint，然后单击 **[!UICONTROL 打开]**.
1. 单击&#x200B;**[!UICONTROL 保存]**。

   将创建一个JSON文件并下载到您的计算机。 您可以在 [!UICONTROL 下载] 文件夹。

## 使用模板复制和重用方案

您可以创建模板作为您的项目的起点 [!DNL Workfront Fusion] 场景。 从模板创建方案时，无需修改模板即可修改方案。 字段值未保存在模板中。

有关创建和使用模板的详细信息，请参阅 [方案模板](../../workfront-fusion/scenarios/templates/fusion-templates.md).
