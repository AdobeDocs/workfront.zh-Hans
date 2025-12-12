---
title: 管理Adobe Workfront Planning电子邮件通知
description: 当有人在Adobe Workfront Planning的记录评论中为您或您的团队添加标签时，您将收到该标签的电子邮件通知。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 1%

---


# 管理Adobe Workfront Planning电子邮件通知

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

当存在以下情况时，您可以从Workfront Planning接收电子邮件通知：

* 有人在记录评论中标记您或您的团队

  有关在记录评论中标记其他人的信息，请参阅[管理记录评论](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人要求您授予访问视图、工作区或记录类型<!--or <span class="preview">or a record</span>-->的权限
* 有人确认已授予您查看、工作区或记录类型<!--<span class="preview">or record</span>-->的访问权限 <!--Isk confirmed that there is nno email for denying access but did not test-->
* 提交Workfront Planning请求。 有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表](/help/quicksilver/planning/requests/create-request-form.md)
* 某人批准或拒绝了您提交的Workfront Planning请求。 有关信息，请参阅[在Adobe Workfront规划中批准请求](/help/quicksilver/planning/requests/approve-request.md)
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

<!--
OLD: 

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
   <td><p> Standard, Light, or Contributor</p>
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
</table>
-->


## 当有人在评论中标记您时管理电子邮件通知

1. （视情况而定，可选）当有人在记录上的评论中标记您或您的团队后，转到通知您标记和评论的电子邮件通知。 电子邮件的发件人为Adobe Experience Cloud。

   ![电子邮件通知示例](assets/email-notification-example.png)

1. （可选）单击电子邮件内&#x200B;**Workfront**&#x200B;框中的消息。

   记录详细信息页面将在Workfront中打开。 您可以更新记录或回复评论。

1. （视情况而定）如果可用，请单击&#x200B;**查看所有通知**。 <!--check with Lilit - do non-IMS users have this button??-->
将在Adobe Experience Cloud中打开**通知**&#x200B;页面。 将显示来自所有Adobe Experience Cloud应用程序的所有通知。

## 在请求和授予权限时管理电子邮件通知

1. （有条件，可选）在有人请求或授予您访问Planning对象类型的权限后，转到通知您权限请求的电子邮件。 电子邮件的发件人为Adobe Experience Cloud。

1. （可选）单击电子邮件内&#x200B;**Workfront**&#x200B;框中的消息。

   您请求权限的对象将在Workfront中打开。

1. （视情况而定）如果可用，请单击&#x200B;**查看所有通知**。
将在Adobe Experience Cloud中打开**通知**&#x200B;页面。 将显示来自所有Adobe Experience Cloud应用程序的所有通知。


有关请求、授予或拒绝权限的信息，请参阅[请求视图或工作区的权限](/help/quicksilver/planning/access/request-permissions.md)。

有关管理Workfront Planning通知的信息，请参阅[管理Adobe Workfront Planning通知首选项](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。

## 管理有关提交、批准或拒绝Workfront Planning请求的电子邮件通知

1. （可选）转到Workfront发送给您的电子邮件
在您提交请求之后，或者在您提交的请求已被批准或拒绝之后。 电子邮件的发件人为Adobe Workfort。

1. （可选）单击&#x200B;**打开请求**。 该操作将在Workfront Planning中打开请求。

1. 单击屏幕右上角的&#x200B;**通知**&#x200B;图标![通知区域图标Unified Shell](assets/notifications-area-icon-unified-shell.png)以访问&#x200B;**通知**&#x200B;页面。

   有关管理Workfront Planning通知的信息，请参阅[管理Adobe Workfront Planning通知首选项](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。
