---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 复制 [!DNL Adobe Workfront Fusion]中的模块或方案
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 复制[!DNL Adobe Workfront Fusion]中的模块或方案

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [复制模块或方案](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/copy-modules-or-scenarios.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

您可以在[!DNL Adobe Workfront Fusion]中复制模块、模块组或整个方案。 此功能允许您重复使用场景或部分场景，而无需再次构建它们

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

必须先将模块添加到方案中，然后才能复制它们。

## 复制一个模块或一组模块

复制模块时，复制操作会保留原始模块的所有字段值和设置。

您可以将一个或多个模块粘贴到同一场景的另一个区域或另一个场景中。

将模块粘贴到其他方案时，请考虑以下事项。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* 从您未复制的其他模块中提取信息的任何字段值都将无法再访问该信息。 必须设置这些字段才能从新方案中提取信息。
* 如果将模块粘贴到另一个团队或组织所拥有的方案中，则必须将所有连接更新为拥有新方案的组或组织所拥有的连接。

### 复制模块

复制一组模块与复制单个模块类似。

1. 右键单击要复制的模块。

   >[!NOTE]
   >
   >按住[!UICONTROL Shift]并单击要复制的模块，可选择多个模块。 复制一组模块时，还会复制它们之间的任何连接线、过滤器或路由逻辑。

1. 选择&#x200B;**[!UICONTROL 复制模块]**。
1. 将光标移动到您希望场景副本所在的场景区域。
1. 右键单击，然后选择&#x200B;**[!UICONTROL 粘贴]**。
1. 通过将粘贴的模块拖动到方案中的适当位置，将其连接到方案。

   您还可以使用键盘快捷键进行复制和粘贴。

## 通过克隆复制方案

克隆方案会创建方案的副本，然后可以对其进行编辑。

1. 打开方案详细信息页：

   1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]**&#x200B;选项卡，然后单击要了解详细信息的方案。

      或

      如果您正在[场景编辑器中的 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)中处理场景，请单击窗口左上角附近的左箭头![](assets/exit-editing-arrow.png)。

1. 右键单击页面右上角的&#x200B;**[!UICONTROL 选项]**。
1. 选择&#x200B;**[!UICONTROL 克隆]**。
1. （可选）输入新方案的名称。
1. （可选）启用&#x200B;**[!UICONTROL 使任何新模块的状态与正在复制的模块状态相同]**，以确保复制的方案也包含有关原始方案处理的最新记录的信息。
1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以创建方案。

## 使用Blueprint复制方案

场景Blueprint表示给定场景在给定时间点的排列、映射和字段值。 您可以将方案Blueprint导出到计算机上的JSON文件中，然后在创建新方案时导入它。 可以编辑从方案Blueprint导入的方案。

方案Blueprint表示整个方案。 如果只想从场景中复制某些模块，请参阅本文中的[复制模块或模块组](#copy-a-module-or-a-group-of-modules)。

>[!NOTE]
>
>有关[!DNL Adobe Workfront]上下文中Blueprint的信息，请参阅[Blueprint概述](../../administration-and-setup/blueprints/blueprints-overview.md)。

### 导出方案Blueprint

1. 在方案中，单击方案设置区域中的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单。
1. 单击&#x200B;**[!UICONTROL 导出Blueprint]**。

   将创建一个JSON文件并下载到您的计算机。 您可以在[!DNL Downloads]文件夹中找到此文件。

### 导入Blueprint

>[!IMPORTANT]
>
>如果将Blueprint导入现有方案，则方案Blueprint将替换现有方案。 不能将Blueprint附加到现有方案。

1. 开始创建新方案。
1. 在方案中，单击方案设置区域中的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单。
1. 单击&#x200B;**[!UICONTROL 导入Blueprint]**。
1. 在出现的对话框中，单击&#x200B;**[!UICONTROL 浏览]**
1. 导航到要导入的Blueprint，然后单击&#x200B;**[!UICONTROL 打开]**。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   将创建一个JSON文件并下载到您的计算机。 您可以在[!UICONTROL 下载]文件夹中找到此文件。

## 使用模板复制和重用方案

您可以创建模板作为[!DNL Workfront Fusion]方案的起点。 从模板创建方案时，无需修改模板即可修改方案。 字段值未保存在模板中。

有关创建和使用模板的详细信息，请参阅[方案模板](../../workfront-fusion/scenarios/templates/fusion-templates.md)。
