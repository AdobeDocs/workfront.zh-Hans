---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: 项目所有者和赞助者概述
description: 您可以为项目指定项目所有者和项目赞助商。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 项目所有者和赞助者概述

您可以为项目指定项目所有者和项目赞助商。

项目责任人是负责按时按预算完成项目的个人。

项目赞助者是该项目的重要利益相关方，该项目有资源投资于该项目。 项目的完成通常使项目发起人受益。

有关如何更新项目所有者或赞助商的信息，请参阅 [更新项目所有者和赞助者](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## 项目所有者

您可以通过在项目或模板上指定项目所有者来指定项目经理。

您只能为项目定义一个项目所有者。

使用“项目所有者”字段可以执行以下操作：

* 您只能指定一个用户作为项目所有者。
* 您可以将项目所有者指定为项目的小时数审批者。
* 在定义项目、任务或发放审批流程时，您可以将项目责任人指定为通用审批者。 有关批准的信息，请参阅 [编辑批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >如果您为项目所有者分配了批准，并且没有人被指定为项目所有者，则该批准将重新分配给主Workfront管理员，如“设置”区域的“客户信息”部分中所述。 有关信息，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* 您可以启用某些仅发送给项目所有者的通知。

   有关电子邮件通知的更多信息，请参阅部分 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) 在文章中 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您可以在报表或列表中显示项目所有者字段。

   您还可以在视图、分组或提示中显示“项目所有者”字段。

   例如，您可以将以下文本模式表达式复制到过滤器中，以显示登录用户拥有的项目： 

   ```
   ownerID=$$USER.ID
   ```

有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 项目赞助商

您可以将系统中的任何用户指定为项目赞助商。 项目赞助商通常是需要了解项目进展情况的经理、执行官或利益相关方。

在分配项目赞助商时，请考虑以下事项：

* 项目赞助商不会获得对项目的任何其他访问权限，但会添加到项目的电子邮件通知中。 有关通知的信息，请参阅文章 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您只能指定一个项目赞助商。
* 在定义项目、任务或发放审批流程时，您可以将项目主办者指定为通用审批者。 有关批准的信息，请参阅 [编辑批准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >当您为项目发起人分配了批准，并且没有人被指定为项目的发起人时，批准将重新分配给项目所有者。 如果没有人指定为项目所有者，则会将批准分配给Workfront管理员。

* 您可以在报表或列表中显示项目赞助商字段。

   您还可以在视图、分组或提示中显示项目赞助商字段。

   例如，您可以将以下文本模式表达式复制到过滤器中，以显示登录用户赞助的项目：

   ```
   sponsorID=$$USER.ID
   ```

    

   有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
