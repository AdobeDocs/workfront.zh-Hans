---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中过滤报表
description: 在报表中添加或编辑过滤器，以控制哪些数据会在画布功能板中显示。
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
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 5%
---
# 在画布功能板中过滤报表

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

无论是在构建报表时还是在随后任何时间，您都可以过滤报表以控制显示哪些数据。 无论哪种情况，过滤选项和行为都是相同的。

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

您必须在功能板上拥有报表或正在构建报表，然后才能对其进行过滤。 有关详细信息，请参阅[创建画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 添加或编辑报告过滤器

要在报表中添加或编辑过滤器，请执行以下操作：

1. 打开报表的过滤器面板：

   * 如果要构建报表，请单击&#x200B;**配置**&#x200B;对话框左侧面板中的&#x200B;**筛选器**&#x200B;图标。
   * 如果您正在编辑现有报表，请单击右上角的&#x200B;**更多**&#x200B;图标，选择&#x200B;**编辑**，然后单击“**配置**”对话框中的&#x200B;**筛选器**&#x200B;面板。

1. 单击&#x200B;**编辑筛选器**。

1. 单击&#x200B;**添加条件**，然后定义条件：

   * 单击&#x200B;**选择字段**，然后选择要作为筛选依据的字段。
   * 选择定义字段必须满足哪种条件的修饰符。
   * 如果修改量需要值，请键入或选择计算值。

   ![添加条件](assets/add-condition.png)

1. （可选）重复上一步以添加更多条件。

1. （可选）单击&#x200B;**添加筛选器组**&#x200B;以添加另一组筛选条件。 集合之间的缺省运算符是AND。 单击运算符以将其更改为OR。

>[!NOTE]
>
>有关字段、运算符、通配符和特殊筛选规则的完整列表，请参阅[画布功能板的报告过滤器引用](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)。

1. 单击&#x200B;**保存**。
