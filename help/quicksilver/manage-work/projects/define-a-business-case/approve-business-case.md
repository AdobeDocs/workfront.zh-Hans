---
navigation-topic: business-case-and-scorecards
title: 批准业务案例
description: 完成项目请求并提交“业务案例”后，必须批准“业务案例”。 这取决于您组织中的工作流。 在没有业务案例必须获得批准的情况下，项目可以启动，但您的Adobe Workfront管理员和项目所有者可能不认为这样做是理想的选择。
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# 批准业务案例

完成项目请求并提交“业务案例”后，必须批准“业务案例”。 这取决于您组织中的工作流。 在没有业务案例必须获得批准的情况下，项目可以启动，但您的Adobe Workfront管理员和项目所有者可能不认为这样做是理想的选择。 

有关完成和提交业务案例的更多信息，请参阅文章 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 业务案例批准概述

在批准项目的业务案例时，请考虑以下事项：

* 您必须拥有项目的“管理”权限才能批准其业务案例。 
* 您将无法在“在家中审批”下看到正在等待业务案例获得批准的项目。
* 您必须手动转至需要业务案例批准的单个项目，以查看它们是否处于待批准状态。 没有Workfront通知机制会提醒某人必须批准某个项目的商业案例。
* 您可以通过构建项目报告或访问与之关联的项目组合，找到等待业务案例批准的项目。 

   有关Portfolio的更多信息，请参阅文章 [PortfolioAdobe Workfront概述](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## 通过构建项目报告来批准业务案例

您可以为项目构建报表，以查看哪些项目需要其业务案例获得批准。 

要为等待业务案例批准的项目构建报表，请执行以下操作：

1. 为项目创建报表。

   有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 选择 **查看** ，然后单击 **添加列**.

1. 开始在 **在此列中显示** 字段，并在该字段显示在列表中时选择该字段。

    此列将显示项目的状态。

1. 选择 **过滤器** ，然后单击 **添加过滤器规则**.

1. 开始在 **仅显示包含……** 字段，并在该字段显示在列表中时将其选中。
1. 选择 **等于** （在过滤器修饰符中）。
1. 开始在可用字段中键入“已请求”。 

   这可确保报表仅包含处于“请求”状态的项目。

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. （可选）单击 **添加其他过滤器规则**.

   您可以添加其他过滤器，以仅显示您是项目所有者、项目赞助商或Portfolio所有者的项目。

   例如，您可以使用以下filter语句： 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   显示您被指定为项目赞助商的项目

   ```
   Project Owner ID Equals $$USER.ID
   ```

   显示您被指定为项目所有者的项目

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   以显示您被指定为Portfolio管理器的位置。 

1. 单击 **保存并关闭**.

   请注意，报表中的所有项目都处于 **请求**.

1. 单击报表中项目的名称以将其打开。
1. 单击 **商业案例** 中。
1. 单击 **批准** 或 **拒绝** 在“业务案例汇总”区域中批准或拒绝业务案例。 

   ![](assets/business-case-summary-with-rp-information--1-.png)

   项目状态已更改为 **已批准** 业务案例是否被批准。

   项目状态已更改为 **被拒绝** “商业”案例被拒绝时。

   >[!NOTE]
   >
   >没有通知可提醒提交业务案例批准的用户其项目请求是否被批准或拒绝。

## 通过访问组合中请求的项目批准业务案例

有关审核请求项目的详细信息，请参阅文章 [审核请求的项目](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
