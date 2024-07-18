---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 配置删除和还原对象时的影响（小时）
description: 您可以配置当有人删除要记录小时数的项目、任务或问题时，小时数会发生什么情况。 您选择的选项还决定了稍后恢复项目、任务或问题时发生的小时数。 (有关在Workfront中恢复项目的更多信息，请参阅恢复已删除的项目。)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 配置删除和还原对象时的影响（小时）

您可以配置当有人删除要记录小时数的项目、任务或问题时，小时数会发生什么情况。 您选择的选项还决定了稍后恢复项目、任务或问题时发生的小时数。 (有关在Workfront中还原项目的详细信息，请参阅[还原已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。)

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置在删除和还原项目时如何管理小时数

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 展开&#x200B;**时间表和小时数**，然后单击&#x200B;**首选项**。

1. 找到&#x200B;**项目、任务或问题删除首选项**&#x200B;部分。
1. （视情况而定）要配置删除项目时小时数的管理方式，请在&#x200B;**删除项目时**&#x200B;分区中选择以下选项之一：

   * 保留已添加到时间表的已记录小时数作为常规小时数（如果该项目在稍后恢复，小时数仍保留在时间表中）\
     默认情况下，该选项处于选中状态。
   * 删除任何记录的小时数（如果该项目在稍后恢复，记录的小时数将恢复到项目中）

1. （视情况而定）要配置在删除任务或问题时如何管理小时数，请在&#x200B;**删除任务或问题时**&#x200B;部分中选择以下选项之一：

   * 将任何记录的小时数移动到任务或问题所在的项目（如果稍后恢复此任务或问题，小时数仍保留在项目中）\
     默认情况下，该选项处于选中状态。
   * 删除任何记录的小时数（如果稍后恢复此任务或问题，则记录的小时数将恢复到任务或问题）

1. 单击&#x200B;**保存**。
