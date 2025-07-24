---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 手动生成工时表
description: 要使您对时间表用户档案所做的更改反映在当前时间表中，必须首先删除现有时间表，然后手动生成新时间表。 您可以在“设置”的“时间表”区域或“诊断”区域中手动生成时间表，如本文所述。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# 手动生成工时表

要使您对时间表用户档案所做的更改反映在当前时间表中，必须首先删除现有时间表，然后手动生成新时间表。 您可以在“设置”的“时间表”区域或“诊断”区域中手动生成时间表，如本文所述。

有关删除时间表的说明，请参阅[删除Adobe Workfront中的时间表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>规划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员，或者，如果您正在处理组的时间表配置文件，则必须是组管理员(或Workfront管理员)。 有关详细信息，请参阅<a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>。</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

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
1. 单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**生成时间表**。

   新时间表最多可为与时间表配置文件关联的用户创建两个时间段。

## 从诊断区域手动生成系统级时间表

您可以在“设置”的“诊断”区域中手动生成系统级时间表。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 展开&#x200B;**系统**，然后单击&#x200B;**诊断**。

1. 单击&#x200B;**执行诊断**。 
1. 单击&#x200B;**生成工时表**。
