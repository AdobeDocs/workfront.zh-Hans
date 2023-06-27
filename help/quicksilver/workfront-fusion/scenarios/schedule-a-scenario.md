---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中计划场景
description: 默认情况下，场景每15分钟运行一次。 您可以通过定义激活方案运行的时间和频率来更改此设置。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# 在中计划方案 [!DNL Adobe Workfront Fusion]

默认情况下，场景每15分钟运行一次。 您可以通过定义激活方案运行的时间和频率来更改此设置。

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

## 计划方案

1. 在“方案详细信息”页面的右上角，单击 **[!UICONTROL 选项]** > **[!UICONTROL 计划]**

   或

   单击 **[!UICONTROL 计划]** 图标（时钟）。

1. 在下列字段中输入信息：

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL运行方案]</td> 
      <td> <p>选择运行方案的频率，然后选择间隔。</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL按固定间隔]</strong> </p> <p>输入两次执行之间间隔的分钟数。 默认值为15分钟。</p> </li> 
        <li> <p><strong>[！UICONTROL一次]</strong> </p> <p>输入您希望方案运行的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[！UICONTROL每天]</strong> </p> <p>输入您希望方案运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[！UICONTROL每周日期]</strong> </p> <p>天数：选择您希望方案在一周中运行的天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL每月日期]</strong> </p> <p>天数：选择要运行方案的月中天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL指定日期]</strong> </p> <p>月：选择要运行方案的月。 您可以选择一个或多个月份。</p> <p>天数：选择要运行方案的月中天数。 您可以选择一天或多天。</p> <p>时间：输入您希望方案在选定日期运行的时间。 使用格式 <code>h:mm A</code>. 示例: <code>11:00 PM</code></p> </li> 
       </ul> <p>注：方案必须存在日期才能在该日期运行。 例如，仅安排在该月的第31天的方案将不会在2月、4月、6月、9月或11月运行，因为这些月没有第31天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL高级计划]</td> 
      <td>您可以定义运行方案的特定时间间隔。 您可以指定一天中的时间间隔、工作日或月。 对于每个间隔，单击 <strong>[！UICONTROL添加]</strong> 并按照[！UICONTROL运行场景]字段中所述填写字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL开始]</td> 
      <td>输入您希望方案运行的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL结束]</td> 
      <td>输入您希望方案运行之前的日期和时间。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 示例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 确定]** 以保存计划设置并返回到方案。
