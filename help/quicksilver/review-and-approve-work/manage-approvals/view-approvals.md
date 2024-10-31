---
product-area: projects
navigation-topic: approvals
title: 查看审批
description: 批准流程提供了灵活性，可以为项目、任务和问题创建多步批准。 Adobe Workfront管理员定义审批流程，以在整个系统中提供一致性。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: b0b83e8a8a2a076ec20691183605e3d25d10129d
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 查看审批

批准流程提供了灵活性，可以为项目、任务和问题创建多步批准。 Adobe Workfront管理员定义审批流程，以在整个系统中提供一致性。

有关创建审批流程的信息，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

有关将审批与Workfront中的工作关联的信息，请参阅[将新的或现有的审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问与审批关联的对象</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看与审批关联的对象的权限或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 在Adobe Workfront中查找批准

您可以从Workfront的多个区域查看或管理审批。 有关如何管理各个领域的审批的信息，请参阅[审批工作](../../review-and-approve-work/manage-approvals/approving-work.md)。

您可以从以下区域查看或管理审批：

* 在“主页”区域

   * 所有等待您审批的项目、任务、问题、时间表、文档和访问权限都将显示在主页区域的“我的审批”小组件中。
   * 当您选择我已提交的审批过滤器选项时，您自己提交的审批也会显示在主页区域的我的审批小部件中。 有关详细信息，请参阅本文中“主页”区域](#review-work-you-submit-for-approval-in-the-home-area)部分中的[审核您提交供审批的工作。
   * 当关联的项目、任务或问题标记为“已解决”、“已搁置”、“已关闭”或“已取消”时，审批将从“主页”区域的“我的审批”构件中删除。

  有关使用主页的信息，请参阅[主页入门](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md)。

* 在项目、任务、问题、文档或验证的标题中
* 在项目、任务或问题的审批部分
* 在报表中

  >[!NOTE]
  >
  >您无法对报表的批准做出决定。

  您可以创建包含批准信息的项目、任务、问题或文档批准报告。

  有关创建报告的信息，请参阅[创建自定义报告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 在“主页”区域查看您提交以供审批的工作 {#review-work-you-submit-for-approval-in-the-home-area}

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）单击&#x200B;**自定义**&#x200B;以添加&#x200B;**我的审批**&#x200B;小组件。
1. （视情况而定）单击&#x200B;**筛选器**&#x200B;下拉菜单，然后选择&#x200B;**我已提交的审批**&#x200B;以查看您提交的审批。


## 查看对象的审批状态

您可以在对象的以下部分中查看对象的批准状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">更新 </td> 
   <td> <p>发生时显示所有审批状态。 审批状态与<strong>更新</strong>部分中显示的其他状态一致。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">审批</td> 
   <td> <p>显示有关审批流程的更多详细信息，例如审批流程的每个阶段以及审批者是否已授予审批。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 使用更新区域查看审批状态 {#use-the-updates-area-to-view-an-approval-status}

对项目、任务或问题启动审批后，对象的&#x200B;**更新**&#x200B;选项卡中将显示一个状态，指示审批状态。 每当对象通过审批流程过渡时，都会显示新状态。 这包括以下事件：

* 对对象启动批准流程。 当状态更改时，将启动审批流程。
* 对象被拒绝
* 对象已批准

>[!TIP]
>
>如果将批准应用于任务，则批准更新会显示在任务的“更新”选项卡上，而不是显示在任务所在项目的“更新”选项卡上。

### 使用审批区域查看审批状态 {#use-the-approvals-area-to-view-an-approval-status}

您可以查看您当前处理的任务或问题在批准流程中的位置。 您可以看到以下信息：

* 批准流程的阶段
* 哪些批准者已批准它
* 哪些批准者尚未批准它

要查看任务或问题在审批流程中的当前状态，请执行以下操作：

1. 转到与审批关联的项目、任务或问题。
1. 在左侧面板中，单击&#x200B;**审批**。 您可能需要先单击&#x200B;**显示更多**。

   “审批”选项卡显示所有过去审批路径和阶段的完整信息。 您可以准确地查看对批准做出决定的用户，或者是否为团队、工作角色或用户设置了批准。

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   有关创建批准流程的信息，请参阅[为工作项创建批准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。
