---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中计划方案
description: 默认情况下，每15分钟运行一次方案。 您可以通过定义激活方案运行的时间和频率来更改此设置。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 在中计划方案 [!DNL Adobe Workfront Fusion]

默认情况下，每15分钟运行一次方案。 您可以通过定义激活方案运行的时间和频率来更改此设置。

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
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 计划方案

1. 在方案详细信息页面的右上角，单击 **[!UICONTROL 选项]** > **[!UICONTROL 计划]**

   或

   单击 **[!UICONTROL 计划]** 图标（时钟）。

1. 在以下字段中输入信息：

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL运行方案]</td> 
      <td> <p>选择要运行方案的频率，然后选择间隔。</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL定期]</strong> </p> <p>输入执行之间间隔的分钟数。 默认值为15分钟。</p> </li> 
        <li> <p><strong>[!UICONTROL一次]</strong> </p> <p>输入您希望方案运行的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Vedy]</strong> </p> <p>输入您希望方案运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL每周日期]</strong> </p> <p>天数：选择您希望方案运行的一周中的天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL每月日]</strong> </p> <p>天数：选择您希望方案运行的月份天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL指定的日期]</strong> </p> <p>月：选择要运行方案的月份。 您可以选择一个或多个月份。</p> <p>天数：选择您希望方案运行的月份天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
       </ul> <p>注意：方案必须存在日期才能在该日期运行。 例如，仅计划在当月第31日的情景不会在2月、4月、6月、9月或11月运行，因为这些月没有第31天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>您可以定义运行方案的特定时间间隔。 您可以指定每日时间间隔、每周或每月。 对于每个间隔，单击 <strong>[!UICONTROL Add]</strong> 并按照[!UICONTROL运行方案]字段中所述填写字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL开始]</td> 
      <td>输入您希望方案运行的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL结束]</td> 
      <td>输入您希望方案运行的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 确定]** 以保存计划设置并返回到方案。
