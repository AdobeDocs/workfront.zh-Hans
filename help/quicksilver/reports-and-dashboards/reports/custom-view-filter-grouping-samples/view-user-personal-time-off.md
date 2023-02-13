---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：用户个人休息时间
description: “查看：用户个人休息时间
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9b55b302-5cdc-4437-9ce4-a15b5b43dccb
source-git-commit: 68baff382c1c5e6b69906bb021fb20fd513dad0f
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 5%

---

# 查看：用户个人关闭时间

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider hiding this article because this is not a custom view anymore.)</p>
-->

您可以构建“结束时间”报表以捕获用户的结束时间信息。

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

## 查看用户个人休息时间

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) ，然后单击 **报表>新建报表**.

1. 从下拉菜单中，选择 **结束时间**.
1. 单击 **保存并关闭**.

   默认情况下，报表在视图中显示以下字段：

   | 用户 | 在用户档案中指示休息时间的用户的名称。 |
   |---|---|
   | 开始日期 | 用户指示的时段的开始日期。 |
   | 结束日期 | 用户指示的时段的结束日期。 |

   {style=&quot;table-layout:auto&quot;}

1. （可选）通过编辑以下任意选项卡来完成报表的创建：

   * 列（视图）
   * 分组
   * 过滤器
   * 图表

   有关创建报告的信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   >[!TIP]
   >
   >我们建议为用户对象添加分组，以便更便于阅读报表。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Add Time Off information to a user report</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: old way of doing this, not working anymore)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To add a column to a user view or report to display a list of future days which have been marked for time off by users:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/time-off-report-350x61.png" alt="time_off_report.png" style="width: 350;height: 61;"> </p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;<strong>Reports > New Report.</strong> </li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<strong>New Report</strong> drop-down menu, select&nbsp;<strong>User Report</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Add Column</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<strong>Switch to Text Mode</strong>.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
   -->

<!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:<br><!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre>
   </li>
   -->

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Save</strong>+<strong>Close</strong>.</li>
   -->
