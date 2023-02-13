---
product-area: projects
navigation-topic: financials
title: 在项目层改写职务职责开单费率
description: 作为项目经理，您可以指定特定项目中某个职务角色的开单费率。 此项目层开单费率将覆盖此职务角色系统层的开单费率。 Workfront使用职务角色的项目层开单费率来计算收入，而不是使用系统层开单费率。
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 在项目层改写职务职责开单费率

作为项目经理，您可以指定特定项目中某个职务角色的开单费率。 此项目层开单费率将覆盖此职务角色系统层的开单费率。 Workfront使用职务角色的项目层开单费率来计算收入，而不是使用系统层开单费率。

本文介绍了如何覆盖项目的系统职务职责开单费率。

有关改写项目职务职责开单费率并计算项目收入的一般信息，请参阅 [改写职务职责开单费率和计算项目收入的概述](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

有关使用哪个职务角色来计算项目收入的详细信息，请参阅文章中的“了解基于用户和角色分配的任务的收入计算”部分 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>对于实际收入，对添加到标记为已开单的开单记录的小时适用的开单费率，不应受开单记录开单后发生的开单费率改写的影响。

## 访问要求

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
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问</p> <p>作业角色的管理访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理包含编辑财务数据的项目权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在项目层改写职务职责开单费率

您可以通过以下方式改写项目上职务角色的开单费率：

* 一次，为作业角色选择新费率。\
   在项目的整个期间使用新费率计算收入。

* 多次，通过为特定日期范围选择多个新费率。\
   在每个指定的日期范围内，可以使用不同的费率。

>[!TIP]
>
>您无法覆盖项目的用户开单费率。

要改写项目的开单费率，请执行以下操作：

1. 转到要覆盖其开单费率的项目。
1. 单击 **计费费率** 中。 您可能需要先单击 **显示更多**.
1. 单击 **添加帐单费率** > **新计费费率**.

   此时将打开“新计费费率”框。

1. 在 **作业角色** 字段中，选择要更改其开单费率的职务职责。

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   的 **默认开单费率** 字段显示此作业角色的系统级别费率。

1. 在 **账单费率1** 字段，输入一次性开单费率改写，然后单击 **保存** 一次覆盖开单费率

   或

   单击 **添加率** 添加更多计费费率改写。

1. （视情况而定）如果您要添加多个开单费率改写，请指定以下信息：

   * **账单费率1**:从项目开始到第一次改写的第一个日期的开单费率值。 这通常与 **默认比率**.
   * **开始日期**:这是默认费率结束的日期。
   * **结束日期**:新开单费率覆盖结束的日期。

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. 您选择日期的时区显示在“新开单费率”框的底部。 这是与您的Workfront实例关联的时区，如“设置”的“客户信息”区域中所示。 有关信息，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront将覆盖任务角色费率应用于在计算项目收入时指定的时间范围内发生的小时数。
1. 两个覆盖率的时间范围之间不应存在差距。 的 **开始日期** 覆盖率的次日应为紧接 **结束日期** 的次数。

1. 您不能为第一个改写费率指定开始日期，也不能为最后一个改写费率指定结束日期。\
   我们建议您将默认费率用于第一个覆盖率。\
   Workfront假定第一个覆盖率适用于日期早于第一个覆盖结束日期的所有小时，并且最后一个覆盖率适用于日期晚于上次覆盖开始日期的所有小时。\
   如果在项目的计划开始日期之前记录了一个小时，则使用第一个开单费率。\
   如果在项目的计划完成日期后记录了一个小时，则使用最后一个开单费率。

1. 单击&#x200B;**保存**。
