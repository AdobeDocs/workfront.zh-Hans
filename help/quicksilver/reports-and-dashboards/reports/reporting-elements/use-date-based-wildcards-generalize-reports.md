---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于日期的通配符对报表进行泛化
description: 在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# 使用基于日期的通配符对报表进行泛化

在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。

例如，如果要创建一个显示具有特定计划开始日期的任务的报告，则可以在过滤器中使用日历日期选择器来选择特定日期。 但是，如果要创建一个报告来显示其规划开始日期在从访问报告日期起的某个时间范围内具有的任务，则可以使用通配符指示当有人查看报告时，它显示与他们查看报告的时刻相关的时间范围信息。

例如，在过去的一周内、在过去的一年中、接下来的两周内，等等。 这样的话，您只需构建一次报表，但由于您在筛选器中使用通配符，因此每当有人读取它时，它都会生成不同的结果，因为它会根据用户运行报表的日期而有所不同。

在构建以下报表元素时，您可以使用基于日期的通配符：

* 过滤器
* 自定义提示
* 添加列的规则时的视图

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的报告元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理对报告的权限以编辑报告中的报告元素</p> <p>管理视图或筛选器的权限以编辑它们</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

必须先创建报告，然后才能向其添加通配符变量。

有关创建报告的信息，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步骤

要在报表中插入基于日期的通配符，请执行以下操作：

1. 转到要为其插入基于日期的通配符的报表。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**编辑**。
1. 单击&#x200B;**筛选器**&#x200B;选项卡。
1. 单击&#x200B;**添加筛选器规则**。
1. 开始键入要作为筛选依据的字段的名称。\
   您必须键入引用日期的字段。
1. 在筛选器变量的下拉菜单中选择&#x200B;**等于**。

   >[!TIP]
   >
   >在Adobe Workfront中使用通配符时，必须始终选择&#x200B;**等于**&#x200B;筛选器变量。

1. 单击&#x200B;**设置相对日期**&#x200B;切换开关，然后在显示的文本框中键入： `$$TODAY`（如果要显示与运行报告同一天发生的某些事件的相关信息）。

   或

   如果要显示与运行报表的日期和时间同时发生的某些事件的相关信息，请键入`$$NOW`。

   此日期始终不同，因为它会随着用户实际查看报告的日期而更改。 所以报告中的信息每天都是不同的。

1. （可选）如果要显示运行报告日期之后某个时间范围内发生的信息，请键入`$$TODAY+1w`以显示下一周的信息，或键入`$$TODAY+2m`以显示未来两个月的信息。 您还可以指定季度、小时、天或年的时间范围。
1. （可选）如果要显示运行报告日期之前某个时间范围内发生的事件的相关信息，请键入`$$TODAY-1w`以显示前一周的信息，或键入`$$TODAY-2m`以显示前两个月的信息。 您还可以指定季度、小时、天或年的时间范围。

   有关可在基于日期的通配符中使用的属性、限定符和运算符的完整列表，请参阅文章[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 单击&#x200B;**保存+关闭**。

## 其他信息

另请参阅：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [向报告添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
