---
title: 管理Adobe Workfront Planning电子邮件通知
description: 当有人在Adobe Workfront Planning的记录评论中为您标记时，您将收到该标记的电子邮件通知。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 1%

---


# 管理Adobe Workfront Planning电子邮件通知

{{planning-important-intro}}

当存在以下情况时，您可以从Workfront Planning接收电子邮件通知：

* 有人在记录评论中标记您

  有关在记录评论中标记其他人的信息，请参阅[管理记录评论](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人要求您授予访问视图或工作区的权限
* 有人确认已授予您查看或工作区的访问权限<!--Isk confirmed that there is nno email for denying access but did not test-->


## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包含的内容的更多信息，请参阅<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定价和打包</a>。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>您组织的Workfront实例必须载入到AdobeUnified Experience。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准、浅色或贡献者</p>
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
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->


## 当有人在评论中标记您时管理电子邮件通知

1. （视情况而定）当有人在记录上的评论中标记您后，转到通知您标记和评论的电子邮件通知。 电子邮件的发件人为Adobe Experience Cloud。

   ![](assets/email-notification-example.png)

1. 单击&#x200B;**Workfront**&#x200B;框中的消息。

   记录详细信息页面将在Workfront中打开。 您可以更新记录或回复评论。

1. （视情况而定）如果可用，请单击&#x200B;**查看所有通知**。 <!--check with Lilit - do non-IMS users have this button??-->
将在Adobe Experience Cloud中打开**通知**&#x200B;页面。 将显示来自所有Adobe Experience Cloud应用程序的所有通知。

## 在请求和授予权限时管理电子邮件通知

当有人请求或授予您查看或工作区的权限时，您将收到电子邮件通知。

有关请求、授予或拒绝视图或工作区的权限的信息，请参阅[请求视图或工作区的权限](/help/quicksilver/planning/access/request-permissions.md)。

有关管理Workfront Planning通知的信息，请参阅[管理Adobe Workfront Planning通知首选项](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。
