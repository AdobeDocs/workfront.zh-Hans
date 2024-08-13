---
title: 可配置访问每种对象类型的功能
description: 本文介绍了作为Adobe Workfront管理员，您可以对每个对象类型在每个访问级别允许什么。 它还说明了每种访问级别的默认配置。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '3436'
ht-degree: 10%

---

# 可配置访问每种对象类型的功能

本文介绍了作为Adobe Workfront管理员，您可以对每个对象类型在每个访问级别允许什么。 它还说明了每种访问级别的默认配置。

有关每个访问级别中某个对象类型可用的所有功能的信息，请参阅[每个对象类型可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)。

## 项目

在每个访问级别中，您可以为项目配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner（计划许可证类型）</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享项目的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对项目进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>复制</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>查看</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享项目的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许有限的项目编辑权限。 要了解与“规划者”访问级别（允许对项目的完全编辑访问权限）相比，“辅助进程”访问级别中的“编辑”访问权限如何受限，请参阅可用于每个对象类型</a>的<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">功能一文中的<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">项目</a>部分。</p> <p>要优化此设置，您可以配置共享项目的功能。 单击“编辑”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> （默认选择） <p>查看权限受限，因为无法对其进行微调以启用或禁用项目共享。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>项目访问权限不可用。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 任务

在每个访问级别中，您可以为任务配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要微调此功能，您可以配置共享任务的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对任务进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要微调此功能，您可以配置共享任务的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对任务进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> （默认选择）<p>查看权限受限，因为无法对其进行微调以启用或禁用项目共享。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问任务。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

在每个访问级别中，您可以为问题配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享问题的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对问题进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对问题进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对问题进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对问题进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问问题。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 项目组合

在每个访问级别中，您可以为项目组合配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享项目组合的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对项目组合进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> <p>组合访问权限不可用。</p> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>组合访问权限不可用。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 项目群

在每个访问级别中，可以为程序配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要微调这一点，您可以配置共享程序的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对程序进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> <p>无法访问程序。</p> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问程序。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 报告、功能板和日历

在每个访问级别中，您可以为报告、功能板和日历配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b></p><p>要优化此操作，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何操作。 默认情况下，这两个选项都处于启用状态：</p> 
      <ul> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对报告、功能板和日历进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 除<b>查看内置报告</b>、<b>公开共享报告</b>和<b>共享系统范围</b>外，默认启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>公开共享报表（外部）</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> （默认选择）<p>要优化此操作，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何操作。 默认情况下，这两个选项都处于启用状态：</p> 
      <ul> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b> （默认选择）<p>要优化此操作，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何操作。 默认情况下，仅启用“共享”选项。</p> 
      <ul> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b>（默认选择）：允许对与其共享的报告、功能板和日历进行仅查看访问。</p> <p>要微调此功能，您可以配置查看内置报表的功能。 单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>查看内置</b>（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问报告、功能板和日历。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 过滤器、视图和分组

在每个访问级别中，您可以为筛选器、视图和分组配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享筛选器、视图和分组的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对筛选器、视图和分组的完全编辑访问权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享筛选器、视图和分组的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对筛选器、视图和分组的完全编辑访问权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享筛选器、视图和分组的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对筛选器、视图和分组的完全编辑访问权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>视图</b>：</p> <p>要优化此设置，您可以配置共享筛选器、视图和分组的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对筛选器、视图和分组的完全编辑访问权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问筛选器、视图和分组。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 文档

在每个访问级别中，您可以为文档配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要微调此功能，您可以配置共享文档的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对文档的完全编辑权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 除<b>公开共享文档</b>和<b>在系统范围内共享文档</b>外，默认启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>公开（外部）共享文档</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b></p><p>要微调此功能，您可以配置共享文档的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对文档的完全编辑权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 除<b>公开共享文档</b>和<b>在系统范围内共享文档</b>外，默认启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>公开（外部）共享文档</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要微调此功能，您可以配置共享文档的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对文档的完全编辑权限。</p> <p>要优化此操作，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何操作。 默认情况下启用所有这些功能，但最后两个<b>共享公开文档</b>和<b>共享系统范围</b>除外。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>公开（外部）共享文档</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>查看</b></p><p>要微调此功能，您可以配置共享文档的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对文档的完全编辑权限。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>在此访问级别中无法配置对文档的访问。 但外部用户可以使用Workfront查看、查看和下载文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 用户

在每个访问级别中，您可以为用户配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b></p><p>要优化此功能，您可以配置查看用户联系信息的功能。 单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>查看联系人信息</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许用户拥有完整的编辑权限。</p> <p>要优化此操作，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何操作。 默认情况下仅启用前两个选项<b>创建</b>和<b>删除</b>。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li>用户管理员 (所有用户)</li> 
       <li> <p>用户管理员（组用户）</p> </li> 
      </ul> <p>有关两个“用户管理”选项的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">向用户授予访问权限</a>一文中的<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">配置用户的访问权限，以使用自定义访问级别</a>编辑用户部分。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li><p> <b>查看</b> （仅选项可用）</p><p>要优化此功能，您可以配置查看用户联系信息的功能。 单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>查看联系人信息</b>选项（默认启用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li><p> <b>查看</b> （仅选项可用）</p> <p>要优化此功能，您可以配置查看用户联系信息的功能。 单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后启用或禁用<b>查看联系人信息</b>选项（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b> （仅选项可用）</p><p>要优化此功能，您可以配置查看用户联系信息的功能。 单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后启用或禁用<b>查看联系人信息</b>选项（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问用户。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 团队

在每个访问级别中，可为团队配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li><b>视图</b> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下禁用这两个选项。</p> 
      <ul> 
       <li>查看所有团队</li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对团队进行完全编辑访问。</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认启用所有这些组，但<b>编辑我所在的团队</b>除外。</p> 
      <ul> 
       <li>创建</li> 
       <li>删除</li> 
       <li> <p>编辑我所在的团队</p> </li> 
       <li> <p>编辑我管理的组中的团队（仅组管理员）</p> </li> 
       <li> <p>查看所有团队</p> </li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>视图</b>
      <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li>查看所有团队</li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对团队进行完全编辑访问。</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下仅禁用第一个选项<b>编辑我所在的团队</b>。</p> 
      <ul> 
       <li> <p>编辑我所在的团队</p> </li> 
       <li> <p>查看所有团队</p> </li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b> （仅选项可用）</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li> <p>查看所有团队</p> </li> 
       <li>查看与我的组关联的团队</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b> （仅选项可用）</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li> <p>查看所有团队</p> </li> 
       <li>查看与我的组关联的团队</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问团队。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>


## 模板

在每个访问级别中，您可以为模板配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li><p> <b>视图</b></p> <p>要优化此设置，您可以配置共享模板的功能。 单击“查看”按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用<b>共享</b>选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对模板进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下，将启用所有这些功能。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （仅选项可用）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （仅选项可用）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （仅选项可用）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问模板。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 财务数据

在每个访问级别中，您可以为财务数据配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <p><b>视图</b>：</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li>查看角色计费 &amp; 成本费率</li> 
       <li> <p>查看用户计费 &amp; 成本费率</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b>（默认选择）：允许对财务数据进行完全编辑访问。</p> <p>要微调此设置，请单击<b>查看</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项*。 默认情况下只启用最后两个选项，<b>查看角色帐单和成本费率</b>和<b>查看用户帐单和成本费率</b>。</p> 
      <ul> 
       <li>编辑角色计费 &amp; 成本费率</li> 
       <li> <p>编辑用户计费 &amp; 成本费率</p> </li> 
       <li>查看角色计费 &amp; 成本费率</li> 
       <li> <p>查看用户计费 &amp; 成本费率</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （默认选择）</p> </li> 
     <li> <b>视图</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （默认选择）</p> </li> 
     <li><b>视图</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>无访问权限</b> （仅选项可用）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问财务数据。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;有关这些选项的信息，请参阅[帐单和收入概览](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

## 资源管理

在每个访问级别中，您可以为资源管理配置以下选项：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>访问级别</th> 
   <th>选项</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>规划器 </td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>视图</b> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对资源管理进行完全编辑访问。</p> <p>要优化此设置，请单击<b>编辑</b>按钮上的齿轮图标<img src="assets/gear-icon-in-access-levels.png">，然后禁用或启用以下任何选项。 默认情况下仅启用第一个选项<b>在规划者</b>中编辑优先级和预算小时数。</p> 
      <ul> 
       <li> <p> 在“规划者”中编辑优先级和预算小时数</p> </li> 
       <li> <p>管理资源池</p> <p><b>注意</b>：为了管理资源池，用户需要更多财务数据的访问权限和项目财务的权限。 如果您向无权访问财务数据的规划者用户授予资源管理访问权限，则该用户仍可以在资源规划者中查看小时分配，但无法切换到成本视图或查看业务案例。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a>和<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共享对象的财务权限</a>。</p> </li> 
       <li> <p>在工作负载均衡器中更新已计划的小时数</p> <p><b>注意</b>：为了更新工作负载均衡器中的已计划小时数，用户需要权限才能贡献到对象，并在“高级设置”下启用“分配工作”。 有关信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li><b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无访问权限</b> （仅选项可用） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>访问不可用。 外部用户只能使用Workfront来查看和下载文档，以及查看与其共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 场景规划器区域

所有访问级别的默认设置为“无权访问”。 Workfront管理员可以将其更改为任何规划者、工作者和查看者访问级别的查看或编辑权限。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>仅当与另一个用户共享指向该计划的链接时，用户才能查看另一个用户创建的计划。

## Workfront目标区域

所有六个默认访问级别（以及所有4个许可证类型）都可以编辑和查看Workfront目标。

“编辑”是默认选项。
