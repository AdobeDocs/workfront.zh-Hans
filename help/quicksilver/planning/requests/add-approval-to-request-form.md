---
title: 在Adobe Workfront Planning中为申请表单添加批准
description: 您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 83b3bd73fd30b5fba931e64783dee67485d98fe9
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# 在Adobe Workfront Planning中为申请表单添加批准

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning请求表单中添加批准流程，以在创建记录之前为每个提交的请求启动批准。

本文介绍了工作区经理如何向与记录类型关联的请求表单添加批准。

有关在Workfront Planning中创建申请表单的信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

有关向记录类型提交请求以创建记录的信息，请参阅[提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

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
   <li><p>管理对工作区和记录类型的权限</p></li>
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

## 有关将审批添加到请求表单的注意事项

* 您可以向请求表单添加一个或多个批准者。 您只能添加用户作为批准者。
* <span class="preview">您可以通过在“批准者”和“批准日期”字段中提交请求表单，来显示所创建记录的批准信息。 有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。</span>
* 向请求表单添加多个批准者时，所有批准者都必须接受请求，然后才能在Workfront Planning中创建记录。
* 如果所有批准者都批准了该请求，则将为与请求表单关联的记录类型创建记录。
* 如果至少有一个批准者拒绝了请求，并且所有其他批准者都批准了该请求，则会在Workfront中为请求区域创建一个请求，但不会为与请求表单关联的记录类型创建记录。
* 向请求表单添加审批是可选的。 如果申请表单与批准无关，Workfront Planning会在提交申请后立即创建记录。

## 向请求表单添加批准

1. 开始为记录类型创建请求表单，如[在Adobe Workfront Planning中创建和管理请求表单](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 单击&#x200B;**配置**。

   显示&#x200B;**配置**&#x200B;区域。

   ![配置选项卡](assets/configuration-tab.png)
1. 在&#x200B;**审批者**&#x200B;字段中，单击下拉图标，然后在列表中选择一个或多个用户<span class="preview">或团队</span>

   或

   开始键入要设置为审批者的用户<span class="preview">或团队</span>的名称，然后当该名称显示在列表中时将其选定。

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* 您可以将一个或多个批准者添加到请求表单。
   >
   >* 如果添加多个审批者，则在Workfront Planning创建记录之前，所有审批者都必须审批该请求。
   >
   >* 如果至少有一位审批者拒绝了请求，则该请求会被拒绝，并且不会创建记录。 该请求将保留在Workfront请求区域的已提交部分的“计划”选项卡中。
   >
   >* 在批准或拒绝请求之前，所有批准者都必须做出决定。
   >
   >* <span class="preview">如果将团队设置为批准者，则只需该团队做出一个决定。</span>


1. （可选）如果您以前从未共享过该请求表单，请单击&#x200B;**发布**

   或

   单击&#x200B;**共享**&#x200B;以共享表单，然后单击&#x200B;**复制链接**。
1. （可选）用户使用您共享的链接并提交请求后，Workfront Planning会向审批者发送审批应用程序内通知和电子邮件。

   >[!NOTE]
   >
   >   贵组织的Workfront实例必须载入到Adobe Unified Experience，用户才能接收电子邮件和应用程序内通知。


   有关批准请求的信息，请参阅[批准请求](/help/quicksilver/planning/requests/approve-request.md)。
