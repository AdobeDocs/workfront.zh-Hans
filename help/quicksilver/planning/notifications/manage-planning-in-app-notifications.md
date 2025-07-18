---
title: 管理Adobe Workfront Planning应用程序内通知
description: 当有人在记录评论中标记您或您的团队时，您会收到该标记的电子邮件通知。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 1%

---


# 管理Adobe Workfront Planning应用程序内通知

{{planning-important-intro}}

当存在以下情况时，您可以从Workfront Planning接收应用程序内通知：

* 有人在记录评论中标记您或您的团队

  有关在记录评论中标记其他人的信息，请参阅[管理记录评论](/help/quicksilver/planning/records/manage-record-comments.md)。
* 有人要求您授予访问视图或工作区的权限
* 有人确认已授予您查看或工作区的访问权限<!--Isk confirmed there is no notification for denying permissions - did not test-->

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
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--
OLD:

+++ Expand to view access requirements. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## 当有人在评论中标记您时管理应用程序内通知

1. （视情况而定）当有人在记录中的评论中为您或您的团队标记后，请转到Adobe Experience Cloud中的应用程序内&#x200B;**通知**&#x200B;图标![Experience Cloud通知图标](assets/experience-cloud-notifications-icon.png)。

   ![应用内通知示例](assets/in-app-notification-example.png)

1. 单击通知。

   此时将在Workfront Planning中打开记录详细信息页面。 您可以更新记录或回复评论。

1. （可选）单击&#x200B;**全部标记为已读**&#x200B;以指示您已读取所有通知。
1. （可选）单击&#x200B;**查看全部**&#x200B;以转到Adobe Experience Cloud中的&#x200B;**通知**&#x200B;页面。

## 在请求和授予权限时管理应用程序内通知

当有人请求或授予您查看或工作区的权限时，您会收到应用程序内通知。

有关请求、授予或拒绝视图或工作区的权限的信息，请参阅[请求视图或工作区的权限](/help/quicksilver/planning/access/request-permissions.md)。

有关管理Workfront Planning通知的信息，请参阅[管理Adobe Workfront Planning通知首选项](/help/quicksilver/planning/notifications/manage-notification-preferences.md)。
