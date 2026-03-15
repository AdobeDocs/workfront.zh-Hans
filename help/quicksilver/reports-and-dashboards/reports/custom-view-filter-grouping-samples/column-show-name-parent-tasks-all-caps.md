---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：将父任务的名称显示为全部大写字母
description: 您可以将此列添加到任务视图，以便以所有大写字母显示父任务的名称。
author: Courtney
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 7%

---

# 视图：将父任务的名称显示为全部大写字母

<!--Audited: 10/2024-->

您可以将此列添加到任务视图，以便以所有大写字母显示父任务的名称。

![具有父任务的列（全部大写）](assets/column-task-with-all-caps-parent-350x112.png)

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
   <p>用于修改过滤器的参与者或请求 </p>
   <p>用于修改报表的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报表、功能板、日历的访问权限以修改报表</p> <p>编辑对筛选器、视图、分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的详细信息，请参阅[Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将父任务的名称显示为全部大写字母

要在任务视图中生成此列，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**查看**&#x200B;下拉菜单中，选择一个视图，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
或\
   从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新视图**。

1. 在&#x200B;**列预览**&#x200B;区域中，单击列表中显示任务名称的列的标题。
1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，并将其替换为以下代码：

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。
