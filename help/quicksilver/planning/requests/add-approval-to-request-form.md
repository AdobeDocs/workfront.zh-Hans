---
title: 向请求表单添加批准
description: 您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---


<!--

---
title: Add an Approval to a Request Form
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->

# 向请求表单添加批准

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。

本文介绍了工作区经理如何向与记录类型关联的请求表单添加批准。

有关在Workfront Planning中创建申请表单的信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

有关向记录类型提交请求以创建记录的信息，请参阅[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

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

## 有关将审批添加到请求表单的注意事项

* 您可以向请求表单添加一个或多个批准者。 您只能添加用户作为批准者。
* 向请求表单添加多个批准者时，所有批准者都必须接受请求，然后才能在Workfront Planning中创建记录。
* 向请求表单添加审批是可选的。 如果申请表单与批准无关，Workfront Planning会在提交申请后立即创建记录。

## 向请求表单添加批准

1. 开始为记录类型创建请求表单，如[在Adobe Workfront Planning中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 单击&#x200B;**配置**。

   显示&#x200B;**配置**&#x200B;区域。

   ![](assets/configuration-tab.png)
1. 在&#x200B;**审批者**&#x200B;字段中，单击下拉图标，然后在列表中选择一个或多个名称

   或

   开始键入审批者的姓名，然后当该姓名显示在列表中时将其选定。

   >[!TIP]
   >
   >    如果添加多个审批者，则在Workfront Planning创建记录之前，所有审批者都必须审批该请求。

1. （可选）如果您以前从未共享过该申请表单，请单击&#x200B;**Publish**

   或

   单击&#x200B;**共享**&#x200B;以共享表单，然后单击&#x200B;**复制链接**。
1. （可选）用户使用您共享的链接并提交请求后，Workfront Planning会向审批者发送审批通知和电子邮件。

   有关批准请求的信息，请参阅[批准请求](/help/quicksilver/planning/requests/approve-request.md)。
