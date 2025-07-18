---
title: 在Adobe Workfront Planning中批准请求
description: 当用户将请求提交到与Adobe Workfront Planning中的批准关联的请求表单时，批准者会收到有关未决批准的通知，并收到电子邮件。 他们必须先批准请求，Workfront Planning才能创建对象。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 1%

---

# 在Adobe Workfront Planning中批准请求

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

当用户将请求提交到与Adobe Workfront Planning中的批准关联的请求表单时，批准者会收到有关未决批准的通知，并收到电子邮件。 他们必须先批准请求，Workfront Planning才能创建对象。

本文介绍了工作区管理员如何批准提交给Workfront Planning的请求以创建记录。

我们建议您也查看以下文章：

* [在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)
* [提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)
* [向请求表单添加批准](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## 有关批准请求的注意事项

* 已提交的请求将显示在Workfront请求区域的已提交部分的“计划”选项卡中，并具有以下请求状态之一：

   * **等待审阅**：当没有批准者打开请求对象时，将显示此状态。
   * **审核中**：当至少有一个批准者打开请求对象时，**待审核中**&#x200B;状态更改为&#x200B;**审核中**。 在所有批准者都批准请求之前，请求的状态保持为&#x200B;**正在审核**。
   * **已批准**：当批准者批准请求对象时，其单个状态将变为&#x200B;**已批准**，但整个请求对象状态将保持&#x200B;**正在审核**，直到所有批准者做出决定。 当所有批准者批准请求时，请求状态将变为&#x200B;**已批准**。
   * **已完成**：如果所有批准者都批准该请求对象，则其状态将更改为&#x200B;**已完成**，或者该请求不需要批准。
   * **已拒绝**：如果任何审批者拒绝请求对象，则状态将变为&#x200B;**已拒绝**。 不创建记录，必须提交新请求才能创建记录。

* <span class="preview">您可以通过在“批准者”和“批准日期”字段中提交请求表单，来显示所创建记录的批准信息。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。</span>

## 访问要求

+++ 展开以查看访问要求。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p>
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
   <li><p>管理对工作区和记录类型的权限 </p></li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    </ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
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

>[!NOTE]
>
>贵组织的Workfront实例必须载入到Adobe Unified Experience，用户才能接收电子邮件和应用程序内通知。

要批准请求，请执行以下操作：

1. 执行下列操作之一：

   * 如果您有权访问Workfront Planning并且可以查看至少一个工作区，请单击屏幕右上角的&#x200B;**主菜单** ![圆点主菜单](assets/dots-menu.png)，或单击左上角的&#x200B;**主菜单** ![行主菜单](assets/lines-menu.png)（如果可用），然后单击&#x200B;**请求** > **已提交** > **Planning**，然后单击状态为&#x200B;**待审核**&#x200B;或&#x200B;**审核中**&#x200B;的请求。

     >[!TIP]
     >
     >如果您无权访问Workfront Planning，或无权查看任何工作区，则只能使用电子邮件或应用程序内通知访问批准请求。

   * 单击屏幕右上角的Unified Shell中的&#x200B;**通知**&#x200B;区域图标![通知区域图标](assets/notifications-area-icon-unified-shell.png)，然后单击有关待您审批的请求的通知以打开请求。
   * 转到电子邮件中的电子邮件通知，通知您某个请求等待您审批，然后单击&#x200B;**打开请求**&#x200B;以打开该请求。<!--add the name of the button here, from the email-->

   请求页面将以只读模式打开。

   ![处于审核状态的只读请求页面](assets/read-only-reqeust-page-in-review-status.png)

1. （可选）单击请求右上角的&#x200B;**批准**&#x200B;图标![批准图标](assets/approvals-icon.png)以查看批准者。
1. 单击&#x200B;**审核并批准**，然后选择以下选项之一：

   * **批准**：这将批准请求。 在所有批准者批准请求后，将立即为与请求表单关联的记录类型创建记录。
   * **拒绝**：这将拒绝请求，即使您是唯一拒绝该请求的审批者。 没有为与请求表单关联的记录类型创建记录。

   当提交请求的请求被批准或拒绝时，提交请求的用户会收到电子邮件和应用内通知。

   请求的状态将更改为以下内容，具体取决于批准决定：

   * **已完成**：请求已被批准。
   * **已拒绝**：请求被拒绝。

   该请求将保留在Workfront请求区域的已提交部分的“计划”选项卡中。
