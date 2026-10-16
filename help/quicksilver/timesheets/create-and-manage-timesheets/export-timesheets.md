---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 导出时间表列表
description: 作为人员经理或时间表批准者，您可能需要下载时间表列表以快速查看有关您负责人员时间表的信息。 您可以通过导出时间表列表来完成此操作。
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 6%
---
# 导出时间表列表

<!--Audited: 8/2024-->

作为人员经理或时间表批准者，您可能需要下载时间表列表以快速查看有关您负责人员时间表的信息。 您可以通过导出时间表列表来完成此操作。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>浅色或更高 </p>
   <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看或更高权限的任务和问题</p> </td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>查看任务或问题的权限或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 导出时间表列表

{{step1-to-timesheets}}

默认情况下，将显示您有权查看的所有时间表。

![时间表列表](assets/list-of-all-timesheets.png)

1. （可选）执行以下操作之一以更新时间表列表中的过滤器：

   * 选择页面右上角的&#x200B;**我的工时表批准**&#x200B;以仅查看您批准的时间表，

     或

     选择&#x200B;**我的时间表**&#x200B;以仅查看您的时间表。

     这会将&#x200B;**我的工时表批准**&#x200B;或&#x200B;**我的工时表**&#x200B;筛选器应用到工时表列表。

   * 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-nwepng.png)以应用筛选器或创建新筛选器。 有关创建或更新筛选器的信息，请参阅[在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从“设置”区域的“列表控件”或您的“布局模板”中删除了筛选器，则“我的时间表审批”和“我的时间表”选项不会显示在时间表列表的顶部或筛选器列表中。 有关详细信息，请参阅[使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. （可选）单击&#x200B;**视图** ![视图图标](assets/view-icon.png)或&#x200B;**分组** ![分组图标](assets/grouping.png)图标以应用视图或分组或创建新视图或分组。

   有关创建过滤器、视图或分组的信息，请参阅以下文章：

   * [在Adobe Workfront中创建或编辑筛选器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中创建或编辑视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中创建分组](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 选择要导出的时间表，然后单击&#x200B;**导出** ![导出图标](assets/export-38x15.png)图标。

   ![单击“导出”图标](assets/export-timesheets.png)

1. 从以下选项中选择要将时间表列表导出到的文件类型：

   * PDF Ladscape
   * PDF纵向
   * PDF其他大小
   * Excel
   * Excel (xlsx)
   * 制表符分隔

   以选定格式下载到计算机中的时间表列表包含以下时间表信息：

   * Date Range
   * 所有者名称
   * 总小时数
   * 加班金额
   * 审批者姓名
   * 状态
