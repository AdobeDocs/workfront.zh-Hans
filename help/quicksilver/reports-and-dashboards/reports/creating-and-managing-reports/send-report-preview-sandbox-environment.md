---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在“预览Sandbox”环境中发送报告
description: 此页面上的信息介绍了仅在“预览”和“自定义刷新沙盒”环境中可用的功能。 此功能在生产环境中不可用。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 在“预览Sandbox”环境中发送报告

此页面上的信息介绍了仅在“预览”和“自定义刷新沙盒”环境中可用的功能。 此功能在生产环境中不可用。

您可以在任何Adobe Workfront测试环境中设置报表交付选项。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

虽然测试环境的功能应该尽可能接近您的生产环境，但一些功能与您的生产环境不同。

您可以在测试环境中计划报表，但提交报表的方式与从生产环境中提交报表的方式有所不同。

有关在生产环境中计划报表交付的信息，请参阅[报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

根据计划报表的位置，预览沙箱和自定义刷新沙箱中的交付功能有所不同。

## 访问要求

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在预览环境中计划报表

* [在预览环境中计划报表](#schedule-reports-in-the-preview-environment)

### 在预览环境中计划报表

是否在“预览”环境中生成传递的报告取决于&#x200B;**是否启用从此测试环境接收电子邮件**。

有关从沙盒环境启用电子邮件的信息，请参阅[从预览沙盒环境启用电子邮件投放](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在“预览”环境中计划报表交付的过程与在“生产”环境中计划报表的过程相同。 有关计划报表提交的信息，请参阅[报表提交概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

在预览环境中计划报表交付时，存在以下情况：

* 当对接收报告的用户禁用&#x200B;**从此测试环境接收电子邮件**&#x200B;时，在计划提交报告时不会生成任何文件。
* 为接收报告的用户启用&#x200B;**从此测试环境接收电子邮件**&#x200B;后，在计划报告提交时生成的文件将添加到用户的“文档”选项卡中。

## 在自定义刷新沙盒环境中计划报表

是否在自定义刷新沙盒中生成交付的报表取决于是否启用从此测试环境接收电子邮件设置。

有关从预览环境启用电子邮件的信息，请参阅[修改自己的电子邮件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)一文中的[查看和修改电子邮件通知设置](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view)部分。

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

在自定义刷新沙盒环境中计划报表的提交与在生产环境中计划报表相同。 有关计划报表提交的信息，请参阅[报表提交概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

在自定义刷新沙盒环境中计划报表交付时，存在以下情况：

* 当接收报告的用户禁用从此测试环境接收电子邮件时，在计划报告交付时不会生成任何文件。
* 为接收报告的用户启用从此测试环境接收电子邮件后，报告将作为附件通过电子邮件发送到与该用户关联的电子邮件地址。

## 如何通知外部用户

外部用户不会收到从Workfront测试环境发送的报告，也不会收到电子邮件通知。

仅当外部用户是从生产环境交付报告时，才会收到通过电子邮件发送的报表。
