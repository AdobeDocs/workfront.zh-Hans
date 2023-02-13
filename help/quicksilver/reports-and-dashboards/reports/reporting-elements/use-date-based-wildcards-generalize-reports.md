---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于日期的通配符对报表进行归纳
description: 在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行归纳。
author: Lisa
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 使用基于日期的通配符对报表进行归纳

在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行归纳。

例如，如果要创建显示具有特定计划起始日期的任务的报表，则可以使用过滤器中的日历日期选取器来选择特定日期。 但是，如果要创建一个报表，以显示在从访问报表之日起的特定时间范围内具有计划开始日期的任务，则可以使用通配符指示当某人查看报表时，将显示与他们查看报表时间段相关的信息。

例如，在过去一周、过去一年、接下来的两周等。 这样，您只需构建一次报表，但由于您在过滤器中使用通配符，因此每次有人读取报表时，报表都会生成不同的结果，因为它会根据他们运行报表的当天进行调整。

在生成以下报表元素时，可以使用基于日期的通配符：

* 过滤器
* 自定义提示
* 添加列规则时的视图

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的报表元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理报表的权限以编辑报表中的报表元素</p> <p>管理视图或过滤器的权限以对其进行编辑</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建报表，然后才能向报表添加通配符变量。

有关创建报表的信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步骤

要在报表中插入基于日期的通配符，请执行以下操作：

1. 转到要为其插入基于日期的通配符的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 单击 **过滤器** 选项卡。
1. 单击 **添加过滤器规则**.
1. 开始键入要过滤的字段名称。\
   必须键入引用日期的字段。
1. 选择 **等于** （位于过滤器变量的下拉菜单中）。

   >[!TIP]
   >
   >您必须始终选择 **等于** 在Adobe Workfront中使用通配符时筛选变量。

1. 在 **开始键入名称……** 框，键入 `$$TODAY` 当您希望显示有关在报表运行的同一天发生的事件的信息时。

   或

   类型 `$$NOW` 如果您希望显示有关在报表运行的同一日期和时间发生的事件的信息。

   此日期始终不同，因为它会随着用户实际查看报表的日期而发生更改。 因此，报表中的信息会与日常有所不同。

1. （可选）如果要显示在报表运行日期后的某个时间范围内发生的信息，请键入 `$$TODAY+1w` 显示下周的信息，或 `$$TODAY+2m` 以显示未来两个月的信息。 您还可以指示季度、小时、天或年的时间范围。
1. （可选）如果要显示有关在报表运行日期之前的某个时间范围内发生的事件的信息，请键入 `$$TODAY-1w` 显示上周的信息，或 `$$TODAY-2m` 以显示前两个月的信息。 您还可以指示季度、小时、天或年的时间范围。

   有关可在基于日期的通配符中使用的属性、限定符和运算符的完整列表，请参阅文章 [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. 单击 **保存并关闭**.

## 其他信息

另请参阅：

* [基本报表创建程序](https://one.workfront.com/s/basic-report-creation-program)
* [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑过滤器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
