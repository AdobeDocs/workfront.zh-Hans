---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基于用户的通配符对报表进行归纳
description: 在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行归纳。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 使用基于用户的通配符对报表进行归纳

在构建某些报表元素时，您可以使用通配符而不是特定信息来对报表进行归纳。 例如，如果要创建一个报表以显示分配给特定用户的任务，则可以在过滤器的“分配给”字段中使用该用户的名称。 但是，如果要创建报表以显示分配给登录用户的任务（无论该用户是谁），则可以使用通配符指示当某人查看报表时，它仅显示与其相关的信息。 这样，您只需构建一次报表，但由于您在过滤器中使用通配符，因此每次其他人读取报表时，都会生成不同的结果。

在生成以下报表元素时，可以使用基于用户的通配符：

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

有关创建报告的说明，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步骤

要在报表中插入基于用户的通配符，请执行以下操作：

1. 转到要为其插入基于用户的通配符的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 单击 **过滤器** 选项卡。
1. 单击 **添加过滤器规则**.
1. 开始键入要过滤的字段名称。\
   必须键入引用用户对象或有关用户信息的字段。
1. 选择 **等于** （位于过滤器变量的下拉菜单中）。

   >[!TIP]
   >
   >您必须始终选择 **等于** 在Adobe Workfront中使用通配符时筛选变量。

1. 在 **开始键入名称……** 框，键入 `$$USER.ID` 或 `$$USER.name` 如果您希望报告显示有关登录用户的信息（基于用户名）。 您可以插入其他引用登录用户的群组、团队、公司或其他信息的通配符。

   有关基于用户的通配符的完整列表，请参阅 [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 单击 **保存并关闭**.

## 其他信息

另请参阅：

* [基本报表创建程序](https://one.workfront.com/s/basic-report-creation-program)
* [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中创建或编辑过滤器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
