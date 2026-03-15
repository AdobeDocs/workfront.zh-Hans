---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：任务列表的项目发起人
description: 此任务分组允许您按项目发起者对任务进行分组。
author: Courtney
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 10%

---

# 分组：任务列表的项目发起人

<!--Audited: 11/2024-->

此任务分组允许您按项目发起者对任务进行分组。

![按项目发起人分组](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## 按项目发起人分组任务列表


要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 删除显示区域中的文本，然后将其替换为以下代码：

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. 单击&#x200B;**完成**。
1. 更新分组名称，然后单击&#x200B;**保存分组**。

