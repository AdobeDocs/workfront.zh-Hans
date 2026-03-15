---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：在列中添加任务后续任务列表
description: 您可以在任务视图中添加一列，以显示任务的后续任务列表。 “任务后续任务”列包含后续任务的编号以及名称。
author: Courtney
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 7%

---

# 视图：在列中添加任务后续程序的列表

<!--Audited: 11/2024-->

您可以在任务视图中添加一列，以显示任务的后续任务列表。 **任务后续任务**&#x200B;列包含后续任务的编号以及名称。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或请求修改筛选器 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑筛选器、视图、组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 在列中添加任务后续程序的列表

要将此列添加到任务视图，请执行以下操作：

1. 转到任务列表。
1. 展开&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**新建视图**。
1. 单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 删除&#x200B;**编辑文本模式**&#x200B;框中的所有文本，并将其替换为以下代码：

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。
