---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：在“时间表视图”中计算超时成本
description: 在Adobe Workfront中默认不计算超时，但您可以创建用于计算超时的时间表报表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 查看：在时间表视图中计算超时成本

在Adobe Workfront中默认不计算超时，但您可以创建用于计算超时的时间表报表。

如果用户在其配置文件中与每小时成本费率关联，则您还可以计算该用户的超时成本金额。\
有关将用户与每小时成本费率关联的信息，请参阅文章 [配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>可添加到列表或报表中的“时间表”视图的“超时”字段显示在时间表的“超时”字段中找到的信息。 此信息由有权修改时间表的用户手动更新。 有关时间表中“超时”字段的详细信息，请参阅文章 [了解时间表布局](../../../timesheets/timesheets/timesheet-layout.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在时间表视图中计算超时成本

要向工时单视图添加计算的超时列，请执行以下操作：

1. 转到工时单列表，或创建工时单报表。

   有关创建报告的信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 单击 **自定义视图** 时间表列表中。

   或

   选择 **列（视图）** 选项卡。

1. 单击 **添加列**.
1. 单击 **切换到文本模式**.
1. 在 **在此列中显示** 区域，单击 **单击以编辑文本**.
1. 在 **文本模式** 对话框。
   <pre>displayname=Calculated Ambering Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}。{costPerHour},{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >此计算假定用户通常每周工作40小时。

1. 单击 **保存**，然后命名新视图并单击 **保存视图** 时间表列表中。

   或

   单击 **保存并关闭** 时间表报表中。

1. （可选和视情况而定）如果要生成时间表报表，请指定报表的名称，然后单击 **保存报表**.

   每个用户的超时成本显示在 **计算的加班成本** 列。

   ![calculated_overtime_cost_in_timeske_report_png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
