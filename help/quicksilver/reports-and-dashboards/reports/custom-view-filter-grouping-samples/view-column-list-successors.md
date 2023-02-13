---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：在列中添加任务后续项列表
description: 您可以向任务视图添加列，以显示任务后续项的列表。 “任务后继者”列包括后继者的编号和名称。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 查看：在列中添加任务后续项列表

您可以向任务视图添加列，以显示任务后续项的列表。 的 **任务后继者** 列包括后继项的编号和名称。

![task_view_with_a_list_of_subsifers_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## 在列中添加任务后续项列表

要将此列添加到任务视图，请执行以下操作：

1. 转到现有任务视图。
1. 展开“视图”下拉菜单，然后选择 **自定义视图**.
1. 单击 **添加列**.
1. 单击 **切换到文本模式**.
1. 将鼠标悬停在 **在此列中显示** ，然后单击 **单击以编辑文本**.

1. 删除“文本模式”框中的所有文本，并将其替换为以下代码：

   <pre>displayname=任务后继者<br>listdelimiter=<br><br>listmethod=nested(subsers)。lists<br>textmode=true<br>type=interate<br>valueexpression=CONCAT（{后继者}）。{taskNumber},' - ',{后继者}。{name})<br>valueformat=HTML</pre>

1. 单击 **保存视图**.
