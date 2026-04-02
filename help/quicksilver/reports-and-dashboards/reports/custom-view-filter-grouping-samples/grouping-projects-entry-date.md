---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：按输入日期显示项目
description: 在此自定义项目分组中，您可以显示按项目输入日期值分组的项目。
author: Courtney
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 7%

---

# 分组：按输入日期显示项目

<!--Audited: 10/2024-->

在此自定义项目分组中，您可以显示按项目输入日期值分组的项目。

每个分组都会显示其输入日期在以下范围内的项目：

* 过去30天
* 30-60天
* 60天或更早

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
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
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

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. 单击&#x200B;**完成** > **保存分组**。
1. （可选）更新分组的名称，然后单击&#x200B;**保存分组**。
