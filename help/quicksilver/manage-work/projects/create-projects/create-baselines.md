---
product-area: projects
navigation-topic: create-projects
title: 创建项目基线
description: 基线是一个项目快照，它表示初始项目计划中或在项目生命周期的任何给定时间包含的关键信息。
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 创建项目基线

基线是一个项目快照，它表示初始项目计划中或在项目生命周期的任何给定时间包含的关键信息。

您可以使用基线来比较当前计划中的这些信息与原始计划或任何其他时间点的信息，以识别问题任务、范围蠕变和其他随时间变化的趋势。

## 访问要求

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注意</b>
   如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问项目的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予对项目的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高级别的权限以查看基线</p> <p>管理项目以创建基线的权限</p> <p> 有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>.</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用基线的注意事项

* 您可以在项目的生命周期内多次捕获项目进度的快照，从而创建多个基线。
* 您可以通过创建基线或构建基线报告来查看项目基线中包含的信息。
* 创建基线时，还会在该基线的基线任务上捕获任务信息。
* 您可以通过构建基线任务报告来查看基线任务的信息。

>[!IMPORTANT]
>
>基线会生成项目名称、日期和财务信息的快照。 基线不包括项目中自定义字段的值。 有关基线中包含的财务信息，请参阅 [项目基线中包含的项目资金](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## 创建基线

可以通过以下方式创建基线：

* **自动**:您的Workfront管理员或组管理员会为Workfront设置项目首选项，以便当项目变为“当前”时自动创建基线。 启用此设置后，当项目状态变为“当前”时，将创建一个基线。 未启用此设置时，必须手动创建基线。

   有关配置项目首选项和设置自动基线创建的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!CAUTION]
   >
   >启用此设置后，每当项目状态变为“当前”时，都会自动为项目创建基线。 第一个创建的基线是默认的基线。 在项目生命周期中必须手动创建所有其他基线。

* **手动**:您可以根据需要为项目创建新基线，以便项目继续运行。 然后，可以比较基线以查看项目在一段时间内的进展情况。

要创建基线，请执行以下操作：

1. 导航到项目。
1. 在左侧面板中，单击 **基线**.

   或

   单击 **显示更多**，然后单击 **基线**.

   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)

1. 单击 **新建基线。**
1. 指定基线的名称。
1. （可选）如果这是第一个基线，则可能需要选择它作为默认基线。
1. 单击&#x200B;**保存**。

   默认情况下，将显示有关所创建基线的以下信息：

   * 基线名称
   * 基准条目日期
   * 计划起始日期创建基准时项目的起始日期
   * 预计起始日期创建基准时的项目日期
   * 创建基线时项目的实际持续时间
   * 创建基线时项目完成百分比
   * 显示基线是否为项目的默认基线的默认基线指示器

      >[!TIP]
      >
      >不能在同一视图或报表中同时查看任意两个基线的信息。 您只能在同一报表中查看给定基线和默认基线的信息。 在项目生命周期中，您可以随时修改您认为是默认基线的基线。

1. （可选）单击“视图”旁边的下拉箭头，然后 **自定义视图** 向视图添加字段并比较基线之间的其他信息。

## 创建基线或基线任务报表

要查看基线信息，您还可以创建基线或基线任务报告。 这允许您在一个视图中显示有关基线或基线任务的任意数量的字段，以比较它们。

>[!TIP]
>
>必须先创建基线，然后才能创建基线或基线任务报告。

有关创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

我们建议您将项目名称分组添加到基线或基线报表中，以便更便于阅读。

有关创建分组的信息，请参阅 [在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
