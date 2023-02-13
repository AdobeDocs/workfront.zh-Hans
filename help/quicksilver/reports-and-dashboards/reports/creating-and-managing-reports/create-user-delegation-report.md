---
product-area: reporting
keywords: 用户，委派，报表，委派，批准
navigation-topic: create-and-manage-reports
title: 创建用户委派报表
description: 创建用户委派报表
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# 创建用户委派报表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

在Adobe Workfront中，用户可以将项目、任务和发布批准委派给其他用户，以确保在用户不在办公室时对其批准进行管理。 具有计划许可证的用户可以创建用户委派报告，以查看：

* 已将其任务、问题和项目批准委派给其他用户的人员
* 哪些用户已将委派的任务、问题和项目批准分配给他们

* 代表团开始和结束的日期

要了解有关委派批准的更多信息，请参阅 [委派批准请求](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

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
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看授权项目和授权涉及的用户的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建用户委派报告

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.

1. 单击 **新建报表**，然后选择 **用户委派**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   默认情况下，此报表中会显示以下字段：

   | 字段 | 描述 |
   |---|---|
   | **来自用户** | 这是将其任务、问题和项目批准委派给其他用户的用户。 |
   | **至用户** | 该用户具有委派给他们的任务、问题和项目批准。 |
   | **开始** | 对于已进行委派的用户而言，这是外出时间的开始。 |
   | **结束** | 对于已进行委派的用户而言，这是离职时间的结束。 |

   {style=&quot;table-layout:auto&quot;}

1. （可选）在报表生成器中，修改以下内容：

   * 列
   * 分组
   * 过滤器
   * 图表

   要进一步了解这些功能，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 完成生成报告后，单击 **保存并关闭**.

1. 在 **报表名称** 字段，然后单击 **保存报表**.

   此时将显示报表。
