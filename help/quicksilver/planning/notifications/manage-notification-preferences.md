---
title: 管理Adobe Workfront Planning通知首选项
description: 您或许可以管理Adobe Workfront Planning的通知首选项。 本文介绍了如何配置通知首选项。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 60f2890e431065d0eb034a9254680e43a51ecab8
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---


# 管理Adobe Workfront Planning通知首选项

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Workfront Planning中发生以下操作时，您可能会收到应用程序内通知或电子邮件通知：

* 有人将您添加到记录页面上的评论中
* 有人请求访问视图或工作区的权限
* 有人授予您访问视图或工作区<!--I could not test this but Isk confirmed-->的权限
* 提交Workfront Planning请求。
* 某人批准或拒绝了您提交的Workfront Planning请求。
* 状态将更改为您提交的Workfront Planning请求。

## 访问要求

+++ 展开以查看访问要求。

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
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>您组织的Workfront实例必须载入到Adobe Unified Experience。</p> 
<p>仅当您的组织登记到Workfront Unified Experience时，您组织中的用户才会从Adobe Planning接收通知。 </p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p><p>标准、浅色或贡献者
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
   <td>   <p>查看工作区或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

有关Workfront Planning通知的更多信息，另请参阅以下文章：

* 有关记录的注释信息，请参阅[管理记录注释](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有关Workfront Planning的应用程序内通知的信息，请参阅[管理Adobe Workfront Planning的应用程序内通知](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)。
* 有关Workfront Planning电子邮件通知的信息，请参阅[管理Adobe Workfront Planning的电子邮件通知](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)。


## 管理通知首选项

1. 使用您的Adobe Experience Cloud凭据登录Workfront 。
1. 单击屏幕右上角的Experience Cloud **上的**&#x200B;帐户菜单![图标](assets/account-menu-icon-on-experience-cloud.png)帐户菜单图标，然后单击&#x200B;**首选项**。
1. 在&#x200B;**通知**&#x200B;部分下，单击&#x200B;**Workfront**。
1. 选择要接收的通知。
或
取消选择要停止接收的通知。

   适用于Workfront Planning的![Adobe Experience Cloud通知面板](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfront提供以下通知：

   * **提及**：当有人在Workfront Planning的评论中为您或您的团队加标签时，您会收到通知
   * **请求**：当有人执行以下操作之一时，您会收到通知：

      * 请求或授予您访问Workfront Planning对象的权限
      * 您已提交Workfront规划请求
      * 您提交更改的Workfront Planning请求的状态
      * 请求、授予或拒绝对Workfront Planning请求的批准

   有关管理通知的详细信息，请参阅[帐户首选项和通知](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences)。

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
