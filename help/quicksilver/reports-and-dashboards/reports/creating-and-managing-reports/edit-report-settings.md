---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 编辑报表设置
description: 您可以编辑报表的设置，以定义报表向其他用户显示的方式，或用户在运行报表之前可提示哪些类型的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 5%

---

# 编辑报表设置

您可以编辑报表的设置，以定义报表向其他用户显示的方式，或用户在运行报表之前可提示哪些类型的信息。

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

## 操作步骤

1. 通过转到 **主菜单** > **报表**，然后选择报表的对象。

   或

   打开现有报表，然后单击 **报表操作** > **编辑**.

1. 单击 **报表设置** 报表生成器的右上角。
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
      <td>指定描述报表用途和用途的语句。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用</td> 
      <td>选择您希望此报表在为其他用户显示时使用的访问权限的用户。 有关运行具有其他用户访问权限的报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">运行并提交具有其他用户访问权限的报表</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">加载报表时，显示</td> 
      <td>选择在报表加载时为所有用户显示的默认选项卡。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在功能板上加载报表时，显示……项目</td> 
      <td>指定报表在功能板上加载时向所有用户显示的项目数。 默认为15个项目，最大项目数为200个。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在“详细信息”(Details)选项卡上显示“资源网格”(Resource Grid)视图</td> 
      <td> <p>（仅限用户报表）选择此选项，可在报表的“详细信息”选项卡上显示资源网格。</p> <p>注意：在将“资源网格”视图应用于用户报表时，该报表仅显示处于“当前”状态的项目。 如果要查看任何其他状态的项目，可以使用全局导航栏的“人员”区域中的“用户利用率”选项卡，并在此处应用“资源网格视图”。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在“详细信息”(Details)选项卡上显示特殊视图</td> 
      <td>（仅限项目报表）在“详细信息”选项卡上指定用户访问此信息时将看到的视图类型。 例如，您可以选择“里程碑”或“甘特”视图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认情况下在甘特图中显示此报告</td> 
      <td>（仅限项目报表和任务报表）选择此选项，可在用户查看此报表的“详细信息”选项卡时自动启用“甘特图”视图。<br>有关在项目报告和任务报告中查看甘特图的详细信息，请参阅文章中的“在项目列表中查看任务信息甘特图”一节 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特图中查看信息 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变查看方式</td> 
      <td>选择此选项可允许用户在运行报表时更改视图。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中改变小组</td> 
      <td>选择此选项可允许用户在运行报表时更改群组。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许在报告中更改筛选</td> 
      <td>选择此选项可允许用户在运行报表时更改过滤器。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **报表提示** 设置报表的任何提示。\
   有关向报表添加提示的详细信息，请参阅文章 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 单击&#x200B;**完成，** 然后单击 **保存并关闭**.

## 其他信息

另请参阅：

* [为新的Workfront体验创建基本报表计划](https://one.workfront.com/s/basic-report-creation-program)
* [开始使用Adobe Workfront中的报表](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
