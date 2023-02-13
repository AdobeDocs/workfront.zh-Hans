---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目实际开始日期概览
description: 项目、任务和问题在Adobe Workfront中具有实际开始日期。 对于任务和问题，这是它们标记为“进行中”的日期。 对于项目，这是项目上的第一个任务标记为正在进行或已完成的日期。
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 项目实际开始日期概览

项目、任务和问题在Adobe Workfront中具有实际开始日期。 对于任务和问题，这是它们标记为“进行中”的日期。 对于项目，这是项目上的第一个任务标记为正在进行或已完成的日期。

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
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问项目</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 关于Workfront中实际开始日期的考虑事项

* “实际开始日期”位于项目、任务和问题的“详细信息”部分。 
* 在创建项目、任务或问题时，不会填充其实际起始日期。
* 在项目、任务或问题上实际开始工作时，会填充实际开始日期。
* 如果项目的工作尚未开始，则“项目详细信息”选项卡中不会显示实际开始日期。

   如果任务和问题详细信息选项卡上的工作尚未开始，则实际开始日期在这些选项卡上显示为空白。

* 您可以手动修改任务或问题的实际开始日期，但无法修改项目的实际开始日期。

## 关于项目实际开始日期的注意事项

* 当发生以下任何情况时，Workfront会自动设置项目的实际日期：

   * 任务被分派人从 *新建* 不等同于 *新建*.

   * 任务受分配人更改任务的完成百分比。

      >[!IMPORTANT]
      >
      >当项目标记为“当前”时，不会填充项目实际开始日期。 必须在填充项目的实际开始日期之前，开始对项目任务执行实际工作。

      在这些情况下，项目的实际开始日期设置为项目最早任务发生这些操作的日期和时间。 这表示项目实际在此日期和时间开始。

## 找到项目的实际开始日期

您可以在以下区域中找到项目的实际开始日期：

* 在项目的详细信息部分。
* 在项目报表或视图中，当您在报表中为对象项目添加实际开始日期时。

   有关创建报告的信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

要在项目的“详细信息”部分中找到实际开始日期，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **项目**.
1. 单击要查看其实际开始日期的项目。
1. 单击 **项目详细信息** ，然后转到 **概述** 中。

   实际开始日期与其他项目日期一起显示。

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
