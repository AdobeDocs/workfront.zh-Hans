---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：显示您当前的待批准项目
description: 以下项目筛选器显示处于“当前 — 待批准”状态的项目，其中登录用户是项目赞助商或Portfolio经理。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 过滤器：显示当前项目待批准

以下项目筛选器显示处于“当前 — 待批准”状态的项目，其中登录用户是项目赞助商或Portfolio经理。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 筛选当前待批项目

要应用此过滤器，请执行以下操作：

1. 转到项目列表。
1. 从 **过滤器** 下拉菜单，选择 **新建过滤器**.

1. 单击&#x200B;**切换到文本模式**.
1. 在 **为报表设置过滤器规则** ，请复制并粘贴以下代码：
   <pre>status=CUR:A<br>ponsorID=$USER.ID<br>或:a:status=CUR:A<br>或:a:portfolio:ownerID=$USER.ID</pre>

1. 单击 **保存过滤器**.
