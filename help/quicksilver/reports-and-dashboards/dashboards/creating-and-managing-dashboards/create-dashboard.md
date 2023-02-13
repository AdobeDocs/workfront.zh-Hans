---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 创建功能板
description: 您可以创建功能板以快速访问报表、日历和外部页面中的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 创建功能板

您可以创建功能板以快速访问报表、日历和外部页面中的信息。

要了解有关功能板的更多信息，请参阅 [功能板入门](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront计划*</strong></p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront许可证*</strong></p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>编辑对报表、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>您将获得对新功能板的管理权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.<br>有关功能板权限的更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">共享报表、功能板和日历 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建以下任何对象，然后才能将其添加到功能板：

* **报表**:有关创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **日历**:有关创建日历的信息，请参阅 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **外部页面**:有关创建外部页面的信息，请参阅 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 创建功能板

1. 单击主菜单图标 ![](assets/main-menu-icon.png)，然后单击 **功能板。**
1. 单击 **新功能板**.\
   此时将显示“新建功能板”对话框。

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名称</strong></td>
      <td><p>这是您的功能板的名称。</p><p>如果您没有指定名称，则功能板上第一个报表的名称将默认成为功能板的名称。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>描述（可选）</strong></td>
      <td>这是功能板的描述。</td>
     </tr>
    </tbody>
   </table>

1. 单击与其对应的单选按钮以选择布局。

   默认为单列布局。

   有关功能板上报表布局的信息，请参阅 [了解报表在功能板上的显示方式](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. 通过在 **按名称或类型搜索……** ，然后将它们拖到布局窗格中（当它们显示在列表中时）。

   >[!NOTE]
   >
   >在搜索项目时，搜索会返回最近创建的2,000个报表中的任意一个。 搜索结果中不会返回包含Unicode字符的报表名称。 在Workfront中通过键入名称来命名对象时，最好避免包含unicode字符，而不是从其他源复制和粘贴名称。

   ![搜索报表](assets/qs-new-dashboard-ui-0722.png)

1. （可选）单击 **添加外部页面** 向功能板添加外部页面。\
   有关创建外部页面并将其嵌入功能板的更多信息，请参阅 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. 单击 **保存并关闭**.\
   功能板的右上角会显示时间戳。 时间戳包括功能板上次刷新的日期、时间和时区。
