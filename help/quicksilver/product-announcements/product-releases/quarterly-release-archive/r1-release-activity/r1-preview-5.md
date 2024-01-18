---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览5
description: 本页介绍R1 Preview 5版本在Preview环境中可用的所有更改。 2017年3月16日，预览环境中提供了此页面上的功能。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 13%

---

# R1预览5

本页介绍R1 Preview 5版本在Preview环境中可用的所有更改。 2017年3月16日，预览环境中提供了此页面上的功能。

有关在R1中所做所有更改的列表，请参见 [R1发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## 使用利用率报告跟踪项目进度

现在，具有项目管理访问权限的用户可以使用利用率报告跟踪项目进度。

利用利用率报表，您可以快速查看在给定周或月或整个项目中，实际小时数是如何与预算小时数或计划小时数进行跟踪的，从而让项目保持在预算范围之内的。 此外，您还可以查看按工作角色或个人用户分类的每个类别（预算、计划和实际）中的小时数的详细信息。

有关跟踪项目中利用率的详细信息，请参阅 [资源利用率报表概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

作为系统管理员，您可以配置用户是否可以使用“利用率”选项卡。 默认情况下，“利用率”选项卡位于项目的“更多”下拉菜单中。 您可以将“利用率”选项卡移动到其他位置，也可以完全隐藏该选项卡。 如果您为组织中的用户定义了自定义布局模板，则需要手动将“利用率”选项卡添加到自定义布局模板。

有关配置“利用率”选项卡位置的更多信息，请参阅创建和管理布局模板中的“自定义选项卡”。

## 修改单个对象的现有全局批准流程

现在，当您将全局批准流程与对象关联时，可以修改现有的全局批准流程。 您所做的修改仅适用于关联该对象的审批流程。

有关更多信息，请参阅 [将新的或现有的审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) 在 [将新的或现有的审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## 配置报告以默认显示新的甘特图

您可以将创建的项目和任务报告配置为默认显示新的甘特图，并使用新选项“默认在甘特图中显示此报告”。

有关配置报表以显示新甘特图的更多信息，请参阅 [编辑报表设置](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

有关在项目报告和任务报告中查看甘特图的更多信息，请参阅 [在甘特图中查看信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的&quot; [在甘特图中查看信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## 回收站改进：任务和子任务恢复为之前的顺序

现在，当您在删除任务或子任务后恢复该任务或子任务时，该任务或子任务将恢复至其先前位置（位于任务列表中或父任务下方），恢复顺序与删除前显示的顺序相同。

在此更改之前，已恢复的任务和子任务始终恢复为最后一个任务（在任务列表中或父任务下方），无论它们在被删除前出现的顺序如何。

有关在Workfront中恢复对象的更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 里程碑视图改进

在“里程碑”视图中查看项目列表或项目报告时，现在有以下改进可用：

* **配置是否在视图中显示“进度状态”和“完成百分比”：** 新选项允许您配置进度状态图标是否显示在里程碑视图中。 此外，您还可以配置是否显示与项目和任务相关的完成百分比信息。\
  有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) 在 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **直接从“里程碑”视图中编辑完成百分比：** 现在，您可以直接从“里程碑”视图中编辑项目和任务的完成百分比。\
  有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) 在 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## 更新了多个系统设置页面的外观

“设置”区域的“系统”菜单中的以下页面的外观和感觉已更新（功能保持不变）：

* 诊断
* 单点登录(SSO)包括：

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* 更新 SSO 的用户

## 更新了“电子邮件设置”区域中的事件通知分组

电子邮件设置区域中事件通知的组织标题现在与用户配置文件设置区域中使用的部分标题匹配。

有关事件通知的更多信息，请参阅  [为系统中的每个人配置事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## 选择退出即时通知：上下文摘要配置

现在，即时电子邮件通知中提供了以下选项。 这些选项仅适用于同时具有每日摘要对应项的即时通知：

* “将此项添加到每日摘要”
* “停止此类型的电子邮件”

现在，当您收到即时电子邮件通知时，您可以将该通知添加到每日摘要通知中，也可以完全取消订阅该通知。

这些选项在电子邮件通知中可用。 有关接收电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)

## 各种电子邮件通知已从“需要操作”部分移至其他与项目相关的部分

一些通知已从用户配置文件页面的“需要操作”部分移动到其他部分，如下所示：

有关配置电子邮件通知的更多信息，请参阅 [修改您自己的电子邮件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>通知</strong> </th> 
   <th><strong>旧分区</strong> </th> 
   <th><strong>新建分区</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>在添加问题之后，发送电子邮件给项目所有者。</td> 
   <td> <p> 需要操作 </p> </td> 
   <td>   <p>“我拥有的项目”相关信息</p></td> 
  </tr> 
  <tr> 
   <td>我参与的项目已添加一个问题</td> 
   <td>   <p>需要操作</p><p> </p></td> 
   <td> <p> “我拥有的项目”相关信息 </p>   </td> 
  </tr> 
  <tr> 
   <td>在添加未分配问题之后，发送电子邮件给项目所有者。</td> 
   <td>   <p>需要操作</p></td> 
   <td>   <p>“我拥有的项目”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我参与的项目添加了一个未分派问题 </p> </td> 
   <td> <p> 需要操作 </p>   </td> 
   <td> <p> “我拥有的项目”相关信息 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 当任务的提交日期改变时，向项目所有者发送电子邮件 </p> </td> 
   <td>   <p>需要操作</p></td> 
   <td>   <p>“我拥有的项目”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 当问题的提交日期改变时，向项目所有者发送电子邮件 </p>   </td> 
   <td>   <p>需要操作</p></td> 
   <td> <p> “我拥有的项目”相关信息 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 我被分派的一个任务的到期日期已更改 </p> </td> 
   <td>   <p>需要操作</p></td> 
   <td>   <p>“分配给我的工作”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我被分派的一个问题的到期日期更改了 </p> </td> 
   <td> <p> 需要操作 </p>   </td> 
   <td>   <p>“分配给我的工作”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我被分派的一个任务有状态更改 </p>   </td> 
   <td> <p> 需要操作 </p>   </td> 
   <td> <p> “分配给我的工作”相关信息 </p>   </td> 
  </tr> 
 </tbody> 
</table>

## 新的资源计划功能（在R1的生产中不可用）

>[!NOTE]
>
>此功能当前在“预览”环境中可用。 它将在R1发布到“生产”环境前大约一个月从“预览”环境中删除。 然后，它将被重新引入R2 Preview 1中的Preview环境。

 

添加了以下更改以支持未来的资源规划功能：

* 当前的“资源计划”选项卡已在人员区域重命名为“旧版资源计划”。 
* 在将要开发新功能的“人员”区域引入了新的“资源规划”选项卡。\
  有关新的“资源计划”选项卡的详细信息，请参阅 [资源规划入门](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* 当前的“资源池”对象已重命名为“旧版资源池”。\
  有关创建新的基于用户的资源池的详细信息，请参见 [资源池概述](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* 已创建新的“资源池”对象，以支持新的（基于用户的）资源池。

  >[!NOTE]
  >
  >
  >   
  >   
  * 如果您当前对现有旧版资源池运行报告，则现有报告将不会更改。
  * 如果要为现有（基于工作角色的）传统资源池创建新报告，则需要选择“传统资源池”作为报告的对象。
  * 如果要为新的（基于用户的）资源池创建新报告，则需要选择“资源池”作为报告的对象。
  >   
  >
