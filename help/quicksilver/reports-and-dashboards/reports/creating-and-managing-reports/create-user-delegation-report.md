---
product-area: reporting
keywords: 用户，委派，报告，委派，批准
navigation-topic: create-and-manage-reports
title: 创建用户委派报告
description: 创建用户委派报告
author: Courtney
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/xauKU-ASfnD7MiuqK-t9h-JGiTTlcVmzFL-pofZOPJ8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 7%

---

# 创建用户委派报告

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

在Adobe Workfront中，用户可以将项目、任务和问题审批委派给其他用户，以确保在外出时管理其审批。 具有Standard或Plan许可证的用户可以创建用户委派报告，以查看：

* 已将其任务、问题和项目审批委托给其他用户的用户
* 哪些用户已委派任务、问题和项目审批给他们

* 委派开始和结束的日期

要了解有关委托审批的更多信息，请参阅[委托审批请求](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>标准</p>
      <p>规划</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
 <td> <p>查看被委派审批的项和委派中涉及的用户的权限</p></td>  
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建用户委派报告

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。

1. 单击&#x200B;**新建报告**，然后选择&#x200B;**用户委派**。

   ![新报告用户委派](assets/classic-new-report-user-delegation-350x644.png)

   默认情况下，此报表中显示以下字段：

   | 字段 | 描述 |
   |---|---|
   | **来自用户** | 该用户正在将其任务、问题和项目审批委派给其他用户。 |
   | **至用户** | 这是具有委托给他们的任务、问题和项目审批的用户。 |
   | **开始日期** | 对于进行委派的用户来说，这是外出时间的开始。 |
   | **结束日期** | 对于进行委派的用户而言，这是外出时间的结束。 |

   {style="table-layout:auto"}

1. （可选）在Report Builder中，修改以下内容：

   * 列（视图）
   * 分组
   * 过滤器
   * 图表

   若要了解有关这些功能的更多信息，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 完成报表生成后，单击&#x200B;**保存+关闭**。

   此时将显示报表。
