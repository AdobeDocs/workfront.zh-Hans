---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中对报表数据进行分组
description: 将报告结果组织成组。 根据报表类型，分组的作用会有所不同。
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 4%
---
# 在画布功能板中对报表数据进行分组

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

分组将组织您的报告结果，以便相关记录显示在一起。 分组的工作方式取决于报表类型，因此本文为每种类型提供了一个单独的部分。

## 访问要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>“任一” </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>标准</p> 
<p>规划</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td><p>编辑对报告、功能板和日历的访问权限</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>管理仪表板的权限</p>
  </td> 
  </tr>
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

您必须在功能板上拥有报表或正在构建报表，然后才能对其数据进行分组。 有关详细信息，请参阅[创建画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 对表格报表中的行进行分组

在表报表中，分组将组织报表本身的行。

1. 在&#x200B;**配置**&#x200B;对话框中，单击左侧面板中的&#x200B;**群组设置**&#x200B;图标。

1. 单击&#x200B;**添加分组**，然后选择要作为分组依据的字段。 该分组将显示在右侧的预览中。

1. （可选）重复以上步骤以添加更多分组。

## 在图表和KPI报告中配置深入分析分组

在图表和KPI报表中，您不需要将主要可视化图表分组。 相反，您可以配置在查看者钻取值时如何对明细表进行分组。

1. 在&#x200B;**配置**&#x200B;对话框中，单击左侧面板中的&#x200B;**深入分析组设置**&#x200B;图标。

1. 单击&#x200B;**添加分组**，然后选择要作为明细表分组依据的字段。

## 在数据透视表中配置区段

数据透视表不使用分组。 相反，您最多定义两个区段，这两个区段是透视量度分组和汇总的类别。

1. 在&#x200B;**配置**&#x200B;对话框中，单击左侧面板中的&#x200B;**区段**&#x200B;图标。

1. 单击&#x200B;**添加区段**，然后选择所需的字段。 区段在预览中显示为一列。

1. （可选）重复以上步骤以添加第二个区段。 您最多可以添加两个区段。

## 在仪表板上查看分组数据

报表查看器可以展开、折叠和排序分组数据。 有关详细信息，请参阅[使用画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)中的[查看包含分组数据的报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data)。
