---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: 了解如何在功能板上组织报表
description: 您可以查看报表是否已添加到Adobe Workfront中的功能板。 在决定可以保留哪些报表以及可以从系统中删除哪些报表时，这可能非常有用。 如果报表位于功能板上，则用户可能仍然依赖这些报表。 我们建议不要删除用户正在使用的功能板上列出的报表。 有关将报表添加到功能板的更多信息，请参阅文章将报表添加到功能板。
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 了解如何在功能板上组织报表

## 在报表列表中访问功能板信息

您可以查看报表是否已添加到Adobe Workfront中的功能板。 在决定可以保留哪些报表以及可以从系统中删除哪些报表时，这可能非常有用。 如果报表位于功能板上，则用户可能仍然依赖这些报表。 我们建议不要删除用户正在使用的功能板上列出的报表。\
有关将报表添加到功能板的更多信息，请参阅文章 [将报表添加到功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

您可以通过执行以下操作之一，查看是否将报表添加到功能板：

* 构建报表列表视图，并在列中包含功能板信息
* 按一个或多个您知道正在积极使用的特定功能板过滤报表列表
* 为报表对象生成报表，并使用包含功能板信息的视图或过滤器

任何人都可以构建视图或过滤器，但您必须在访问权限级别拥有对报表的编辑访问权限才能构建报表。\
有关访问报表的更多信息，请参阅文章 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
有关构建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## 在报表列表的视图中显示功能板信息

>[!WARNING]
>
>在报表列表中包含功能板列可能会显着增加加载时间，尤其是对于较长的报表列表而言。

要使用报表列表的功能板信息构建视图，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.
1. 在报表列表中，单击 **查看** 下拉菜单。
1. 单击 **新建视图**.
1. 单击 **添加列**.
1. 开始在 **开始键入字段名称** 字段。
1. 在 **报表** 对象，选择 **功能板**.

1. 单击 **保存视图**.\
   报表显示的功能板显示在报表列表的“功能板”列中。\
   ![](assets/qs-dashboards-in-report-view.png)

## 按功能板信息过滤报表列表

要按功能板信息过滤报表列表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.

1. 在报表列表中，单击 **过滤器** 下拉菜单。
1. 单击 **新建过滤器**，然后单击 **添加过滤器规则**.

1. 开始在 **开始键入字段名称** 字段。

1. 在 **功能板** 对象，选择 **名称**.

1. 选择 **等于** 在修饰符下拉菜单中，开始键入要过滤的功能板名称。 您可以为过滤器选择多个功能板。\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. 单击 **保存并关闭**.\
   这会显示仅在指定功能板上列出的报表列表。\
   您还可以为报表对象构建报表，并在报表中使用此过滤器。
