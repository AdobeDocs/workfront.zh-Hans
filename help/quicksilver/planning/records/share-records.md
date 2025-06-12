---
title: 共享记录
description: 您可以与其他人共享记录以提高协作能力。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# 共享记录

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

要与其他用户协作，您可以与他人共享记录。

您可以通过以下方式共享Adobe Workfront Planning记录：

* 打开记录页面时，从浏览器复制该页面的链接。

* 在记录类型的表视图中查看记录时，复制指向记录页面的链接。

* 通过共享工作区<span class="preview">和记录类型，您可以与其他用户共享工作区中的所有记录。</span>

  有关更多信息，请参阅以下文章：

   * [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [共享记录类型](/help/quicksilver/planning/access/share-record-types.md)

  </div>

本文介绍了如何从记录类型的表视图中复制指向记录页面的链接。

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
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 参与者或更高许可证 </p>
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
   <td>  <p>查看工作区<span class="preview">和记录要共享的类型</span>的权限或更高的权限   使用链接的记录 </p>
   <p>管理工作区<span class="preview">和记录类型</span>的权限以共享工作区中的记录 </p>
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning区域的布局模板。</p>
   <div class="preview">
<p> 在“预览”环境中，必须为具有轻度或参与者许可证的用户分配包含Planning的布局模板。</p>

<p>默认情况下，标准用户和系统管理员已启用Planning。</p></div>

<p>有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">创建和管理布局模板</a>。</p></td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 从记录类型表格视图中共享记录链接

{{step1-to-planning}}

您上次访问的工作区随即打开。
1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. （视情况而定）从表右上角的&#x200B;**视图**&#x200B;下拉菜单中，选择一个表视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 右键单击记录行

   或

   将鼠标悬停在记录名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**复制链接**。

   ![记录行的上下文菜单](assets/contextual-menu-for-record-row.png)

   该链接将会复制到您的剪贴板中。

1. 将链接粘贴到电子邮件或聊天窗口中，以便与其他用户共享。 当用户收到链接时，将打开记录页面。

   >[!TIP]
   >
   >记录页面中的字段与记录的“表”视图中可用的字段相同。


   <!--add there when it will be available: if they have access to this record-->

## 通过共享工作区来共享工作区中的所有记录

与他人共享工作区时，您可以共享工作区中的所有记录。

只有对工作区具有管理权限的用户才能与他人共享该工作区。

有关详细信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)。


<div class="preview">

## 通过共享记录类型共享记录类型中的所有记录

在生产环境中，记录从工作区继承权限。

在“预览”环境中，记录从记录类型继承权限。

默认情况下，记录类型从工作区继承权限。

但是，您可以执行以下任一操作：

* 禁用从工作区继承的记录类型权限。 这将删除对记录的更高权限，但保留对工作区、记录类型和记录的查看权限。
* 手动将权限授予记录类型的用户，即使他们无权访问工作区。 这将自动授予他们查看工作区的权限。 这将授予用户对记录的权限。

只有对工作区具有管理权限的用户才能与其他人共享其记录类型和记录。

有关详细信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。

</div>
