---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在预览沙盒环境中发送报表
description: 此页面上的信息是指仅在“预览”和“自定义刷新”沙盒环境中可用的功能。 此功能在生产环境中不可用。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 在预览沙盒环境中发送报表

此页面上的信息是指仅在“预览”和“自定义刷新”沙盒环境中可用的功能。 此功能在生产环境中不可用。

您可以在任何Adobe Workfront测试环境中设置“报表交付”选项。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

虽然测试环境可以尽可能接近生产环境，但某些功能与生产环境有所不同。

您可以在测试环境中计划报表，但报表的提交方式与在生产环境中交付报表的方式有所不同。

有关计划报表在生产环境中提交的信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

根据您计划报表的位置，“预览”和“自定义刷新”沙箱的提交功能会有所不同。

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
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在预览环境中计划报表

* [在预览环境中计划报表](#schedule-reports-in-the-preview-environment)

### 在预览环境中计划报表

是否在“预览”环境中生成已提交的报表取决于 **从此测试环境接收电子邮件** 是否启用。

有关启用来自沙盒环境的电子邮件的信息，请参阅 [允许从预览沙盒环境发送电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在“预览”环境中计划报表提交与在生产环境中计划报表相同。 有关计划报表提交的信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

在预览环境中计划报表提交时，会出现以下情况：

* When **从此测试环境接收电子邮件** 对于接收报表的用户，如果禁用，则在计划报表提交时不会生成任何文件。
* When **从此测试环境接收电子邮件** 为接收报表的用户启用了，则计划报表提交时生成的文件将添加到用户的“文档”选项卡中。

## 在自定义刷新沙盒环境中计划报表

是否在“自定义刷新”沙盒中生成投放的报表，取决于是否启用了从此测试环境接收电子邮件设置。

有关从预览环境启用电子邮件的信息，请参阅部分 [查看和修改电子邮件通知设置](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 在文章中 [激活或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在自定义刷新沙盒环境中计划报表交付的方式与在生产环境中计划报表的方式相同。 有关计划报表提交的信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

在自定义刷新沙盒环境中计划报表交付时，存在以下情况：

* 如果对于正在接收报表的用户禁用从此测试环境接收电子邮件，则在计划报表提交时不会生成任何文件。
* 为接收报表的用户启用从此测试环境接收电子邮件后，报表会通过电子邮件作为与用户关联的电子邮件地址的附件发送。

## 如何通知外部用户

外部用户不会收到从Workfront测试环境发送的报表，也不会收到电子邮件通知。

仅当外部用户从生产环境发送报表时，才会收到电子邮件报表。
