---
title: 授予项目访问权限
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中项目的访问权限。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e47f5d06d0c7d72c171583b53b69f951e4e99afe
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 授予项目访问权限

<!-- Audited: 12/2023 -->

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对项目的访问权限，如以下文章所述：
* [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

有关使用自定义访问级别管理用户对Workfront中其他对象类型的访问的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准 </p>
 <p>或</p> 
<p>当前：计划 </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定义访问级别配置用户对项目的访问权限

1. 开始创建或编辑访问级别，如中所述 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **视图** 或 **编辑** 按钮，然后在下选择要授予的功能 **微调您的设置**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* 拥有工作许可证的用户具有有限的项目权限。 他们可以参与项目，但无法管理项目。
   >* 具有“审阅”许可证的用户对转化问题中的项目具有“查看”权限，但其“查看”权限受限。
   >* 有关用户在与他人共享项目时可以授予的权限的信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* 在为特定类型的对象配置访问级别设置时，该配置不会影响用户对较低排名的对象的访问。 例如，您可以限制用户删除其访问级别的项目，但这不会限制他们删除比项目级别低的任务。有关对象层次结构的详细信息，请参阅部分 [对象的相互依赖性和层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （可选）单击 **设置共享默认值** 创建选项的右侧，然后 **添加规则** ，为新项目添加共享规则。

   当具有此访问级别的用户创建项目时，该项目将自动与您在左侧菜单中选择的用户共享。

   ![](assets/project-sharing-menu.png)

   在右侧的菜单中，指定您希望如何与这些用户共享项目：

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >如果具有此访问级别的用户使用项目访问模板，则该模板将覆盖访问级别中的共享设置。 有关项目访问模板的信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   您可以重复此步骤，根据需要为访问级别添加任意数量的项目共享规则。

1. 单击X关闭 **微调您的设置** 盒子。
1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行中列出的文章之一 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任务访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

   创建访问级别后，可将其分配给用户。 有关更多信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按许可证类型访问报告、功能板和日历

有关每个访问级别的用户可处理问题的信息，请参阅部分 [项目](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 访问共享项目

作为问题的所有者或创建者，您可以通过授予其他用户对其的权限来与其共享，如中所述 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置
