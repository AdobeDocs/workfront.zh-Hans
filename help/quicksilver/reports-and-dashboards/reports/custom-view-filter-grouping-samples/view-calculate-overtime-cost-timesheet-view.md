---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：在时间表视图中计算加班成本'
description: 在Adobe Workfront中默认不计算加班，但您可以创建计算加班的时间表报表。
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# 视图：在时间表视图中计算加班成本

<!--Audited: 11/2024-->

在Adobe Workfront中默认不计算加班，但您可以创建计算加班的时间表报表。

如果用户与其配置文件中的每小时成本费率相关联，则还可以计算该用户加班的成本额。\
有关将用户与每小时成本费率关联的信息，请参阅文章[配置我的设置](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

>[!NOTE]
>
>可添加到列表或报告中时间表视图的超时字段显示了在时间表超时字段中找到的信息。 此信息由有权修改时间表的用户手动更新。 有关时间表中“加班”字段的更多信息，请参阅文章[时间表布局概述](../../../timesheets/timesheets/timesheet-layout.md)。

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工时表视图中计算加班成本

要向时间表视图添加计算的加班列，请执行以下操作：

1. 转到时间表列表。

1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 在&#x200B;**编辑文本模式**&#x200B;框中，删除框中的文本，然后复制并粘贴以下文本模式代码：

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >此计算假定用户通常每周工作40小时。

1. 单击&#x200B;**完成**，然后命名新视图，并在时间表列表中单击&#x200B;**保存视图**。

   每个用户的加班成本显示在&#x200B;**已计算的加班成本**&#x200B;列中。


