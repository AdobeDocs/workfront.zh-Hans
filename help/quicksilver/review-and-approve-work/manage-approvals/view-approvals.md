---
product-area: projects
navigation-topic: approvals
title: 查看批准
description: 审批流程为项目、任务和问题创建多步审批提供了灵活性。 Adobe Workfront管理员可定义批准流程以在整个系统中保持一致性。
author: Courtney
feature: Work Management
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 查看批准

审批流程为项目、任务和问题创建多步审批提供了灵活性。 Adobe Workfront管理员可定义批准流程以在整个系统中保持一致性。

有关创建审批流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

有关将审批与Workfront中的工作关联的信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

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
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问与批准关联的对象</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看或更高对与批准关联的对象的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在Adobe Workfront中查找批准

您可以查看或管理Workfront多个区域的批准。 有关如何管理各个区域的审批的信息，请参阅 [批准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

您可以从以下区域查看或管理批准：

* 在主区

   * 选择查看“全部”或“批准”时，所有等待您批准的项目、任务、问题、时间表、文档和访问都会显示在“主页”区域。
   * 您自行提交的批准也会显示在工作列表的“Home”（主页）区域的“Approvals I&#39;ve Submitted”（我已提交的批准）部分。 有关更多信息，请参阅 [在“主页”区域查看您提交以供审批的工作](#review-work-you-submit-for-approval-in-the-home-area) 章节。
   * 将关联的项目、任务或问题标记为“已解决”、“暂挂”、“关闭”或“已取消”时，将从“主页”区域中删除批准。

   有关使用主页的信息，请参阅 [开始使用Home](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* 在项目、任务、问题、文档或校样的标题中
* 在项目、任务或问题的“批准”部分
* 在报表中

   >[!NOTE]
   >
   >您无法从报表中对批准做出决定。

   您可以创建包含审批信息的项目、任务、发放或单据审批报表。

   有关创建报表的信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 在“主页”区域查看您提交以供审批的工作 {#review-work-you-submit-for-approval-in-the-home-area}

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   >* 将其替换为自定义的图像，以说明您的组织。 在这种情况下，图标将与本文中显示的不同。
   >* 将链接到该页面的页面替换为其他页面。 在这种情况下，单击 **主菜单** ![](assets/main-menu-icon.png) ，然后单击 **主页**.


1. 选择 **工作列表**，然后单击 **过滤器** 下拉菜单，然后选择 **批准**.
1. 展开 **我已提交的批准** ，然后查找您提交的批准。

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## 查看对象的批准状态

您可以在对象的以下部分中查看对象的批准状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">更新 </td> 
   <td> <p>显示所有审批状态。 审批状态与 <strong>更新</strong> 中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">审批</td> 
   <td> <p>显示有关批准流程的更详细信息，如批准流程的每个阶段以及批准者是否已批准。</p> </td> 
  </tr> 
 </tbody> 
</table>

* [使用“更新”区域查看批准状态](#use-the-updates-area-to-view-an-approval-status)
* [使用“审批”区域可查看审批状态](#use-the-approvals-area-to-view-an-approval-status)

### 使用“更新”区域查看批准状态 {#use-the-updates-area-to-view-an-approval-status}

在对项目、任务或问题启动审批后， **更新** 选项卡，以指示批准状态。 每当对象在审批流程中转换时，都会显示新状态。 这包括以下事件：

* 对对象启动批准流程。 当状态发生更改时，将启动审批流程。
* 对象被拒绝
* 对象已获批准 

>[!TIP]
>
>如果对任务应用了批准，则批准更新会显示在任务的“更新”选项卡中，而不是显示在任务所在项目的“更新”选项卡中。

### 使用“审批”区域可查看审批状态 {#use-the-approvals-area-to-view-an-approval-status}

您可以查看当前正在处理的任务或问题在审批流程中的位置。 您可以看到以下信息：

* 审批流程的阶段
* 哪些批准者已经批准了
* 哪些批准者尚未批准

要查看任务或问题在审批流程中所处的当前状态，请执行以下操作：

1. 转到与审批关联的项目、任务或问题。
1. 在左侧面板中，单击 **批准**. 您可能需要先单击 **显示更多**.

   “批准”选项卡显示有关所有过去批准路径和阶段的完整信息。 您可以确切地看到谁对批准做出了决策，或者是为团队、职务角色还是用户设置了批准。

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   有关创建审批流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
