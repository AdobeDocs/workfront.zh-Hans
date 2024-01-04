---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于用户的通配符对报告进行归纳
description: 在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# 使用基于用户的通配符对报告进行归纳

在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行泛化。 例如，如果要创建显示分配给特定用户的任务的报告，则可以在过滤器的“分配给”字段中使用用户的名称。 但是，如果您要创建显示分配给登录用户的任务的报表，而不考虑该用户的身份，则可以使用通配符来指示当有人查看报表时，该报表仅显示与他们有关的信息。 这样的话，您只需构建一次报表，但由于您在筛选器中使用了通配符，因此每当其他人读取此报表时，它都会生成不同的结果。

在构建以下报表元素时，您可以使用基于用户的通配符：

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
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的报告元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理对报告的权限以编辑报告中的报告元素</p> <p>管理视图或筛选器的权限以编辑它们</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建报告，然后才能向其添加通配符变量。

有关创建报告的说明，请参阅 [创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步骤

要在报表中插入基于用户的通配符，请执行以下操作：

1. 转到要为其插入基于用户的通配符的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 单击 **过滤器** 选项卡。
1. 单击 **添加筛选器规则**.
1. 开始键入要作为筛选依据的字段的名称。\
   您必须键入引用用户对象或用户相关信息的字段。
1. 选择 **等于** 过滤器变量的下拉菜单中。

   >[!TIP]
   >
   >您必须始终选择 **等于** 在Adobe Workfront中使用通配符时的筛选器变量。

1. 在 **开始键入名称……** 框，键入： `$$USER.ID` 或 `$$USER.name` 如果您希望报表显示有关登录用户的信息（基于其名称）。 您可以插入引用登录用户的组、团队、公司或其他信息的其他通配符。

   有关基于用户的通配符的完整列表，请参见 [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 单击 **保存+关闭**.

## 其他信息

另请参阅：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑筛选器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
