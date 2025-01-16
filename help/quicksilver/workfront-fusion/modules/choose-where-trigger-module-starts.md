---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 选择触发器模块在Adobe Workfront Fusion中的启动位置
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# 选择触发器模块在[!DNL Adobe Workfront Fusion]中的开始位置

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [选择触发器模块的开始位置](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/choose-where-trigger-module-starts.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

某些触发器模块允许您选择希望开始捆绑包检索的第一个捆绑包。

您还可以指定是在特定日期之后检索所有捆绑包，还是仅检索捆绑包。

有关触发器模块的详细信息，请参阅文章[模块类型](../../workfront-fusion/modules/module-types.md)中的[触发器模块](../../workfront-fusion/modules/module-types.md#triggers)部分。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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

+++

## 选择触发器模块的启动位置

1. 保存触发器模块。

   或

   按照[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md)中配置模块设置中的说明更改触发器模块的设置。

   或

   右键单击[!UICONTROL 方案编辑器]中触发器模块的图标，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案中所述。

1. 在出现的&#x200B;**[!UICONTROL 选择开始位置]**&#x200B;框中选择一个选项。

   ![](assets/choose-where-to-start-350x346.jpg)

   显示的选项取决于给定服务的可能性。 它们可能包括：

   <table style="table-layout:auto">
        <tr>
            <td>[！UICONTROL从现在开始]（默认）</td>
            <td>从现在起检索添加或更新的所有包（取决于设置）</td>
        </tr>
        <tr>
            <td>[！UICONTROL From after a specific date]</td>
            <td>检索在指定日期/时间之后添加或更新的所有包（取决于设置）</td>
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
            <td>允许您选择从中开始检索包的第一个包</td>
        </tr>
   </table>
