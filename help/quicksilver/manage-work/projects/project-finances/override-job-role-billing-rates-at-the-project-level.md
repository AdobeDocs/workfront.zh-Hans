---
product-area: projects
navigation-topic: financials
title: 覆盖项目级别的工作角色记帐费率
description: 作为项目经理，您可以指定特定项目上工作角色的记帐费率。 此项目级别的记帐费率将覆盖此工作角色的系统级别的记帐费率。 Workfront使用工作角色的项目级别记帐费率来计算收入，而不是使用系统级别的记帐费率。
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# 覆盖项目级别的工作角色记帐费率

作为项目经理，您可以指定特定项目上工作角色的记帐费率。 此项目级别的记帐费率将覆盖此工作角色的系统级别的记帐费率。 Workfront使用工作角色的项目级别记帐费率来计算收入，而不是使用系统级别的记帐费率。

本文介绍了如何覆盖项目的系统工作角色记帐费率。

有关覆盖项目的工作角色记帐费率和计算项目收入的一般信息，请参阅[覆盖工作角色记帐费率并计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

有关哪个工作角色用于计算项目收入的更多信息，请参阅[账单和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)一文中的“了解基于用户和角色分配的任务的收入计算”一节。

>[!NOTE]
>
>在实际收入中，应用到标记为已记帐的记帐记录的小时数的记帐费率，不应受记帐记录记帐后发生的记帐费率覆盖的影响。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> <p>工作角色的管理访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理对包含编辑财务数据的项目的权限 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆盖项目级别的工作角色记帐费率

您可以通过以下方式覆盖项目上工作角色的记帐费率：

* 一次，通过为工作角色选择新费率。\
  新费率用于项目的整个持续时间以计算收入。

* 多次，为特定日期范围选择多个新费率。\
  在每个指定的日期范围内可以使用不同的费率。

>[!TIP]
>
>您无法覆盖项目的用户记帐费率。

要覆盖项目的记帐费率，请执行以下操作：

1. 转到要覆盖其记帐费率的项目。
1. 单击左侧面板中的&#x200B;**记帐费率**。 您可能需要先单击&#x200B;**显示更多**。
1. 单击&#x200B;**添加记帐费率** > **新记帐费率**。

   将打开“新建记帐费率”框。

1. 在&#x200B;**工作角色**&#x200B;字段中，选择要更改其计费率的工作角色。

   ![覆盖项目](assets/override-billing-rate-on-project-nwe-350x310.png)的计费率

   **默认记帐费率**&#x200B;字段显示此工作角色的系统级别费率。

1. 在&#x200B;**记帐费率1**&#x200B;字段中，输入一次性记帐费率覆盖，然后单击&#x200B;**保存**&#x200B;以一次性覆盖记帐费率

   或

   单击&#x200B;**添加费率**&#x200B;以添加更多记帐费率覆盖。

1. （视情况而定）如果要添加多个开单费率改写，请指定以下信息：

   * **记帐费率1**：从项目开始到第一次覆盖的第一个日期的记帐费率值。 这通常与&#x200B;**默认费率**&#x200B;相同。
   * **开始日期**：这是默认费率的结束日期。
   * **结束日期**：新计费率覆盖结束的日期。

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. 所选日期的时区将显示在“新建计费率”框的底部。 这是与您的Workfront实例关联的时区，如设置中的客户信息区域所示。 有关信息，请参阅[配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
1. Workfront将覆盖工作角色费率应用于计算项目收入时指定的时间范围内发生的小时数。
1. 两个覆盖率的时间范围之间不应存在间隔。 覆盖率的&#x200B;**开始日期**&#x200B;应紧跟上一个覆盖日期的&#x200B;**结束日期**&#x200B;的日期。

1. 您不能为第一个覆盖率指定开始日期，也不能为最后一个覆盖率指定结束日期。\
   我们建议您为第一个覆盖率使用默认覆盖率。\
   Workfront假定第一个覆盖率适用于日期早于第一个覆盖的结束日期的所有小时，最后一个覆盖率适用于日期早于最后一个覆盖的开始日期的所有小时。\
   如果在项目的计划开始日期之前记录了一个小时，则使用第一个记帐费率。\
   如果在项目的计划完成日期后记录了一个小时，则使用最后记帐费率。

1. 单击&#x200B;**保存**。
