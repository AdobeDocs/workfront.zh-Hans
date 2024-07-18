---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：在列中添加任务后置任务列表'
description: 您可以在任务视图中添加一列，以显示任务的后续任务列表。 “任务后置任务”列包括后置任务的数目以及名称。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 视图：在列中添加任务后续任务列表

您可以在任务视图中添加一列，以显示任务的后续任务列表。 **任务后置任务**&#x200B;列包含后置任务编号和名称。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在列中添加任务后置任务列表

要将此列添加到任务视图，请执行以下操作：

1. 转到现有任务视图。
1. 展开“视图”下拉菜单，然后选择&#x200B;**自定义视图**。
1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在此列&#x200B;**区域中的**&#x200B;显示上，然后单击&#x200B;**单击以编辑文本**。

1. 删除“文本模式”框中的所有文本，然后将其替换为以下代码：
   <pre>displayname=Task Successors<br>listdelimiter=<br><br>listmethod=nested(successors)。lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor})。{taskNumber}，' - '，{successor}。{name})<br>valueformat=HTML</pre>

1. 单击&#x200B;**保存视图**。
