---
product-area: projects
navigation-topic: create-projects
title: 创建项目基线
description: 基线是项目快照，表示初始项目计划中包含的关键信息段或在项目生命周期内的任何给定时间。
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 创建项目基线

<!-- Audited: 12/2023 -->

基线是项目快照，表示初始项目计划中包含的关键信息段或在项目生命周期内的任何给定时间。

您可以使用基准线将那些信息段从当前计划与原始计划或任何其他时间点进行比较，以确定问题任务、范围变动和其他随时间变化的趋势。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
    <td><p>新增：标准</p>
        <p>或</p>
        <p>当前：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高版本的权限以查看基线</p> <p>管理项目的权限以创建基线</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用基线的注意事项

* 您可以在项目的生命周期内多次捕获项目进度的快照，从而创建多个基线。
* 通过创建基线或生成基线报告，可以查看项目基线中包含的信息。
* 创建基线时，也会在该基线的基线任务中捕获任务信息。
* 您可以通过构建基线任务报告来查看基线任务的信息。

>[!IMPORTANT]
>
>基线会快照项目的名称、日期和财务信息。 基线不包括项目中的自定义字段值。 有关基线中包含的财务信息，请参阅[项目基线中包含的项目财务](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md)。

## 创建基线

可通过以下方式创建基线：

* **自动**：您的Workfront管理员或组管理员可为Workfront设置项目首选项，以便在项目变为当前时自动创建基线。 启用此设置后，当项目状态变为“当前”时，将创建一个基线。 如果未启用此设置，则必须手动创建基线。

  有关配置项目首选项和设置自动基线创建的详细信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

  >[!CAUTION]
  >
  >启用此设置可在每次项目状态更改为当前时自动为项目创建基线。 第一个创建的基线是默认基线。 在项目的有效期内，您必须手动创建所有其他基线。

* **手动**：您可以根据需要随着项目的进展为项目创建新基线。 然后，您可以比较基线，以查看项目在一段时间内的进展情况。

要创建基线，请执行以下操作：

1. 转到项目。
1. 在左侧面板中，单击&#x200B;**基线**。

   项目![&#128279;](assets/baselines-section-on-project-with-header.png)中的基线部分

1. 单击&#x200B;**新建基线。**
1. 指定基线的名称。
1. （可选）如果这是第一个基线，则可能需要选择它作为默认基线。
1. 单击&#x200B;**保存**。

   默认情况下，将显示有关所创建基线的以下信息：

   * 基线名称
   * 基线输入日期
   * 创建基线时项目的计划开始日期
   * 创建基线时项目的预计开始日期
   * 创建基线时项目的实际持续时间
   * 创建基线时项目的完成百分比
   * 默认基线指示器，显示基线是否为项目的默认基线

     >[!TIP]
     >
     >不能在同一视图或报告中同时查看来自任意两个基线的信息。 您只能在同一个报告中查看给定基线和“默认”基线的信息。 您可以在项目生命周期内的任何时间修改您认为作为默认基线的基线。

1. （可选）单击&#x200B;**视图**&#x200B;按钮，然后创建新视图或编辑当前视图以将字段添加到视图中，并在基线之间比较其他信息。 有关信息，请参阅[在Adobe Workfront中创建或编辑视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)。

## 创建基线或基线任务报告

要查看基线信息，您还可以创建基线或基线任务报告。 这样，您可以在一个视图中显示任意数量的有关基线或基线任务的字段，以对其进行比较。

>[!TIP]
>
>必须先创建基线，然后才能创建基线或基线任务报告。

有关创建报告的信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

我们建议您在基线或基线任务报告中添加项目名称分组，以便于阅读。

有关创建分组的信息，请参阅[在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。
