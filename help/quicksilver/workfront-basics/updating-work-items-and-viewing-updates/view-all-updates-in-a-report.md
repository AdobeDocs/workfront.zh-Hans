---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在备注报告中查看所有更新
description: 要查看任何用户为对象输入的所有更新，您可以创建显示所有更新的“注释”报告。
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 在备注报告中查看所有更新

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

默认情况下，对象的“更新”区域最多显示200个更新。 要查看任何用户为对象输入的所有更新，您可以创建显示所有更新的“注释”报告。

>[!NOTE]
>
>您可以构建一个报表，以使用日记条目报表在预览中查看对象的更新。 有关详细信息，请参阅日志条目报告[的](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)更新区域报告。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑访问权限，并创建以下内容：</p> 
    <ul> 
     <li> <p>报告、功能板和日历</p> </li> 
     <li> <p>筛选器、视图和分组</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表中对象的权限</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 创建注释报告

为任何对象创建“注释”报告的方法与创建对象相同。

例如，要为项目中的所有注释创建注释报告：

{{step1-to-reports}}

1. 在页面的左上角，单击&#x200B;**新建报告**，然后选择&#x200B;**注释**。

1. （可选）单击&#x200B;**（列）视图**，然后单击&#x200B;**添加列**&#x200B;以将&#x200B;**项目**&#x200B;的&#x200B;**名称**&#x200B;添加到报表视图中。 

1. （可选）如果同时报告多个项目，请单击&#x200B;**分组**，然后单击&#x200B;**将分组**&#x200B;按&#x200B;**项目**&#x200B;的&#x200B;**名称**&#x200B;添加到分组中。 这可确保按其各自的项目对注释进行分组，从而使报告更易于阅读。 

1. （可选）单击&#x200B;**筛选器**，然后单击&#x200B;**添加筛选器规则**。
1. 为&#x200B;**注释** > **注释文本** > **添加筛选器不是空白的**。

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   如果项目字段已更新，但在更新时未添加任何注释，则更新的&#x200B;**注释文本**&#x200B;将显示为&#x200B;**（未向更新添加文本）**。


1. （可选）为&#x200B;**项目** > **名称** > **等于**&#x200B;添加另一个筛选器，并添加一个或多个要查看其注释的项目名称。
1. 单击&#x200B;**保存+关闭**。 具有查看项目权限的所有用户在项目中输入的所有更新都会显示在报表中。
