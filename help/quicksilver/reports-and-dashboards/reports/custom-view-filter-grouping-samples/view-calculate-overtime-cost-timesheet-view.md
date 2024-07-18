---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：在时间表视图中计算加班成本'
description: 在Adobe Workfront中默认不计算加班，但您可以创建计算加班的时间表报表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 视图：在时间表视图中计算加班成本

在Adobe Workfront中默认不计算加班，但您可以创建计算加班的时间表报表。

如果用户与其配置文件中的每小时成本费率相关联，则还可以计算该用户加班的成本额。\
有关将用户与每小时成本费率关联的信息，请参阅文章[配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

>[!NOTE]
>
>可添加到列表或报告中时间表视图的超时字段显示了在时间表超时字段中找到的信息。 此信息由有权修改时间表的用户手动更新。 有关时间表中“加班”字段的更多信息，请参阅文章[时间表布局概述](../../../timesheets/timesheets/timesheet-layout.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在工时表视图中计算加班成本

要向时间表视图添加计算的加班列，请执行以下操作：

1. 转到时间表列表，或创建时间表报告。

   有关创建报告的信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 在时间表列表中单击&#x200B;**自定义视图**。

   或

   选择时间表报告中的&#x200B;**列（视图）**&#x200B;选项卡。

1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**。
1. 在&#x200B;**显示在此列**&#x200B;区域中，单击&#x200B;**单击以编辑文本**。
1. 在&#x200B;**文本模式**&#x200B;对话框中复制并粘贴以下文本模式代码。
   <pre>displayname=计算的加班成本<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40，({totalHours}-40)*{user}。{costPerHour}，{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >此计算假定用户通常每周工作40小时。

1. 单击&#x200B;**保存**，然后命名新视图，并在时间表列表中单击&#x200B;**保存视图**。

   或

   在时间表报告中单击&#x200B;**保存+关闭**。

1. （可选且有条件）如果要构建时间表报告，请指定报告的名称，然后单击&#x200B;**保存报告**。

   每个用户的加班成本显示在&#x200B;**已计算的加班成本**&#x200B;列中。

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
