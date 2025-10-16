---
title: 在Adobe Workfront Planning中批准请求
description: 当用户将请求提交到与Adobe Workfront Planning中的批准关联的请求表单时，批准者会收到有关未决批准的通知，并收到电子邮件。 他们必须先批准请求，Workfront Planning才能创建对象。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 1%

---

# 在Adobe Workfront Planning中批准请求

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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

* 对于通过提交请求表单而创建的记录，您可以在“批准者”和“批准日期”字段中显示批准信息。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<ul><li><p>任何Workfront包</p></li>
与
<li><p>任何规划包</p></li></ul>
或
<ul><li><p>任何工作流包</p></li>
与
<li><p>任何规划包</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区的权限并记录类型</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
