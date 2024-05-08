---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在备注报告中查看所有更新
description: 在备注报告中查看所有更新
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 在备注报告中查看所有更新

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

默认情况下，对象的“更新”区域最多显示200个更新。 要查看任何用户为对象输入的所有更新，您可以创建显示所有更新的“注释”报告。

>[!NOTE]
>
>您可以构建一个报表，以使用日记条目报表在预览中查看对象的更新。 有关更多信息，请参阅 [报告更新区域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>新增：标准 </p>
   <p>当前：计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>编辑以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报告、功能板和日历</p> </li> 
     <li> <p>创建筛选器、视图和分组</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看</p> <p><b>注释</b></p>
   <p>如果您没有对象的“查看”权限或更高权限，则该对象的信息不会显示在报表中。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅 [Adobe Workfront中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 创建注释报告

为任何对象创建“注释”报告的方法与创建对象相同。

例如，要为项目中的所有注释创建注释报告：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 **报表**.
1. 单击 **新建报告**，然后选择 **注意**.

1. （可选）单击 **视图**，则 **添加列** 添加 **名称** 的 **项目** 从报告中可以看出。 

1. （可选）单击 **分组**，则 **添加分组** 分组依据 **项目名称**，如果同时报告多个项目。\
   这可确保按其各自的项目对注释进行分组，从而使报告更易于阅读。 

1. （可选）单击 **筛选器，** 则 **添加筛选器规则**.
1. 添加筛选条件 **注意** > **注释文本** > **不为空**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   如果更新了项目字段，但在更新时没有添加注释，则 **注释文本** 的更新显示为 **（未向更新添加文本）**.


1. （可选）添加另一个过滤器 **项目** > **名称** > **等于** 并添加一个或多个要查看其注释的项目名称。
1. 单击 **保存+关闭**.\
   所有至少具有查看权限的用户在项目中输入的所有更新都会显示在报表中。
