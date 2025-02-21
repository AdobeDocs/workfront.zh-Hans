---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: 了解如何在功能板上组织报表
description: 您可以查看是否向Adobe Workfront中的功能板添加了报表。 在决定您可以保留哪些报告以及可以从系统中删除哪些报告时，这可能很有用。 如果报表位于功能板上，则用户可能仍依赖这些报表。 我们建议不要删除用户正在使用的功能板上列出的报表。 有关将报表添加到功能板的更多信息，请参阅将报表添加到功能板一文。
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 了解如何在功能板上组织报表

## 访问报告列表中的仪表板信息

您可以查看是否向Adobe Workfront中的功能板添加了报表。 在决定您可以保留哪些报告以及可以从系统中删除哪些报告时，这可能很有用。 如果报表位于功能板上，则用户可能仍依赖这些报表。 我们建议不要删除用户正在使用的功能板上列出的报表。\
有关将报告添加到仪表板的更多信息，请参阅文章[将报告添加到仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)。

通过执行以下操作之一，可查看是否将报告添加到功能板：

* 构建报表列表的视图，并在列中包含仪表板信息
* 按一个或多个您知道当前正在使用的特定功能板过滤报告列表
* 为报告对象构建报告，并使用包含仪表板信息的视图或过滤器

任何人都可以构建视图或过滤器，但您必须具有访问级别的“编辑”报表访问权限才能构建报表。\
有关访问报告的详细信息，请参阅文章[授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。\
有关生成报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在报告列表视图中显示仪表板信息

>[!WARNING]
>
>在报表列表中包含功能板列可能会显着增加加载时间，尤其是对于较长的报表列表。

要构建包含报告列表的报告面板信息的视图，请执行以下操作：

1. 单击Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 在报表列表中，单击&#x200B;**查看**&#x200B;下拉菜单。
1. 单击&#x200B;**新建视图**。
1. 单击&#x200B;**添加列**。
1. 开始在&#x200B;**开始键入字段名称**&#x200B;字段中键入“仪表板”。
1. 在&#x200B;**报表**&#x200B;对象下，选择&#x200B;**仪表板**。

1. 单击&#x200B;**保存视图**。\
   报表所显示的功能板会显示在报表列表的功能板列中。\
   ![报告中的报告面板](assets/qs-dashboards-in-report-view.png)

## 按功能板信息过滤报表列表

要按功能板信息筛选报表列表，请执行以下操作：

1. 单击Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。

1. 在报表列表中，单击&#x200B;**筛选器**&#x200B;下拉菜单。
1. 单击&#x200B;**新建筛选器**，然后单击&#x200B;**添加筛选器规则**。

1. 开始在&#x200B;**开始键入字段名称**&#x200B;字段中键入“仪表板”。

1. 在&#x200B;**仪表板**&#x200B;对象下，选择&#x200B;**名称**。

1. 在修饰符下拉菜单中选择&#x200B;**等于**，然后开始键入要作为筛选依据的仪表板的名称。 您可以为过滤器选择多个功能板。\
   ![报告筛选器中的仪表板](assets/qs-dashboards-in-report-filters-350x143.png)

1. 单击&#x200B;**保存+关闭**。\
   这会显示仅列在指定功能板上的报表列表。\
   您还可以为报表对象构建报表，并在报表中使用此过滤器。
