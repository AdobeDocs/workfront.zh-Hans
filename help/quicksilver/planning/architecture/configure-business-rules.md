---
title: 配置记录类型业务规则
description: 您可以配置记录类型业务规则，以定义如何在Adobe Workfront Planning中管理该类型的记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 4%

---


# 配置记录类型业务规则

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

您可以配置记录类型业务规则，以定义如何在Adobe Workfront Planning中管理该类型的记录。

## 访问权限要求

+++ 展开以查看访问要求以执行本文中的步骤：  

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
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>工作流标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>规划标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理对工作区和记录类型的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置业务规则时的注意事项

* 您可以配置规则以确定何时可以编辑或删除记录。
* 您无法为创建记录的时间配置规则。 任何对记录类型具有管理权限的人员都可以创建记录。
* 您可以为业务规则创建一个条件，该条件引用除以下字段类型之外的所有字段类型：
  * 公式字段
  * 查找字段
  * 引用字段

## 配置业务规则

1. 转到记录类型。
1. 单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击“业务规则”。



