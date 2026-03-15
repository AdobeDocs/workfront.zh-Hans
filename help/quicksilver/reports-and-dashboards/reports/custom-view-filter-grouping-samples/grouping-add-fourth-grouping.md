---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：向列表中添加第四个分组
description: 矩阵报表中可包含4个分组。 有关矩阵报表的更多信息，请参阅创建矩阵报表。
author: Courtney
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---

# 分组：向列表中添加第四个分组

<!--Audited: 10/2024-->

矩阵报表中可包含4个分组。 有关矩阵报表的详细信息，请参阅[创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

通过标准界面，标准报表中只能有3个分组。 要在标准报表中添加第4个分组，必须使用文本模式。

![Four_groupings_in_a_standard_report.png](assets/four-tier-grouping-for-tasks-350x239.png)

例如，您可能有一个按项目名称、进展状态和计划完成日期分组的任务报表，但您还需要按分配至名称对报表分组。

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

## 向列表添加第四个分组

要添加第四个分组，请执行以下操作：

1. 单击&#x200B;**切换到文本模式**。
1. 删除&#x200B;**分组报表**&#x200B;区域中的文本。
1. 将显示的框中的文本替换为以下代码：

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存分组**。
1. （可选）更新分组的名称，然后单击&#x200B;**保存分组**。
