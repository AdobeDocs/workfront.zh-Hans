---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和管理组的时间表配置信息
description: 当您查看在组区域管理的组时，可以查看和使用组或其子组的管理员具有管理访问权限的时间表配置文件。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 创建和管理组的周期性工时表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

当您查看在组区域管理的组时，可以查看和使用组或其子组的管理员具有管理访问权限的时间表配置文件。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td><p>您必须是组的组管理员或系统管理员。</p>
   <p>您还必须对时间表具有管理访问权限。</p></td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建和编辑组级时间表配置文件

您可以创建和编辑要在您管理的组中使用的时间表配置文件。 有关说明，请参阅[创建、编辑和分配时间表配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

## 删除组级别周期性工时表

您可以删除您管理的组正在使用的时间表配置文件。 有关说明，请参阅[删除时间表配置文件](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)。

## 手动生成组时间表

要使您对组时间表配置文件所做的更改能够反映在当前组时间表中，您必须首先删除现有时间表，然后手动生成新时间表。 有关说明，请参阅[手动生成时间表](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)中的[从时间表和小时区域](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)手动生成时间表。

有关删除组时间表的信息，请参阅[删除Adobe Workfront中的时间表](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

## 导出组级别周期性工时表

{{step-1-to-setup}}

1. 单击&#x200B;**组**。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击包含要导出的时间表配置文件的组的名称。
1. 单击&#x200B;**周期性工时表**。
1. 单击&#x200B;**导出**&#x200B;以导出组的时间表配置文件列表。
