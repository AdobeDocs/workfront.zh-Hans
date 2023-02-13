---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 在Adobe Workfront Fusion中选择触发器模块的启动位置
description: 某些触发器模块允许您选择要从中开始检索包的第一个包。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 选择触发器模块的开始位置 [!DNL Adobe Workfront Fusion]

某些触发器模块允许您选择要从中开始检索包的第一个包。

您还可以指定是要从特定日期之后检索所有包，还是仅检索包。

有关触发器模块的更多信息，请参阅部分 [触发器模块](../../workfront-fusion/modules/module-types.md#triggers) 在文章中 [模块类型](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 选择触发器模块的启动位置

1. 保存触发器模块。

   或

   按照 [在 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   或

   右键单击 [!UICONTROL 方案编辑器]，如 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 在 **[!UICONTROL 选择开始位置]** 框中。

   ![](assets/choose-where-to-start-350x346.jpg)

   显示的选项取决于给定服务的可能性。 它们可能包括：

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on]（默认）</td>
            <td>从现在开始检索添加或更新的所有包（取决于设置）</td>
        </tr>
        <tr>
            <td>[!UICONTROL从特定日期之后开始]</td>
            <td>检索指定日期/时间后添加或更新的所有包（取决于设置）</td>
        </tr>
        <tr>
            <td>[!UICONTROL，其ID大于或等于特定值]</td>
            <td>检索ID大于或等于指定ID的所有包</td> 
        </tr>
        <tr>
            <td>[!UICONTROL所有包]</td>
            <td>检索所有可用的包</td>
        </tr>
        <tr>
            <td>[!UICONTROL选择第一个包]</td>
            <td>用于选择开始检索包的第一个包</td>
        </tr>
   </table>
