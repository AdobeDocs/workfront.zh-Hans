---
title: 可对每种对象类型的功能进行可配置的旧版访问
description: 本文介绍作为Adobe Workfront管理员，您可以在每个旧版访问级别中，为每个对象类型提供哪些权限。 它还说明每种类型的旧版访问级别的默认配置。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '3456'
ht-degree: 10%

---

# 可对每种对象类型的功能进行可配置的旧版访问

本文介绍作为Adobe Workfront管理员，您可以在每个旧版访问级别中，为每个对象类型提供哪些权限。 它还说明每种类型的旧版访问级别的默认配置。

有关每个访问级别中对象类型可用的所有功能的信息，请参阅 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 项目

在每个旧版访问级别中，您可以为项目配置以下选项：

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
   <td>计划员（计划许可证类型）</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享项目的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对项目进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享项目的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对项目进行有限的编辑访问。 要了解与计划员访问级别（允许对项目进行完全编辑访问）相比，在工作人员访问级别中编辑访问权限受限的情况，请参阅部分 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">项目</a> 在文章中 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">可用于每种对象类型的功能</a>.</p> <p>要优化此设置，您可以配置共享项目的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> （默认选择） <p>查看访问权限受到限制，因为您无法对其进行微调以启用或禁用项目共享。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问项目。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 任务

在每个旧版访问级别中，您可以为任务配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要微调此功能，您可以配置共享任务的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对任务进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要微调此功能，您可以配置共享任务的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对任务进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> （默认选择）<p>查看访问权限受到限制，因为您无法对其进行微调以启用或禁用项目共享。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问任务。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

在每个旧版访问级别中，您可以针对问题配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享问题的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对问题进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对问题进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对问题进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享问题的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对问题进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问问题。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 项目组合

在每个旧版访问级别中，您可以为组合配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享项目组合的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对项目组合进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> <p>无法访问项目组合。</p> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问项目组合。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 项目群

在每个旧版访问级别中，您可以为程序配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享程序的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对程序进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> <p>无法访问程序。</p> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问程序。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 报表、功能板和日历

在每个旧版访问级别中，您可以为报表、功能板和日历配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b></p><p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮)，然后禁用或启用以下任何操作。 默认情况下，这两个选项都处于启用状态：</p> 
      <ul> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对报表、功能板和日历进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态，但 <b>查看内置报表</b>, <b>公开共享报表</b>和 <b>在系统范围内共享</b>.</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>查看嵌入报表</p> </li> 
       <li> <p>共享</p> </li> 
       <li> <p>公开（外部）共享报表</p> </li> 
       <li> <p>在系统范围内共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> （默认选择）<p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任何操作。 默认情况下，这两个选项都处于启用状态：</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b> （默认选择）<p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任何操作。 默认情况下，只启用“共享”选项。</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b> （默认选择）：允许仅查看与其共享的报表、功能板和日历。</p> <p>要优化此设置，您可以配置查看内置报表的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用 <b>查看内置</b>（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问报表、功能板和日历。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 过滤器、视图和分组

在每个旧版访问级别中，您可以为过滤器、视图和分组配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享过滤器、视图和分组的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对过滤器、视图和分组进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置共享过滤器、视图和分组的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对过滤器、视图和分组进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享过滤器、视图和分组的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对过滤器、视图和分组进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <p><b>查看</b>:</p> <p>要优化此设置，您可以配置共享过滤器、视图和分组的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对过滤器、视图和分组进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
   <td> <p>无法访问过滤器、视图和分组。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 文档

在每个旧版访问级别中，您可以为文档配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要微调此功能，您可以配置共享文档的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对文档进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态，但 <b>公开共享文档</b> 和 <b>在系统范围内共享</b>.</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b></p><p>要微调此功能，您可以配置共享文档的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对文档进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态，但 <b>公开共享文档</b> 和 <b>在系统范围内共享</b>.</p> 
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
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要微调此功能，您可以配置共享文档的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对文档进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任何操作。 默认情况下，除最后两个选项外，所有这些选项都处于启用状态。 <b>公开共享文档</b> 和 <b>在系统范围内共享</b>.</p> 
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
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b></p><p>要微调此功能，您可以配置共享文档的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对文档进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li> <p>共享</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>在此访问级别中无法配置对文档的访问。 但外部用户可以使用Workfront来查看、审阅和下载文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 用户

在每个旧版访问级别中，您可以为用户配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b></p><p>要优化此设置，您可以配置查看用户联系信息的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用 <b>查看联系信息</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许用户进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任何操作。 只有前两个选项， <b>创建</b> 和 <b>删除</b>，则默认情况下处于启用状态。</p> 
      <ul> 
       <li> <p>创建</p> </li> 
       <li> <p>删除</p> </li> 
       <li>用户管理员 (所有用户)</li> 
       <li> <p>用户管理员（组用户）</p> </li> 
      </ul> <p>有关两个“用户管理员”选项的信息，请参阅部分 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">配置用户的访问权限以使用自定义访问级别编辑用户</a> 在文章中 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li><p> <b>查看</b> （仅可用选项）</p><p>要优化此设置，您可以配置查看用户联系信息的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用 <b>查看联系信息</b> 选项（默认启用）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li><p> <b>查看</b> （仅可用选项）</p> <p>要优化此设置，您可以配置查看用户联系信息的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后启用或禁用 <b>查看联系信息</b> 选项（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>查看</b> （仅可用选项）</p><p>要优化此设置，您可以配置查看用户联系信息的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后启用或禁用 <b>查看联系信息</b> 选项（默认情况下处于禁用状态）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问用户。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 团队

在每个旧版访问级别中，您可以为团队配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li><b>查看</b> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，这两个选项均处于禁用状态。</p> 
      <ul> 
       <li>查看所有团队</li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对团队进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，所有这些组件都处于启用状态，但 <b>编辑我所在的团队</b>.</p> 
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
     <li> <b>查看</b>
      <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li>查看所有团队</li> 
       <li> <p>查看与我的组关联的团队</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对团队进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 只有第一个选项， <b>编辑我所在的团队</b>，默认情况下处于禁用状态。</p> 
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
     <li> <p><b>查看</b> （仅可用选项）</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，这两个选项都处于启用状态。</p> 
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
     <li> <p><b>查看</b> （仅可用选项）</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li> <p>查看所有团队</p> </li> 
       <li>查看与我的组关联的团队</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问团队。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>


## 模板

在每个旧版访问级别中，您可以为模板配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li><p> <b>查看</b></p> <p>要优化此设置，您可以配置共享模板的功能。 单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> ，然后禁用或启用 <b>共享</b> 选项（默认启用）。</p> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对模板进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 默认情况下，所有这些组件都处于启用状态。</p> 
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
     <li> <p><b>无权访问</b> （仅可用选项）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <p><b>无权访问</b> （仅可用选项）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>无权访问</b> （仅可用选项）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问模板。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 财务数据

在每个旧版访问级别中，您可以为财务数据配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <p><b>查看</b>:</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 默认情况下，这两个选项都处于启用状态。</p> 
      <ul> 
       <li>查看角色记帐 &amp; 成本率</li> 
       <li> <p>查看用户记帐 &amp; 成本率</p> </li> 
      </ul> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对财务数据进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>查看</b> 按钮，然后禁用或启用以下任一选项*。 只有最后两种选择， <b>查看角色开单和成本费率</b> 和 <b>查看用户账单和成本费率</b>，则默认情况下处于启用状态。</p> 
      <ul> 
       <li>编辑角色记帐 &amp; 成本率</li> 
       <li> <p>编辑用户记帐 &amp; 成本率</p> </li> 
       <li>查看角色记帐 &amp; 成本率</li> 
       <li> <p>查看用户记帐 &amp; 成本率</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li> <p><b>无权访问</b> （默认选择）</p> </li> 
     <li> <b>查看</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <p><b>无权访问</b> （默认选择）</p> </li> 
     <li><b>查看</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <p><b>无权访问</b> （仅可用选项）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>无法访问财务数据。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 有关这些选项的信息，请参阅 [账单和收入概述](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 资源管理

在每个旧版访问级别中，您可以为资源管理配置以下选项：

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
   <td>计划人 </td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> </li> 
     <li> <p><b>编辑</b> （默认选择）：允许对资源管理进行完全编辑访问。</p> <p>要微调此参数，请单击齿轮图标 <img src="assets/gear-icon-in-access-levels.png"> 在 <b>编辑</b> 按钮，然后禁用或启用以下任一选项。 只有第一个选项， <b>在计划员中编辑优先级和预算小时数</b>，则默认情况下处于启用状态。</p> 
      <ul> 
       <li> <p> 在“规划者”中编辑优先级和预算小时数</p> </li> 
       <li> <p>管理资源池</p> <p><b>注意</b>:为了管理资源池，用户需要额外访问财务数据并拥有项目财务的权限。 如果您向无权访问财务数据的计划员用户授予资源管理访问权限，则用户仍可以在资源计划器中查看每小时分配，但无法切换到“成本”视图或查看“业务案例”。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予对财务数据的访问权限</a> 和 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共享对象的财务权限</a>.</p> </li> 
       <li> <p>在工作负载均衡器中更新已计划的小时数</p> <p><b>注意</b>:为了更新工作负载平衡器中的计划小时数，用户需要向对象贡献权限，并在“高级设置”下启用“进行分配”。 有关信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象共享权限概述</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>员工 </td> 
   <td> 
    <ul> 
     <li><b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查看者</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> </li> 
     <li> <b>查看</b> （默认选择）</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>请求人</td> 
   <td> 
    <ul> 
     <li> <b>无权访问</b> （仅可用选项） </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>外部用户</td> 
   <td> <p>访问不可用。 外部用户只能使用Workfront来审阅和下载文档，以及查看与他们共享的日历。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 方案计划员区域

所有旧版访问级别的默认设置为“无权访问”。 Workfront管理员可以将其更改为“查看”或“编辑”访问级别，以供任何“计划员”、“工作人员”和“审阅人”访问级别使用。

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>用户只能查看其他用户创建的计划，前提是与他们共享指向该计划的链接。

## Workfront目标区域

所有六个默认旧版访问级别（以及所有4个许可证类型）都可以编辑和查看Workfront目标。

默认选项为“编辑”。
