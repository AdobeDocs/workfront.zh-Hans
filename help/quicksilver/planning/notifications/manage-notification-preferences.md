---
title: 管理Adobe Workfront Planning通知首选项
description: 您或许可以管理Adobe Workfront Planning的通知首选项。 本文介绍了如何配置通知首选项。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

---


# 管理Adobe Workfront Planning通知首选项

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Workfront Planning中发生以下操作时，您可能会收到应用程序内通知或电子邮件通知：

* 有人将您或您的团队添加到记录页面上的评论中
* 有人请求访问视图或工作区<!--or <span class="preview">or a record</span>-->的权限
* 有人授予您访问视图或工作区<!--or <span class="preview">or a record</span>-->的权限 <!--I could not test this but Isk confirmed-->
* 提交Workfront Planning请求。
* 某人批准或拒绝了您提交的Workfront Planning请求。
* 状态将更改为您提交的Workfront Planning请求。

## 访问权限要求


+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>浅色或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>查看工作区或更高权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p><p>Standard, Light, or Contributor
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table> -->

有关Workfront Planning通知的更多信息，另请参阅以下文章：

* 有关记录的注释信息，请参阅[管理记录注释](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有关Workfront Planning的应用程序内通知的信息，请参阅[管理Adobe Workfront Planning的应用程序内通知](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)。
* 有关Workfront Planning电子邮件通知的信息，请参阅[管理Adobe Workfront Planning的电子邮件通知](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)。


## 管理通知偏好设置

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

   有关管理通知的详细信息，请参阅[帐户首选项和通知](https://experienceleague.adobe.com/zh-hans/docs/core-services/interface/features/account-preferences)。

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/zh-hans/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
