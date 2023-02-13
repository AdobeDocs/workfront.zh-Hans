---
product-area: reporting
navigation-topic: report-usage
title: 查看报表使用情况
description: 查看报表使用情况
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# 查看报表使用情况

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

为了了解在您的系统中使用报表的范围，您可以在报表列表中查看以下信息：

* 最近10位查看了报表的用户
* 在指定的时间范围内查看计数

   >[!NOTE]
   >
   >Adobe Workfront为每位用户每天计为一次视图。 如果您每天多次访问同一报表，Workfront会将此计为该报表的一个视图。 如果同一日期其他用户访问同一报表，则Workfront会将此计为第二个用户的新视图。

* 最近查看日期
* 用户上次查看时间
* 包含报表的功能板列表\
   有关显示可在报表列表中添加报表的功能板名称的详细信息，请参阅文章 [了解如何在功能板上组织报表](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

您可以构建报表列表视图，以在其中显示此信息。\
您可以按其中某些字段过滤报表列表。\
有关可以按哪些字段过滤报表的详细信息，请参阅文章 [按使用情况信息过滤报表列表](#filter-a-report-list-by-usage-information).

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

## 在报表列表的视图中显示报表使用情况信息

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.

1. 在报表列表中，单击 **查看** 下拉菜单。
1. （可选）选择 **报表使用情况** 查看以显示最常见的报表使用情况信息。\
   或

1. 单击 **新建视图** 创建自定义视图。
1. 单击 **添加列**.
1. 开始键入以下任意字段，并在这些字段显示在 **报表** 对象，以将其添加到新列：

   * **最近10位用户**:显示最近10个查看了报表的用户的名称。
   * **视图**:显示以下任意时间范围内的查看次数：

      * **本月、本季度、本年**
      * **上个月、季度、年**
      * **所有视图**:显示报表上所有视图的整体计数
   * **上次查看者**:显示有关上次查看报表的用户的信息
   * **上次查看日期**:显示上次查看报表的日期


1. 单击 **保存视图**.\
   有关报表的使用情况信息将显示在您添加到视图的列中。\
   您还可以为报表对象构建报表，并在报表中使用此视图。\
   有关构建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   您必须在访问级别拥有对报表的编辑访问权限才能构建报表。\
   有关访问报表的更多信息，请参阅文章 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 按使用情况信息过滤报表列表 {#filter-a-report-list-by-usage-information}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.
1. 在报表列表中，单击 **过滤器** 下拉菜单。
1. 单击 **新建过滤器**，然后单击 **添加过滤器规则**.
1. 开始键入以下任意字段，并在这些字段显示在 **报表** 对象，以将其添加为新过滤器规则：

   * **视图**:显示以下任意时间范围内的查看次数：

      * **本月、本季度、本年**
      * **上个月、季度、年**
      * **所有视图**
   * **上次查看者**:显示有关上次查看报表的用户的信息
   * **上次查看日期**:显示上次查看报表的日期


1. 为字段选择修饰符，然后在出现提示时指定一个值。\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. 单击 **保存过滤器**.\
   这会显示符合您定义的使用信息的报表列表。\
   您还可以为报表对象构建报表，并在报表中使用此过滤器。\
   有关构建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 您必须在访问级别拥有对报表的编辑访问权限才能构建报表。\
   有关访问报表的更多信息，请参阅文章 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 查看报表使用情况信息时出现异常

>[!IMPORTANT]
>
>自2018年3月起，已收集报告使用情况信息。 此日期之前的任何信息均不可用。

以下是使用报表使用情况信息时需要注意的一些例外情况：

* 每当报表显示在功能板或自定义选项卡上时，它都计为一个视图。 在其功能板中显示该报表的用户将显示为上次查看方式：命名用户，并显示功能板的日期将显示为上次查看日期。
* Workfront不会收集内置报表的使用情况信息。\
   有关Workfront内置报表的更多信息，请参阅文章 [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront不会收集已传送报表的使用情况信息。 提交的报表不计为一个视图。\
   有关已传送报表的更多信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* 当系统或组管理员以其他用户身份登录时，这些视图将被计入系统或组管理员，并与其关联。
* Workfront不会按自定义季度收集报表的使用情况信息。 报表使用情况字段中仅引用标准内置季度。
* Workfront不会收集共享和公开查看的报表的使用情况信息。 如果某人在未登录Workfront的情况下查看了公共报表，则不会计算报表查看次数。\
   有关共享报表的更多信息，请参阅文章 [在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
