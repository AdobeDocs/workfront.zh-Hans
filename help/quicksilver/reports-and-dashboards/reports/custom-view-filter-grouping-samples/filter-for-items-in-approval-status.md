---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '筛选器：仅显示处于审批状态的项目'
description: 您只能显示处于特定状态（当前处于“未决批准”中）的项目。 这同样适用于具有审批状态的任何其他对象。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# 筛选器：仅显示处于审批状态的项目

您只能显示处于特定状态（当前处于“未决批准”中）的项目。 这同样适用于具有审批状态的任何其他对象。

您可以将以下对象置于批准状态：

* 任务
* 问题
* 项目

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

## 仅显示处于审批状态的项目

1. 例如，转到要为项目列表自定义的过滤器。
1. 单击列表对象的&#x200B;**状态**&#x200B;字段的&#x200B;**添加筛选规则**。\
   例如，在项目报表中，添加&#x200B;**Status Equal Planning**，以便只显示处于&#x200B;**Planning - Pending Approval**&#x200B;状态的项目。

1. 单击&#x200B;**切换到文本模式**。
1. 修改

   ```
   status
   ```

   通过将&#x200B;**：A**&#x200B;添加到状态的3个字母的键来行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存筛选器**。

   该列表仅显示处于“计划 — 未决批准”状态的项目。
