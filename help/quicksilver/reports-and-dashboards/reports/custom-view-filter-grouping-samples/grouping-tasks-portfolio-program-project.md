---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：按Portfolio、方案和项目列出的任务
description: 使用此任务分组可以按产品组合、方案，然后按与其关联的项目对任务进行分组。
author: Courtney
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 8%

---

# 分组：按产品组合、方案和项目列出的任务

<!--Audited: 10/2024-->

使用此任务分组可以按产品组合、方案，然后按与其关联的项目对任务进行分组。

![Portfolio的程序项目分组](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## 按产品组合、计划和项目对任务进行分组

要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。
1. 单击&#x200B;**添加分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 删除&#x200B;**Group by**&#x200B;区域中的文本。
1. 将文本替换为以下代码：

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true
   ```

1. 单击&#x200B;**完成** > **保存分组**。
1. （可选）更新分组名称，然后单击&#x200B;**保存分组**。

