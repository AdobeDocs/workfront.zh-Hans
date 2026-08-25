---
title: 共享Workfront规划字段
description: 您可以与其他人共享Workfront Planning记录的字段，以确保在使用Adobe Workfront Planning时进行协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 2%

---


# 共享Workfront规划字段

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

您可以与其他人共享Workfront Planning记录的字段，以确保在使用Adobe Workfront Planning时进行协作。

字段共享让工作区管理员能够控制对单个字段的访问。 记录类型中的每个字段都有自己的共享对话框，其中访问权限可以设置为无权访问、查看字段值或管理字段值。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>带规划包的任何Workfront或工作流</p> 
或
<p>任何Workfront Planning作为独立产品包</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>“任一”</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>“任一”</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>管理字段的权限以更改字段值</p>  
   <p>向记录类型分配或更高权限以继承字段的管理权限</p>  
   </td> 
  </tr>
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关共享字段的注意事项

* 您可以与用户、工作角色、组、团队或公司共享字段。
* 对字段的访问权限来自组合以下设置：

  * **继承的权限**：默认情况下，字段继承某人对该记录类型的相同访问权限（查看记录类型权限授予用户查看字段值的权限；Contribute或Manage记录类型权限授予用户管理字段值的权限）。 您可以关闭继承权限，并授予用户比记录类型更低的字段访问权限。
  * 工作区中的&#x200B;**每个人都可以查看**&#x200B;或&#x200B;**只有受邀人员才能访问**&#x200B;选择。 您可以允许拥有工作区权限的每个人查看该字段，也可以仅向单个实体授予权限。

  如果同一人适用多个规则，则他们会从其中一个规则中获取可用的最高权限。

* 只有工作区所有者和管理员可以调整字段权限；工作区管理员始终保留对所有字段的管理访问权限，并且这一点无法降低。
* 字段共享控制对值的访问，而不是字段设置。 只有工作区管理员才能更改字段的配置。
* 将某人添加到字段的共享列表不会授予他们工作区或记录类型访问权限。 如果他们缺少该访问权限，则会显示一个警告图标，指示权限仅在他们被添加到记录类型后才会生效。
* 系统字段（例如，创建者、记录ID）和主字段不能具有受限共享。
* 受限制的字段会在字段显示位置强制执行。 这包括所有视图、记录详细信息页面、请求表单、连接和查找字段、画布功能板、API和MCP工具。
* 查找字段继承其源字段的权限。
* 任何能够访问公共视图的人都可以完全查看和只读公共视图。
* 复制记录时，受限制的值将不会复制到新记录中。
* 受限制的字段值更改不会记录在记录的历史记录中。
* 字段的权限更改不会触发通知。
* 对于全局记录类型，字段权限适用于所有辅助工作区，并且无法本地调整。


从克劳德：
字段的其他权限 — 可以将其添加到所有共享的概述文章?? - help/quicksilver/planning/access/sharing-permissions-overview.md

下面是记录类型/工作区访问如何在文档中映射到字段级访问：

字段权限级别（只有两个，加上无）：

无权访问 — 字段完全隐藏
查看字段值 — 可以查看值，无法编辑
管理字段值 — 可以查看和编辑

从记录类型角色的默认继承

记录类型/工作区访问权限默认字段权限
查看查看字段值
Contribute管理字段值
管理（工作区管理器）管理字段值（已锁定 — 无法减少）

因此，默认情况下，字段只是镜像某个人在记录类型上所具有的任何角色 — 查看者获得只读权限，参与者和管理者获得编辑权限。 Workspace管理员属于特殊情况：无论何时将其添加到字段共享列表，都会预先选择“管理字段值”并禁用“查看字段值”选项，因为他们的编辑权限永远都不会被剥夺。

通配符（回退）设置
除了继承之外，每个字段都有一个通配符默认值：

工作区中的每个人都可以查看（默认）
仅受邀人员可访问

最终权限的计算方式

如果启用了继承权限：人员的访问权限=中的最高权限（继承自记录类型、通配符、单独授予的权限）。
如果禁用继承的权限：人员的访问权限= （通配符，单独授予的权限）中的最高值 — 记录类型角色不再考虑在内。
如果禁用继承，则通配符为“只有受邀人员才能访问”，并且受邀人员在“无权访问”→不会单独进行添加。

其他权限注释

单独授予某人访问权限不会授予他们工作区/记录类型的访问权限 — 它只会处于非活动状态（带有警告图标），直到他们单独添加到工作区。
对于全局记录类型，字段权限设置一次，并应用于所有辅助工作区；辅助/团队工作区管理员无法在本地覆盖它们。

## 共享字段

