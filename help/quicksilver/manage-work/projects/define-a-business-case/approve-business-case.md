---
navigation-topic: business-case-and-scorecards
title: 批准业务案例
description: 在完成并提交项目请求的商业论证后，必须批准该商业论证。 这取决于您组织中的工作流。 项目可以在没有业务案例必须获得批准的情况下开始，但您的Adobe Workfront管理员和项目所有者可能认为不宜这样做。
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# 批准业务案例

<!--Audit: 6/2025-->

在完成并提交项目请求的商业论证后，必须批准该商业论证。 这取决于您组织中的工作流。 项目可以在没有业务案例必须获得批准的情况下开始，但您的Adobe Workfront管理员和项目所有者可能认为不宜这样做。

有关完成和提交业务案例的详细信息，请参阅文章[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
   <p>当前：Prime或更高版本</p>
   <p>或</p>
   <p>旧版：商业版或更高版本</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   <p>当前：标准 </p> 
   <p>旧版：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理项目的权限</p> <p>查看项目组合或更高权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 业务案例审批概览

在批准项目的业务案例时，请考虑以下事项：

* 您必须对项目具有管理权限才能审批该项目的业务案例。
* 您将无法在主页的“我的审批”小组件下看到正在等待业务案例获得批准的项目。
* 您必须手动转到需要业务案例批准的单个项目，以查看它们正在等待批准。 没有Workfront通知机制可提醒某人必须批准项目的业务案例。
* 您可以通过构建项目报告或访问与项目组合相关联的项目来查找等待业务案例审批的项目。

  有关项目组合的详细信息，请参阅文章[Adobe Workfront中的Portfolio概述](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

## 通过构建项目报告审批业务案例

您可以为项目构建报告，以查看哪些项目需要其业务案例获得批准。

要为等待其业务案例审批的项目构建报告，请执行以下操作：

1. 创建项目报告。

   有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 选择报告的&#x200B;**视图**&#x200B;选项卡，然后单击&#x200B;**添加列**。

1. 开始在&#x200B;**显示在此列**&#x200B;字段中键入“Status”，并在该字段出现在列表中时将其选中。

   此列将显示项目的状态。

1. 选择报告的&#x200B;**筛选器**&#x200B;选项卡，然后单击&#x200B;**添加筛选器规则**。

1. 开始在&#x200B;**仅向我显示……**&#x200B;字段中键入“状态”，并在该字段出现在列表中时将其选定。
1. 为筛选器修饰符选择&#x200B;**等于**。
1. 在可用字段中开始键入“Requested”。

   这可确保报表仅包含处于已请求状态的项目。

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. （可选）单击&#x200B;**添加其他筛选器规则**。

   您可以添加其他过滤器，以仅显示您是项目所有者、项目发起人或Portfolio所有者的项目。

   例如，您可以使用以下filter语句：

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   显示您指定为项目发起人的项目

   ```
   Project Owner ID Equals $$USER.ID
   ```

   显示您指定为项目所有者的项目

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   以显示您指定为Portfolio Manager的位置。

1. 单击&#x200B;**保存+关闭**。

   请注意，报告中的所有项目都处于&#x200B;**已请求**&#x200B;状态。

1. 单击报表中项目的名称以将其打开。
1. 单击左侧面板中的&#x200B;**业务案例**。
1. 在业务案例摘要区域单击&#x200B;**批准**&#x200B;或&#x200B;**拒绝**&#x200B;以批准或拒绝业务案例。

   &lt;！—![商业论证](assets/business-case-summary-with-rp-information--1-.png)—>

   如果业务案例获得批准，项目状态将更改为&#x200B;**已批准**。

   如果业务案例被拒绝，项目状态将更改为&#x200B;**已拒绝**。

   >[!NOTE]
   >
   >没有通知可提醒提交业务案例批准的用户其项目请求是否被批准或拒绝。

## 通过访问项目组合中请求的项目批准业务案例

有关审阅请求项目的详细信息，请参阅文章[审阅请求的项目](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md)。
