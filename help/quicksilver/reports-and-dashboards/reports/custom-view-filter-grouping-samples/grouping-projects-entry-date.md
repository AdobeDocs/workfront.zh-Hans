---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：按输入日期显示项目'
description: 在此自定义项目分组中，您可以显示按项目输入日期值分组的项目。
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 分组：按输入日期显示项目

在此自定义项目分组中，您可以显示按项目输入日期值分组的项目。

每个分组都会显示其输入日期在以下范围内的项目：

* 过去30天
* 30-60天
* 60天或更早

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

## 按输入日期对项目分组

要应用此分组，请执行以下操作：

1. 转到现有项目报告，或创建新项目报告。\
   有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
1. 单击&#x200B;**报告操作** > **编辑**。
1. 在&#x200B;**分组**&#x200B;选项卡中，单击&#x200B;**添加分组**。
1. 单击&#x200B;**切换到文本模式**。
1. 删除&#x200B;**分组依据**&#x200B;区域中的文本。
1. 将文本替换为以下代码：

   group.0.linkedname=direct
group.0.name=项目条目
group.0.valueexpression=IF(ABS(DATEDIFF({entryDate}，$$TODAY))&lt;=30，&quot;最近30天&quot;，IF(ABS(DATEDIFF({entryDate}，$$TODAY)))>30&amp;&amp;ABS(DATEDIFF({entryDate}，$$TODAY))&lt;=60，&quot;30-60天&quot;，&quot;60天之前&quot;)
group.0.valueformat=atDateAsMonthString
textmode=true

1. 单击&#x200B;**完成** > **保存分组**。
1. （可选）更新分组的名称，然后单击&#x200B;**保存分组**。
