---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：当状态与不同的组关联时，按相同名称状态显示项目。
description: 您可以使用3个字母的键NST将任务状态分配给A组命名的新状态。 您可能已为B组分配了另一个任务状态，该状态也命名为New Status，且带有3个字母的键NES。 尽管2个状态的名称可以相同，但3个字母的代码始终是唯一的。 有关群组状态的更多信息，请参阅创建或编辑群组状态。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 过滤器：当状态与不同组关联时，按相同名称状态显示项目

您可以为A组分配任务状态，该组名为 *新状态* 带3个字母的键 *NST*. 您可能已为B组分配另一个任务状态，该状态也名为 *新状态* 带3个字母的键 *NES。* 尽管2个状态的名称可以相同，但3个字母的代码始终是唯一的。\
有关组状态的更多信息，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

使用过滤器生成器，您无法识别具有相同名称的两种状态。 您必须使用文本模式来区分两种状态。

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

## 当状态与不同的组关联时，按相同名称状态显示项目

1. 例如，转到要自定义的任务列表的过滤器。\
   对于项目和问题，这也是一样的。
1. 单击 **添加过滤器规则** 对于 **状态** 列表对象的字段。\
   例如，在任务报表中，添加 **状态等于新状态**，则您希望仅显示状态为 **新状态**.

   >[!TIP]
   >
   >请注意，对于名为“New Status”（新状态）的状态，您只有一个选项。

1. 单击 **切换到文本模式**.\
   应显示以下代码：

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此处仅显示一个状态。 状态行显示其中一个状态的3个字母键之一。

1. 添加以下2行代码，以添加过滤器中缺少的状态：

   <pre>或:1:status=NES<br>或:1:status_Mod=in</pre>

1. 单击 **完成**，则 **保存过滤器**.

   该列表显示组A中状态为“新状态”的任务和组B中状态为“新状态”的任务。
