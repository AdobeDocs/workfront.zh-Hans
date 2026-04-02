---
content-type: overview
product-area: projects
navigation-topic: financials
title: 覆盖项目级别的用户记帐费率
description: 本文介绍了如何覆盖项目的系统用户计费率。
author: Lisa
feature: Work Management
source-git-commit: 8f6f14d4b36a9eee499111b1a37912f641c9f2ba
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 2%

---

# 覆盖项目级别的用户记帐费率

{{highlighted-preview-article-level}}

作为项目经理，您可以指定特定项目上用户的记帐费率。 此项目级别的记帐费率将覆盖此用户在系统级别的记帐费率。 Workfront使用用户的项目级记帐费率来计算收入，而不是使用系统级记帐费率。

本文介绍了如何覆盖项目的系统用户计费率。

有关覆盖项目的记帐费率和计算项目收入的一般信息，请参阅[覆盖记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

有关计算项目收入的更多信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)以及文章[记帐和收入概览](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments)中的[基于用户和角色分配的任务的收入计算](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)部分。

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
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p>
       <p><p>您还必须具有下列任一属性：</p> 
        <ul> 
          <li> <p>系统管理员访问级别。 </li> 
          <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理对包含编辑财务数据的项目的权限 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆盖项目级别的用户记帐费率

在改写项目用户的记帐费率时，您可以分配有效日期，并且每个日期范围具有不同的费率。 如果您未分配有效日期，则您输入的开单费率改写将用于项目的整个持续时间以计算收入。

要覆盖项目的用户记帐费率，请执行以下操作：

1. 转到要覆盖其记帐费率的项目。
1. 单击左侧面板中的&#x200B;**费率**。 您可能需要先单击&#x200B;**显示更多**。
1. 单击&#x200B;**帐单**&#x200B;选项卡（如果尚未选择）。
1. 单击&#x200B;**添加记帐费率** > **新用户记帐费率**。

   将打开“新建用户记帐费率”框。

1. 在&#x200B;**用户**&#x200B;字段中，选择要更改其计费率的用户。
1. 为记帐费率覆盖选择&#x200B;**货币**。
1. 在&#x200B;**记帐费率**&#x200B;字段中，输入第一个记帐费率覆盖。
1. （可选）单击&#x200B;**添加日期有效费率**&#x200B;以添加更多记帐费率覆盖。
1. （视情况而定）如果要添加多个开单费率改写，请为每个行指定以下信息：

   * **记帐费率**：指定时间段内的记帐费率值。
   * **开始日期**：计费率覆盖开始的日期。
   * **结束日期**：记帐费率覆盖结束的日期。

   ![新用户记帐费率框显示有效日期](assets/new-user-billing-rate-on-project2.png)

   在计算项目收入时，Workfront会将覆盖用户费率应用于这些时间范围内发生的小时。

   Workfront允许您在覆盖时间范围之间保留间隔，但您将收到一则警告消息，确认这是有意为之。

   您无需为第一个覆盖率指定开始日期，也不需要为最后一个覆盖率指定结束日期。

   如果您只输入一个记帐费率覆盖，则该费率适用于项目的整个持续时间。 如果添加多个生效日期的覆盖，Workfront会假定第一个覆盖适用于其结束日期之前的所有小时数，而最后一个覆盖适用于其开始日期之后的所有小时数。

   Workfront假定第一个覆盖率适用于日期早于第一个覆盖的结束日期的所有小时，最后一个覆盖率适用于日期早于最后一个覆盖的开始日期的所有小时。

   如果在项目的计划开始日期之前记录了一个小时，则使用第一个记帐费率。

   如果在项目的计划完成日期后记录了一个小时，则使用最后记帐费率。

1. 单击&#x200B;**保存**。
