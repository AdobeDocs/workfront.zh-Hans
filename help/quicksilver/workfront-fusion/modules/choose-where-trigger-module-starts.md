---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 选择触发器模块在Adobe Workfront Fusion中的启动位置
description: 某些触发器模块允许您选择希望开始检索捆绑的第一个捆绑包。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# 选择触发器模块的开始位置 [!DNL Adobe Workfront Fusion]

某些触发器模块允许您选择希望开始检索捆绑的第一个捆绑包。

您还可以指定是要检索所有捆绑包，还是只检索特定日期之后的捆绑包。

有关触发器模块的更多信息，请参阅部分 [触发器模块](../../workfront-fusion/modules/module-types.md#triggers) 在文章中 [模块类型](../../workfront-fusion/modules/module-types.md).

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

## 选择触发器模块的启动位置

1. 保存触发器模块。

   或

   按照中的说明更改触发器模块的设置 [在中配置模块的设置 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   或

   右键单击中触发器模块的图标 [!UICONTROL 场景编辑器]，如中所述 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 在 **[!UICONTROL 选择开始位置]** 框。

   ![](assets/choose-where-to-start-350x346.jpg)

   显示的选项取决于给定服务的可能性。 它们可能包括：

   <table style="table-layout:auto">
        <tr>
            <td>[！UICONTROL从现在开始]（默认）</td>
            <td>从现在开始检索添加或更新的所有包（取决于设置）</td>
        </tr>
        <tr>
            <td>[！UICONTROL自特定日期之后]</td>
            <td>检索在指定的日期/时间之后添加或更新的所有包（取决于设置）</td>
        </tr>
        <tr>
            <td>[！UICONTROL ID大于或等于特定值]</td>
            <td>检索ID大于或等于指定ID的所有包</td> 
        </tr>
        <tr>
            <td>[！UICONTROL所有包]</td>
            <td>检索所有可用的包</td>
        </tr>
        <tr>
            <td>[！UICONTROL选择第一个包]</td>
            <td>允许您选择开始检索包的第一个包</td>
        </tr>
   </table>
