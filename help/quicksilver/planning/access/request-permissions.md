---
title: 请求访问视图或Workspace的权限
description: 当某人共享指向您无权访问的视图或工作区的链接时，您可以请求权限以便能够打开该链接。 本文介绍了当您遇到无法打开的共享链接时，请求访问视图或工作区的步骤。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# 请求对视图或工作区的权限

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p><b>重要</b></p>
<p>只有当您的组织登记到Adobe Unified Experience时，您组织中的用户才能请求查看和工作区的权限。 </p>
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
   <td>  <p>在授予您的权限请求后，您将获得以下权限：</p>
   <ul><li><p>查看或管理视图</p></li>
   <li><p>查看、贡献或管理工作区</p></li></ul>  
   <p>只有对工作区和视图具有管理权限的用户才能公开共享视图。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> 
   <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning区域的布局模板。</p>
   <div class="preview">
<p> 在“预览”环境中，必须为具有轻度或参与者许可证的用户分配一个布局模板，该模板包括以下区域的Planning选项：</p>
   <ul><li>主菜单</li>
   <li>项目、项目组合和程序的左侧面板</li>
   </ul>
   <p>有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">创建和管理布局模板</a>。</p>
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div>
   </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


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
