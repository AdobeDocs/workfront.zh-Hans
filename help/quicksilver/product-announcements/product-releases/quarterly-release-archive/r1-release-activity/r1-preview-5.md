---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览5
description: 本页介绍R1 Preview 5版本的预览环境中所有可用的更改。 此页面上的功能于2017年3月16日在预览环境中提供。
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# R1预览5

本页介绍R1 Preview 5版本的预览环境中所有可用的更改。 此页面上的功能于2017年3月16日在预览环境中提供。

有关R1中所有更改的列表，请参阅 [R1发行活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## 使用使用情况报表跟踪项目进度

现在，对项目具有“管理”访问权限的用户可以通过使用情况报告跟踪项目的进度。

利用率报表，您可以快速查看实际小时数如何跟踪给定周或月的预算小时数或计划小时数，或整个项目的实际小时数，从而使您的项目保持在预算范围内。 此外，您还可以查看按职务职责或个人用户分类的每个类别（预算、计划和实际）中小时数的详细信息。

有关跟踪项目中利用率的更多信息，请参阅 [资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

作为系统管理员，您可以配置“利用率”选项卡是否可供用户使用。 默认情况下，“利用率”选项卡位于项目的“更多”下拉菜单中。 您可以将“利用率”选项卡移动到其他位置，或完全隐藏。 如果您为组织中的用户定义了自定义布局模板，则需要手动将“利用率”选项卡添加到自定义布局模板。

有关配置“利用率”选项卡位置的更多信息，请参阅“创建和管理布局模板”中的“自定义选项卡”。

## 修改单个对象的现有全局批准流程

现在，当您将全局批准流程与对象关联时，可以修改现有的全局批准流程。 您所做的修改仅应用于要关联对象的审批流程。

有关更多信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [将新审批流程或现有审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## 配置报表以默认显示新甘特图

您可以配置您创建的项目和任务报表，以在默认情况下显示新的甘特图，并使用新选项“默认在甘特视图中显示此报表”。

有关配置报表以显示新甘特图的详细信息，请参阅 [编辑报表设置](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

有关在项目报表和任务报表中查看甘特图的详细信息，请参阅 [在甘特图中查看信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; [在甘特图中查看信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## 回收站改进：任务和子任务将恢复为其上一顺序

现在，当您在删除某个任务或子任务后恢复该任务或子任务时，该任务或子任务将恢复到其先前位置（在任务列表中或父任务下），其顺序与删除前显示的顺序相同。

在进行此项更改之前，已还原的任务和子任务始终作为最后一项任务（在任务列表中或在父任务下）进行还原，而不管它们在被删除之前显示的顺序如何。

有关在Workfront中恢复对象的更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 里程碑视图改进

现在，在“里程碑”视图中查看项目列表或项目报表时，可以使用以下改进功能：

* **配置视图中是否显示进度状态和完成百分比：** 新选项允许您配置进度状态图标是否显示在里程碑视图中。 此外，您还可以配置是否显示与项目和任务相关的完成百分比信息。\
   有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **直接从“里程碑”视图编辑完成百分比：** 现在，您可以直接从“里程碑”视图编辑项目和任务的完成百分比。\
   有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## 更新了多个系统设置页面的外观

“设置”区域的“系统”菜单中的以下页面的外观已更新（功能保持不变）：

* 诊断
* 单点登录(SSO)，包括：

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* 更新 SSO 的用户

## 更新了“电子邮件设置”区域中的事件通知分组

“电子邮件设置”区域中事件通知的组织标题现在与用户配置文件设置区域中使用的章节标题相匹配。

有关事件通知的更多信息，请参阅  [为系统中的每个人配置事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## 选择退出即时通知：上下文内摘要配置

现在，即时电子邮件通知中提供了以下选项。 这些选项仅适用于同时具有每日摘要的即时通知：

* “将此项添加至每日摘要”
* &quot;停止此类型的电子邮件&quot;

现在，当您收到即时电子邮件通知时，您可以将该通知添加到每日摘要通知中，也可以完全取消该通知的订阅。

这些选项在电子邮件通知中可用。 有关接收电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)

## 各种电子邮件通知已从“需要的操作”部分移至其他与项目相关的部分

已将多个通知从用户配置文件页面的“需要的操作”部分移至其他部分，如下所示：

有关配置电子邮件通知的更多信息，请参阅 [激活或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>通知</strong> </th> 
   <th><strong>旧区域</strong> </th> 
   <th><strong>新建区域</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>在添加问题之后，发送电子邮件给项目所有者。</td> 
   <td> <p> 需要操作 </p> </td> 
   <td>   <p>“我拥有的项目”相关信息</p></td> 
  </tr> 
  <tr> 
   <td>在添加问题之后，发送电子邮件给团队。</td> 
   <td>   <p>需要操作</p><p> </p></td> 
   <td> <p> “我拥有的项目”相关信息 </p>   </td> 
  </tr> 
  <tr> 
   <td>在添加未分配问题之后，发送电子邮件给项目所有者。</td> 
   <td>   <p>需要操作</p></td> 
   <td>   <p>“我拥有的项目”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 在添加未分配问题之后，发送电子邮件给团队。 </p> </td> 
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
   <td> <p> 当任务的计划完成日期改变时，向被分派的用户发送电子邮件 </p> </td> 
   <td>   <p>需要操作</p></td> 
   <td>   <p>“分配给我的工作”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 当问题的计划完成日期改变时，向被分派的用户发送电子邮件 </p> </td> 
   <td> <p> 需要操作 </p>   </td> 
   <td>   <p>“分配给我的工作”相关信息</p></td> 
  </tr> 
  <tr> 
   <td> <p> 有关我已分配到的任务的状态已更改 </p>   </td> 
   <td> <p> 需要操作 </p>   </td> 
   <td> <p> “分配给我的工作”相关信息 </p>   </td> 
  </tr> 
 </tbody> 
</table>

## 新的资源规划功能（在R1的生产中不可用）

>[!NOTE]
>
>当前，预览环境中提供了此功能。 在将R1版本发布到生产环境大约一个月之前，它将从预览环境中删除。 然后，将重新将其引入到R2预览1中的预览环境。

 

为支持将来的资源规划功能，添加了以下更改：

* “人员”区域中当前的“资源计划”选项卡已重命名为“旧版资源计划”。 
* 在将开发新功能的“人员”区域中引入了新的“资源规划”选项卡。\
   有关新的“资源计划”选项卡的详细信息，请参阅 [资源规划入门](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* 当前“资源池”对象已重命名为“旧版资源池”。\
   有关创建新的基于用户的资源池的详细信息，请参阅 [资源池概述](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* 已创建新的“资源池”对象以支持新的（基于用户的）资源池。

   >[!NOTE]
   * 如果您当前正在现有旧版资源池上运行报表，则现有报表不会发生更改。
   * 如果要为现有（基于作业角色的）旧版资源池创建新报表，则需要选择“旧版资源池”作为报表的对象。
   * 如果要为新的（基于用户的）资源池创建新报表，则需要选择“资源池”作为报表的对象。

  >   
