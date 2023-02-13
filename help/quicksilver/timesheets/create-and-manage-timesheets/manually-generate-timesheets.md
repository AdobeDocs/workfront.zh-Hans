---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 手动生成工时单
description: 要使您对时间表配置文件所做的更改能够反映在当前时间表中，必须先删除现有时间表，然后手动生成新时间表。 您可以从“工时单”区域或“设置”中的“诊断”区域手动生成工时单，如本文所述。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 手动生成工时单

要使您对时间表配置文件所做的更改能够反映在当前时间表中，必须先删除现有时间表，然后手动生成新时间表。 您可以从“工时单”区域或“设置”中的“诊断”区域手动生成工时单，如本文所述。

有关删除工时单的说明，请参阅 [删除Adobe Workfront中的工时单](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是Workfront管理员，或者，如果您正在处理组的时间表配置文件，则必须是组管理员(或Workfront管理员)。 有关更多信息，请参阅 <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>.</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关手动生成工时单的注意事项

手动生成工时单时：

* 系统会根据与用户关联的时间表配置文件生成这些配置文件。 没有与其关联的工时单配置文件的用户不会收到工时单。 
* 只生成当前时间表和后续时间表。 Workfront不会为同一时段生成两个工时单。 如果您已拥有特定时间范围的时间表，则当您使用手动流程生成时间表时，将不会生成另一个时间表。

## 从工时单和工时区手动生成工时单

您可以从“设置”的“工时单和小时”区域手动生成系统级或组级工时单。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 如果要生成整个系统中正在使用的工时单，请单击 **工时单和工时。**

   或

   如果要生成特定组使用的工时单，请单击 **群组**，然后单击群组的名称。

1. 单击 **时间表配置文件**.
1. 单击 **更多**，则 **生成工时单**.

   为与工时单配置文件关联的用户创建的新工时单最长为两个时间段。

## 从“诊断”区域手动生成系统级时间表

您可以从“设置”中的“诊断”区域手动生成系统级时间表。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 展开 **系统**，然后单击 **诊断**.

1. 单击 **执行诊断**. 
1. 单击 **生成工时单**.
