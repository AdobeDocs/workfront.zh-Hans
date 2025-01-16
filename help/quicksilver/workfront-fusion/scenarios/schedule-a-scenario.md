---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中计划方案
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中计划方案

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [计划方案](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/schedule-a-scenario.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

默认情况下，场景每15分钟运行一次。 您可以通过定义激活方案运行的时间和频率来更改此设置。 融合场景可以计划为每5分钟运行一次。

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

## 计划方案

1. 在“方案详细信息”页面的右上角，单击&#x200B;**[!UICONTROL 选项]** > **[!UICONTROL 计划]**

   或

   单击方案触发器模块上的&#x200B;**[!UICONTROL 计划]**&#x200B;图标（时钟）。

1. 在下列字段中输入信息：

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL运行方案]</td> 
      <td> <p>选择要运行方案的频率，然后选择间隔。</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL，按固定间隔]</strong> </p> <p>输入两次执行之间的分钟数。 默认值为15分钟。</p> </li> 
        <li> <p><strong>[！UICONTROL一次]</strong> </p> <p>输入您希望方案运行的日期和时间。 使用格式<code>MM/DD/YYYY h:mm A</code>。 示例： <code>06/25/2019 11:00 PM</code>。</p> </li> 
        <li> <p><strong>[！UICONTROL每天]</strong> </p> <p>输入您希望方案运行的时间。 使用格式<code>h:mm A</code>。 示例： <code>11:00 PM</code>。</p> </li> 
        <li> <p><strong>[！UICONTROL一周天数]</strong> </p> <p>天数：选择您希望方案在一周中运行的天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式<code>h:mm A</code>。 示例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL每月日期]</strong> </p> <p>天数：选择要运行方案的月中天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式<code>h:mm A</code>。 示例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL指定日期]</strong> </p> <p>月份：选择要运行方案的月份。 您可以选择一个或多个月份。</p> <p>天数：选择要运行方案的月中天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式<code>h:mm A</code>。 示例： <code>11:00 PM</code></p> </li> 
       </ul> <p>注：方案必须存在日期才能在该日期运行。 例如，仅安排在每月第31天的方案将不会在2月、4月、6月、9月或11月运行，因为这些月份没有第31天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL高级计划]</td> 
      <td>您可以定义运行方案的特定时间间隔。 您可以指定一天中的时间间隔、工作日或月。 对于每个间隔，单击<strong>[！UICONTROL添加]</strong>并按照[！UICONTROL运行场景]字段中所述填写字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL开始]</td> 
      <td>输入您希望方案运行的日期和时间。 使用格式<code>MM/DD/YYYY h:mm A</code>。 示例： <code>06/25/2019 11:00 PM</code>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL结尾]</td> 
      <td>输入您希望方案运行之前的日期和时间。 使用格式<code>MM/DD/YYYY h:mm A</code>。 示例： <code>06/25/2019 11:00 PM</code>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 确定]**&#x200B;保存计划设置并返回方案。
