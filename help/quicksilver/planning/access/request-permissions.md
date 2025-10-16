---
title: 请求访问视图或Workspace的权限
description: 当某人共享指向您无权访问的视图或工作区的链接时，您可以请求权限以便能够打开该链接。 本文介绍了当您遇到无法打开的共享链接时，请求访问视图或工作区的步骤。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 请求对视图或工作区的权限

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>仅当您的组织登记到Adobe Unified Experience后，本文中描述的功能才可用。
>
>有关详细信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。


当有人与您共享指向您无权访问的视图或工作区的链接时，您可以请求对视图或工作区的权限。

向视图请求权限与向工作区请求权限类似。

本文介绍当有人与您共享链接而您无法访问共享页面时，如何请求对视图或工作区的访问权限。

有关向视图和工作区授予权限的信息，请参阅以下文章：

* [共享视图](/help/quicksilver/planning/access/share-views.md)
* [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和Planning包</p> 
或
<p>任何工作流和计划包</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>在授予您的权限请求后，您将获得以下权限：</p>
   <ul><li><p>查看或管理视图</p></li>
   <li><p>查看、贡献或管理工作区</p></li></ul>  
   <p>只有对工作区和视图具有管理权限的用户才能公开共享视图。</p></td> 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table> -->


## 请求对视图或工作区的权限

向视图请求权限与向工作区请求权限类似。

当有人与您共享指向您无权访问的工作区或视图的链接时：

1. 单击与您共享的视图或工作区的链接。

   显示&#x200B;**您没有访问权限**&#x200B;页面，通知您无权访问视图或工作区。

   ![请求查看权限](assets/request-access-to-view.png)

1. （视情况而定）如果共享的链接用于您有权访问的工作区的视图，请单击&#x200B;**用现有视图打开**。 如果您有权访问工作区，则记录类型页面将在默认视图中打开。

1. （可选且有条件）如果您无权查看工作区，请在可用框中添加个性化消息，然后单击&#x200B;**请求访问**。

   所有具有查看或工作区管理权限的用户都会收到以下访问请求通知：
   * 应用程序内通知
     ![访问请求的应用程序内通知](assets/in-app-notification-for-access-request.png)
   * 电子邮件通知
     ![访问请求的电子邮件通知](assets/email-notification-for-access-request.png)

1. （视情况而定）当视图或工作区经理授予您查看或工作区的权限时，您会收到电子邮件通知和应用程序内通知，其中包含已授予权限的确认。<!--check this - I was not able to test this, but Isk confirmed.-->
