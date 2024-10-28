---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '筛选器：当状态与不同组关联时，按同名状态显示项目'
description: 您可以将具有3个字母键NST的任务状态分配给名为“组A”的新状态。 您可能会有另一个任务状态分配给组B，该任务状态也命名为“新状态”，带有3个字母的键NES。 虽然2个状态的名称可以相同，但3个字母的代码始终是唯一的。 有关组状态的详细信息，请参阅创建或编辑组状态。
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 筛选器：当状态与不同组关联时，按同名状态显示项目

<!--Audited: 10/2024-->

您可以将具有三个字母键&#x200B;*NST*&#x200B;的任务状态分配给名为&#x200B;*新状态*&#x200B;的组A。 您可能有另一个任务状态分配给组B，该任务状态也名为&#x200B;*新状态*，其键为3个字母&#x200B;*NES。*&#x200B;虽然2个状态的名称可以相同，但3个字母的代码始终是唯一的。

有关组状态的详细信息，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

使用过滤器生成器，您无法识别具有相同名称的2种状态。 您必须在自定义筛选器中使用“文本模式”来区分2种状态。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 当状态与不同组相关联时，按同名状态显示项目

1. 例如，转到要自定义任务列表的筛选器的&#x200B;**筛选器**&#x200B;下拉列表。\
   这同样适用于项目和问题。
1. 单击&#x200B;**新建筛选器**。
1. 从左上角的第一个下拉列表中，选择Task > Status。
1. 为修饰符选择&#x200B;**等于**，然后选择要报告的状态之一。

   例如，在任务报告中，如果只想显示处于&#x200B;**新状态**&#x200B;状态的任务，请添加&#x200B;**状态等于新状态**。

   >[!TIP]
   >
   >请注意，对于名为“新状态”的状态，您只有一个选项。

1. 单击&#x200B;**文本模式**。\
   以下代码应显示在提供的空格中：

   <pre>OR:1:状态=NST<br>或:1:状态_模式=in </pre>

   >[!NOTE]
   >
   >此处仅显示一个状态。 状态行显示其中一个状态的3个字母键之一。

1. 添加以下2行代码以添加筛选器中缺少的状态：

   <pre>OR:2:状态=NES<br>或:2:状态_模式=in</pre>

1. 单击&#x200B;**应用**，然后单击&#x200B;**另存为新项**。

   该列表同时显示组A中状态为“新状态”和组B中状态为“新状态”的任务。
