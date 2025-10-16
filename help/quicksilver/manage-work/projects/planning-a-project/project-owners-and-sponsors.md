---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: 项目所有者和发起人概览
description: 您可以为项目指定项目所有者和项目发起人。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 项目所有者和赞助者概述

<!-- Audited: 1/2024 -->

您可以为项目指定项目所有者和项目发起人。

项目所有者是负责按时和按预算完成项目的个人。

项目发起人是项目的重要利益相关者，拥有项目资源投资。 项目的完成通常有益于项目发起人。

有关如何更新项目的项目所有者或发起人的信息，请参阅[更新项目所有者和发起人](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md)。

## 项目所有者

您可以通过指定项目或模板上的项目所有者来指定项目经理。

您只能为项目定义一个项目所有者。

使用“项目所有者”字段可以执行以下操作：

* 您只能指定一个用户作为项目所有者。
* 您可以指定项目所有者作为项目的小时批准者。
* 在定义项目、任务或问题审批流程时，您可以将项目责任人指定为通用审批人。 有关审批的信息，请参阅[编辑审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)。

  >[!IMPORTANT]
  >
  >当您将审批分配给项目责任人，并且没有指定任何人为项目责任人时，审批将重新分配给主要Workfront管理员，如设置区域的客户信息部分所述。 有关信息，请参阅[配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
  >


* 您可以启用仅交付给项目所有者的某些通知。

  有关电子邮件通知的更多信息，请参阅[为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify)一文中的[为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)部分。

* 您可以在报告或列表中显示“项目所有者”字段。

  您还可以在视图、分组或提示中显示项目所有者字段。

  例如，您可以将以下文本模式表达式复制到过滤器中，以显示已登录用户拥有的项目：

  ```
  ownerID=$$USER.ID
  ```

有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE: drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 项目发起人

您可以将系统中的任何用户指定为项目发起人。 项目发起人通常是需要了解项目情况的经理、执行人员或利益相关者。

在分配项目发起人时，请考虑以下事项：

* 项目发起人不再获得对项目的任何其他访问权限，而是添加到项目的电子邮件通知中。 有关通知的信息，请参阅文章[为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

* 您只能指定一个项目发起人。
* 在定义项目、任务或问题批准流程时，您可以将项目发起人指定为通用批准者。 有关审批的信息，请参阅[编辑审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)。

  >[!IMPORTANT]
  >
  >当您将审批分配给项目发起人并且没有人被指定为项目发起人时，审批将重新分配给项目所有者。 如果没有指定任何人为项目的所有者，则会将审批分配给Workfront管理员。

* 您可以在报告或列表中显示项目发起人字段。

  您还可以在视图、分组或提示中显示项目发起人字段。

  例如，您可以将以下文本模式表达式复制到过滤器中，以显示由登录用户赞助的项目：

  ```
  sponsorID=$$USER.ID
  ```



  有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
