---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 创建功能板
description: 您可以创建功能板以快速访问Adobe Workfront中的信息。 可以将报告、日历和外部页面添加到功能板，以便与他人共享以实现最佳协作。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 创建功能板

<!--Audited: 01/2024-->

您可以创建功能板以快速访问Adobe Workfront中的信息。 可以将报告、日历和外部页面添加到功能板，以便与他人共享以实现最佳协作。

要了解有关功能板的更多信息，请参阅 [仪表板入门](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront计划</strong></p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront许可证*</strong></p> </td> 
   <td> <p>当前：计划 </p>
   或
   <p>新增：标准 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>访问级别配置</strong> </td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>您将获得对所创建功能板的管理权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 先决条件

必须先创建以下任意对象，然后才能将其添加到功能板：

* **报表**：有关创建报告的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **日历**：有关创建日历的信息，请参阅 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

您可以将现有外部页面添加到功能板，也可以从新功能板创建外部页面。 有关创建外部页面的信息，请参阅 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 创建功能板

{{step1-to-dashboards}}

1. 单击 **新建仪表板**.\
   此时将显示“新建仪表板”对话框。

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名称</strong></td>
      <td><p>这是仪表板的名称。</p><p>如果未指定名称，缺省情况下，操控板上第一个报表的名称将变为操控板的名称。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>描述（可选）</strong></td>
      <td>这是仪表板的描述。</td>
     </tr>
    </tbody>
   </table>

1. 单击顶部与布局对应的单选按钮，选择布局 **选择布局/添加报告/添加日历** 部分。 这是报告、日历或外部页面在功能板上显示的布局。

   默认布局为单列布局。

   有关功能板上的报告布局的信息，请参阅 [了解报告在功能板上的显示方式](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. 在中搜索报告、日历或外部页面 **按名称或类型搜索……** 字段，然后将它们拖到布局窗格中（当它们显示在列表中时）。

   >[!NOTE]
   >
   >在搜索项目时，搜索将返回最近创建的2,000个报表中的任意一个。 搜索结果中不会返回包含Unicode字符的报表名称。 作为最佳实践，在Workfront中通过键入名称来命名对象时避免包含Unicode字符，而不是从其他源复制和粘贴名称。

   ![搜索报表](assets/qs-new-dashboard-ui-0722.png)

1. （可选）单击 **添加外部页面** 将新的外部页面添加到功能板。

   有关创建外部页面并将其嵌入功能板的更多信息，请参阅 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. 单击 **保存+关闭**.

   时间戳显示在仪表板的右上角。 时间戳包括上次刷新功能板的日期、时间和时区。
