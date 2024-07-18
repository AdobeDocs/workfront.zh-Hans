---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '筛选器：当状态与不同组关联时，按同名状态显示项目'
description: 您可以将具有3个字母键NST的任务状态分配给名为“组A”的新状态。 您可能会有另一个任务状态分配给组B，该任务状态也命名为“新状态”，带有3个字母的键NES。 虽然2个状态的名称可以相同，但3个字母的代码始终是唯一的。 有关组状态的详细信息，请参阅创建或编辑组状态。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 筛选器：当状态与不同组关联时，按同名状态显示项目

您可以将具有三个字母键&#x200B;*NST*&#x200B;的任务状态分配给名为&#x200B;*新状态*&#x200B;的组A。 您可能有另一个任务状态分配给组B，该任务状态也名为&#x200B;*新状态*，其键为3个字母&#x200B;*NES。*&#x200B;虽然2个状态的名称可以相同，但3个字母的代码始终是唯一的。\
有关组状态的详细信息，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

使用过滤器生成器，您无法识别具有相同名称的2种状态。 必须使用文本模式来区分2种状态。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改筛选器 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 当状态与不同组相关联时，按同名状态显示项目

1. 例如，转到要为任务列表自定义的筛选器。\
   这同样适用于项目和问题。
1. 单击列表对象的&#x200B;**状态**&#x200B;字段的&#x200B;**添加筛选规则**。\
   例如，在任务报告中，添加&#x200B;**Status Equal New Status**，以便只显示处于&#x200B;**New Status**&#x200B;状态的任务。

   >[!TIP]
   >
   >请注意，对于名为“新状态”的状态，您只有一个选项。

1. 单击&#x200B;**切换到文本模式**。\
   应显示以下代码：
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此处仅显示一个状态。 状态行显示其中一个状态的3个字母键之一。

1. 添加以下2行代码以添加筛选器中缺少的状态：
   <pre>OR:1:状态=NES<br>或:1:状态_模式=in</pre>

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存筛选器**。

   该列表同时显示组A中状态为“新状态”和组B中状态为“新状态”的任务。
