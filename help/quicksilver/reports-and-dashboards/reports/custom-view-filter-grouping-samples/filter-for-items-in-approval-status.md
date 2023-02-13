---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：仅显示处于批准状态的项目
description: 您只能显示当前处于“待批准”状态的特定项目。 对于具有批准状态的任何其他对象，其工作方式均相同。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# 过滤器：仅显示处于批准状态的项目

您只能显示当前处于“待批准”状态的特定项目。 对于具有批准状态的任何其他对象，其工作方式均相同。

您可以将以下对象置于批准状态：

* 任务
* 问题
* 项目

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

## 仅显示处于审批状态的项目

1. 例如，转到要自定义的项目列表的过滤器。
1. 单击 **添加过滤器规则** 对于 **状态** 列表对象的字段。\
   例如，在项目报表中，添加 **状态等于计划**，但是您希望仅显示状态为 **计划 — 待批准**.

1. 单击 **切换到文本模式**.
1. 修改

   ```
   status
   ```

   添加行 **:A** 至状态的3个字母键：
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 单击 **完成**，则 **保存过滤器**.

   该列表仅显示处于“计划 — 待批准”状态的项目。
