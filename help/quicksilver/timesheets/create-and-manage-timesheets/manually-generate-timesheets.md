---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 手动生成工时表
description: 要使您对时间表用户档案所做的更改反映在当前时间表中，必须首先删除现有时间表，然后手动生成新时间表。 您可以在“设置”的“时间表”区域或“诊断”区域中手动生成时间表，如本文所述。
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 手动生成工时表

要使您对时间表用户档案所做的更改反映在当前时间表中，必须首先删除现有时间表，然后手动生成新时间表。 您可以在“设置”的“时间表”区域或“诊断”区域中手动生成时间表，如本文所述。

有关删除时间表的说明，请参阅[删除Adobe Workfront中的时间表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

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
   <td>
   <p>标准</p>
   <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td><p>您必须是Workfront管理员，或者，如果您正在处理组的时间表配置文件，则必须是组管理员(或Workfront管理员)。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关手动生成的时间表的注意事项

当您手动生成时间表时：

* 它们是根据与您的用户关联的时间表配置文件生成的。 不具有与其关联的时间表配置文件的用户不会收到时间表。
* 只生成当前时间表以及要遵循的时间表。 Workfront不会为同一期间生成两个时间表。 如果您已经拥有当前时间范围的工时表，则在使用手动流程生成工时表时将不会生成另一个工时表。

## 从时间表和小时数区域手动生成时间表

您可以从“设置”中的时间表和小时数区域手动生成系统级别或组级别的时间表。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 如果您正在生成整个系统中使用的时间表，请单击&#x200B;**时间表和小时数。**

   或

   如果要生成特定组使用的时间表，请单击&#x200B;**组**，然后单击该组的名称。

1. 单击&#x200B;**周期性工时表**。
1. 单击“更多”图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**生成时间表**。

1. 在时间表配置文件列表顶部，单击系统级时间表配置文件的&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，或单击组时间表配置文件的&#x200B;**更多**，然后单击&#x200B;**生成时间表**。

   新时间表最多可为与时间表配置文件关联的用户创建两个时间段。

## 从诊断区域手动生成系统级时间表

您可以在“设置”的“诊断”区域中手动生成系统级时间表。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 展开&#x200B;**系统**，然后单击&#x200B;**诊断**。

1. 单击&#x200B;**执行诊断**。
1. 单击&#x200B;**生成工时表**。
