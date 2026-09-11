---
title: 与他人共享构思空间
description: Adobe Workfront Planning现在提供了一项可在启动营销活动之前进行构思的额外功能。 利用人工智能的强大功能，在创意成为规划记录之前创建创意并与他人协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---


# 与他人共享构思空间

<!--add to TOC and miniTOC-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它只能作为&#x200B;**构思空间Beta**&#x200B;程序的一部分提供。</span>

<span class="preview">有关详细信息，请参阅[Adobe Workfront规划构思空间入门](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

Workfront Planning记录权限将传输到记录的构思空间。

此外，您还可以向其他用户授予使用构思空间的权限并向其添加构思。

请考虑以下事项：

* 构思创建者始终对其自己的构思具有编辑者权限。

* 您必须对构思空间具有编辑器权限，才能创建摘要并将其导出到其他应用程序。

## 访问权限要求

+++ 展开以查看本文中各项功能的访问要求。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<ul> 
<li><p>带规划包的任何Workfront或工作流</p></li>
或
<li><p>作为独立产品购买时的任何Planning包</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>其他产品</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe工作流许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> 
   <ul>
   <li><p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   </li>
   <li><p>必须取消选择访问级别中的禁用创意空间设置</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>为要添加记录的工作区和记录类型提供或更高权限 </p>
      <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
      <p>查看对Workfront对象的权限以将其添加到摘要 <!--not sure if this is available--></p>
      <p>创意空间上的编辑器权限以创建摘要</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing用户角色</p></td> 
   <td><p><ul><li>用于访问营销活动、产品和角色的任何GenStudio用户角色</li>
   <li>用于访问激活的GenStudio系统管理器 <!--and Events--></li></ul>
   有关信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">用户角色和权限</a>。 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

## 共享构思空间

1. 访问Planning记录的构思空间。

   有关信息，请参阅以下文章之一：

   * [从构思空间简报创建计划记录](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [在构思空间中创建简报](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. 单击右上角的&#x200B;**共享**，然后单击&#x200B;**共享文档**&#x200B;框右上角的&#x200B;**设置**&#x200B;图标![设置图标](assets/setting-icon.png)。
1. 在拥有访问权限列表中，从以下内容中选择：

   * **只有受邀人员才能访问**

     您必须将个人用户添加到构思空间并授予他们权限级别。
   * **&lt;您公司的Workfront环境>中的每个人都可以发表评论**

     贵组织中访问级别为工作流和Planning许可证的所有人均可查找并评论该构思。
   * **拥有该链接的任何人都可以评论**

     您共享该构思链接的任何人都可以在该构思上发表评论，包括组织外部的人员。

1. 单击&#x200B;**复制链接**&#x200B;可生成指向该创意的链接并与他人共享。 该链接将添加到您的剪贴板。
1. 单击“Settings（设置）”框上的“back（后退）”箭头，返回到“sharing（共享）”。
1. （视情况而定）如果您选择与特定人员共享创意空间，请开始键入其姓名或电子邮件地址，然后选择以下权限级别之一：

   | 构思空间权限 | 功能 |
   |---|---|
   | **编辑者** | 可以编辑、下载和共享创意空间 |
   | **评论者** | 可以查看和评论构思空间 |
   | **查看器** | 可以查看构思空间 |

1. （可选）在任务中包含消息，然后单击&#x200B;**邀请**。

   受邀用户会收到有关其权限分配的电子邮件通知。

1. 单击&#x200B;**X**&#x200B;图标以关闭&#x200B;**共享文档**&#x200B;框。











