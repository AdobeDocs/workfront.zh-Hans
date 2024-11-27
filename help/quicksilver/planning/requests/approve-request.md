---
title: 批准请求
description: 当用户将请求提交到与Adobe Workfront Planning中的批准关联的请求表单时，批准者会收到有关未决批准的通知，并收到电子邮件。 他们必须先批准请求，Workfront Planning才能创建对象。
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 1%

---


<!--

---
title: Approve a Request
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->


# 批准请求

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

当用户将请求提交到与Adobe Workfront Planning中的批准关联的请求表单时，批准者会收到有关未决批准的通知，并收到电子邮件。 他们必须先批准请求，Workfront Planning才能创建对象。

本文介绍了工作区管理员如何批准提交给Workfront Planning的请求以创建记录。

我们建议您也查看以下文章：

* [在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)
* [提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)
* [向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## 有关批准请求和请求状态的注意事项

已提交的请求将显示在Workfront请求区域的已提交部分的“计划”选项卡中，并具有以下请求状态之一：

* **等待审阅**：当没有批准者打开请求对象时，将显示此状态。
* **审核中**：至少有一个批准者打开请求对象时，状态将更改为&#x200B;**审核中**。
* **已批准**：当批准者批准请求对象时，其个人状态将变为
* **已批准**，但在所有批准者做出决定之前，整体请求对象状态仍为&#x200B;**正在审核**。
* **已完成**：如果所有批准者都批准该请求对象，则其状态将更改为&#x200B;**已完成**，或者该请求不需要批准。
* **已拒绝**：如果任何审批者拒绝请求对象，则状态将变为&#x200B;**已拒绝**。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront规划<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront计划*</p></td>
   <td>
<p>以下任意Workfront计划：</p>
<ul><li>选择</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning不适用于旧版Workfront计划</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td>
   <td>
<p>任何 </p>  
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <ul>
   <li><p>管理工作区的权限</p></li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    </ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 批准创建记录的请求

用户将请求添加到与批准关联的记录类型请求表单后，该请求将发送给批准者。

批准者将收到有关待其批准的请求的以下通知：

* 应用程序内通知
* 电子邮件通知

要批准请求，请执行以下操作：

1. 执行下列操作之一：

   * 从屏幕右上角的Workfront **主菜单** ![](assets/dots-menu.png)或左上角的&#x200B;**主菜单** ![](assets/lines-menu.png)（如果可用），单击&#x200B;**请求** > **已提交** > **计划**，然后单击状态为&#x200B;**正在审核**&#x200B;的请求<!--did they change this to Pending approval; logged  a bug-->。
   * 转到屏幕右上角的&#x200B;**通知**&#x200B;区域，然后单击有关待您审批的请求的通知以打开该请求。
   * 转到电子邮件中的电子邮件通知，通知您有关待审批的请求，然后单击以打开该请求。<!--add the name of the button here, from the email-->

   请求页面将以只读模式打开。

   ![](assets/read-only-reqeust-page-in-review-status.png)
1. （可选）单击请求右上角的&#x200B;**批准**&#x200B;图标![](assets/approvals-icon.png)以查看批准者。
1. 单击&#x200B;**审核并批准**，然后选择以下选项之一： <!--did they fix the button and removed the &??-->

   * **批准**：批准该请求。 将立即为与请求表单关联的记录类型创建记录。
   * **拒绝**：拒绝请求。 没有为与请求表单关联的记录类型创建记录。<!--check to see if there is a notification sent to the requestor about it being rejected OR approved??-->
