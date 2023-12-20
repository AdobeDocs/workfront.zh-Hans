---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 编辑报表设置
description: 您可以编辑报告的设置以定义对其他用户的显示方式，或者用户在运行报告之前可以提示输入哪些信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 6%

---

# 编辑报表设置

您可以编辑报告的设置以定义对其他用户的显示方式，或者用户在运行报告之前可以提示输入哪些信息。

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 操作步骤

1. 通过转到 **主菜单** > **报表**，然后选择报表的对象。

   或

   打开现有报表，然后单击 **报表操作** > **编辑**.

1. 单击 **报表设置** （位于report builder的右上角）。
1. 配置以下报表设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">报告标题</td> 
      <td>指定报表的标题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>指定描述报告用途和用途的语句。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用以下访问权限运行此报告：</td> 
      <td>选择您希望此报告在为其他用户显示时用于其访问权限的用户。 有关使用其他用户的访问权限运行报告的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">运行并交付具有其他用户访问权限的报告</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">加载报告时，显示</td> 
      <td>选择加载报告时为所有用户显示的默认选项卡。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">当报表在仪表板上加载时，显示……项目</td> 
      <td>指定当报告在功能板上加载时为所有用户显示的项目数。 默认值为15项，最大项数为200。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在详细信息选项卡上显示资源网格视图</td> 
      <td> <p>（仅限用户报表）选择此选项可在报表的详细信息选项卡上显示资源网格。</p> <p>注：在将资源网格视图应用于用户报表时，该报表仅显示处于当前状态的项目。 如果要查看处于任何其他状态的项目，可以使用全局导航栏的“人员”区域中的“用户利用率”选项卡，并在该处应用“资源网格视图”。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在详细信息选项卡上显示特殊视图</td> 
      <td>（仅项目报告）指定用户在详细信息选项卡上访问此信息时将看到的视图类型。 例如，您可以选择“里程碑”或“甘特图”视图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认情况下在甘特图中显示此报告</td> 
      <td>（仅限项目报告和任务报告）选择此选项可在用户查看此报表中的“详细信息”选项卡时自动启用甘特图。<br>有关在项目报告和任务报告中查看甘特图的更多信息，请参阅文章中的“在项目列表甘特图中查看任务信息”部分 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特图中查看信息 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变查看方式</td> 
      <td>选择此选项可允许用户在运行报告时更改视图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变小组</td> 
      <td>选择此选项可允许用户在运行报告时更改组。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中更改筛选</td> 
      <td>选择此选项可允许用户在运行报告时更改筛选器。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **报告提示** 为报告设置任何提示。\
   有关向报表添加提示的更多信息，请参阅文章 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 单击&#x200B;**完成，** 然后单击 **保存+关闭**.

## 其他信息

另请参阅：

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [报告入门](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront内置报告](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
