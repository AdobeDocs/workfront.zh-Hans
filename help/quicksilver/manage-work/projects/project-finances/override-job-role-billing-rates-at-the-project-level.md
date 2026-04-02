---
product-area: projects
navigation-topic: financials
title: 覆盖项目级别的工作角色记帐费率
description: 作为项目经理，您可以指定特定项目上工作角色的记帐费率。 此项目级别的记帐费率将覆盖此工作角色的系统级别的记帐费率。 Workfront使用工作角色的项目级别记帐费率来计算收入，而不是使用系统级别的记帐费率。
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 2%

---

# 覆盖项目级别的工作角色记帐费率

{{highlighted-preview}}

作为项目经理，您可以指定特定项目上工作角色的记帐费率。 此项目级别的记帐费率将覆盖此工作角色的系统级别的记帐费率。 Workfront使用工作角色的项目级别记帐费率来计算收入，而不是使用系统级别的记帐费率。

本文介绍了如何覆盖项目的系统工作角色记帐费率。

有关覆盖项目的工作角色记帐费率和计算项目收入的一般信息，请参阅[覆盖记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

有关使用哪个工作角色计算项目收入的更多信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)以及文章[账单和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)中的[基于用户和角色分配的任务收入计算](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)部分。

>[!NOTE]
>
>在实际收入中，应用到标记为已记帐的记帐记录的小时数的记帐费率，不应受记帐记录记帐后发生的记帐费率覆盖的影响。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td> <p>要覆盖项目的工作角色记帐费率，请执行以下操作：任何Workfront或工作流包</p>
        <p>要将属性应用于工作角色，请执行以下操作：工作流Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> <p>工作角色的管理访问权限</p></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理对包含编辑财务数据的项目的权限 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆盖项目级别的工作角色记帐费率

在改写项目中任务的开单费率时，您可以分配有效日期，并且每个日期范围具有不同的费率。 如果您未分配有效日期，则您输入的开单费率改写将用于项目的整个持续时间以计算收入。

您可以将新记帐费率添加到项目模板，当从该模板创建项目时，这些费率将成为项目记帐费率。 有关编辑模板的信息，请参阅[编辑项目模板](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)。

>[!TIP]
>
>除非您具有Workflow Ultimate包，否则无法覆盖项目的用户计费率。

要覆盖项目的记帐费率，请执行以下操作：

1. 转到要覆盖其记帐费率的项目。
1. 单击左侧面板中的&#x200B;**记帐费率**。

   或

   <span class="preview">单击左侧面板中的&#x200B;**费率**，然后单击&#x200B;**帐单**&#x200B;选项卡（如果尚未选择）。</span>

1. 单击&#x200B;**添加记帐费率** > **新记帐费率**。

   或

   <span class="preview">单击&#x200B;**添加记帐费率>新建工作角色记帐费率**。</span>

   将打开“新建记帐费率”框。

1. 在&#x200B;**工作角色**&#x200B;字段中，选择要更改其计费率的工作角色。

1. <span class="preview">（可选）选择记帐费率的任意属性，如代理或地点。</span>

   <span class="preview">系统管理员在“设置”区域中定义费率属性。</span>

1. 为记帐费率覆盖选择&#x200B;**货币**。
1. 在&#x200B;**记帐费率**&#x200B;字段中输入记帐费率覆盖，然后单击&#x200B;**保存**&#x200B;以一次性覆盖记帐费率

   或

   单击&#x200B;**添加费率**&#x200B;以添加更多记帐费率覆盖。

1. （视情况而定）对于日期有效开单费率改写，请为每个行输入以下信息：

   * **记帐费率**：从项目开始到第一次覆盖的第一个日期的记帐费率值。
   * **开始日期**：计费率覆盖开始的日期。
   * **结束日期**：记帐费率覆盖结束的日期。

   ![覆盖日期的记帐费率](assets/new-job-role-billing-rate-on-project2.png)

   在计算项目收入时，Workfront会将覆盖工作角色费率应用于这些时间范围内发生的小时数。

   Workfront允许您在覆盖时间范围之间保留间隔，但您将收到一则警告消息，确认这是有意为之。

   您无需为第一个覆盖率指定开始日期，也不需要为最后一个覆盖率指定结束日期。

   如果您只输入一个记帐费率覆盖，则该费率适用于项目的整个持续时间。 如果添加多个生效日期的覆盖，Workfront会假定第一个覆盖适用于其结束日期之前的所有小时数，而最后一个覆盖适用于其开始日期之后的所有小时数。

   Workfront假定第一个覆盖率适用于日期早于第一个覆盖的结束日期的所有小时，最后一个覆盖率适用于日期早于最后一个覆盖的开始日期的所有小时。

   如果在项目的计划开始日期之前记录了一个小时，则使用第一个记帐费率。

   如果在项目的计划完成日期后记录了一个小时，则使用最后记帐费率。

1. 单击&#x200B;**保存**。
