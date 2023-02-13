---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在备注报表中查看所有更新
description: 在备注报表中查看所有更新
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 在备注报表中查看所有更新

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

默认情况下，对象的“更新”区域显示的更新最多为200次。 要查看任何用户为对象输入的所有更新，您可以创建一个显示所有更新的注释报表。

>[!NOTE]
>
>您可以构建报表，以在“预览”中查看对象的更新，其中包含“日记帐分录”报表。 有关更多信息，请参阅 [报告更新区域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报表、功能板和日历</p> </li> 
     <li> <p>创建过滤器、视图和分组</p> </li> 
    </ul> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看</p> <p>注意：如果您没有对象的“查看”权限或更高权限，则该对象的信息不会显示在报表中。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建注释报表

为任何对象创建注释报告都是相同的，无论该对象是什么。

例如，要为项目中的所有注释创建注释报表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **报表**.
1. 单击 **新建报表**，然后选择 **注意**.

1. （可选）单击 **视图**，则 **添加列** 添加 **名称** 的 **项目** 在报表视图中。 

1. （可选）单击 **分组**，则 **添加分组** 分组 **项目名称**，如果您同时报告多个项目。\
   这可确保按注释各自的项目对注释进行分组，从而使报表更易于阅读。 

1. （可选）单击 **过滤器、** then **添加过滤器规则** ，以仅筛选一个项目或特定项目。

1. （视情况而定）将 **项目名称** as **等于** 到要查看其更新的项目的项目名称。  

1. 单击 **保存并关闭**.\
   所有有权至少查看项目的用户在项目中输入的所有更新都会显示在报表中。
