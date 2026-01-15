---
product-area: Canvas Dashboards
navigation-topic: canvas-dashboards
title: 使用画布功能板
description: 使用画布功能板
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 41e283ceccd0a95daae005d998a2ed8050a1ab0b
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# 使用画布功能板

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。
>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。
>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

画布功能板允许您通过将不同的报表类型添加到灵活的画布布局来可视化Adobe Workfront数据。 本文概述如何有效使用画布功能板。

## 访问画布功能板

要访问画布功能板，请导航到Adobe Workfront中的功能板部分。 从该位置，您可以查看现有功能板，如果您具有必要的权限，也可以创建新功能板。

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。
1. 单击现有仪表板的名称以将其打开。
   ![打开仪表板](assets/open-dashboard.png)

<!--## Navigating the Dashboard

Once you open a Canvas Dashboard, you can interact with the reports displayed on the dashboard. You can resize, drag, and drop reports to customize the layout according to your preferences.

## Add dashboard to favorites

-->

## 与报表交互

您可以与功能板上的单个报表进行交互。

### 临时自定义表格报表

您可以临时自定义功能板上的表格报表。 这些更改仅适用于当前会话，不会影响原始报告配置。

1. 在左侧面板中，单击&#x200B;**画布功能板**。
1. 单击现有仪表板的名称以将其打开。
   ![打开仪表板](assets/open-dashboard.png)
1. 找到要自定义的表报表。
1. 选择以下任一选项以自定义报表：

   | 选项 | 描述 |
   |--------|-------------|
   | **添加列** | 单击&#x200B;**添加列**&#x200B;以向报表中添加其他列。 |
   | **配置列** | 选择显示或隐藏报表中的特定列。 |
   | **行高** | 调整报表的行高。 |
   | **对齐滚动** | 启用或禁用快照滚动，以便更轻松地在报告中导航。 |

   >[!IMPORTANT]
   >
   >这些更改仅适用于当前会话，不会影响原始报告配置。 若要永久设置这些更改，您需要编辑报告。


<!--

### Quick Search 

### Filter
### Use drilldowns


You can use drilldowns in Canvas Dashboards to sort and group data within reports.

1. In the left panel, click **Canvas Dashboards**.
1. Click the name of an existing dashboard to open it.
    ![Open a dashboard](assets/open-dashboard.png)
1. Locate the report that you want to look at.
1. Click on a data point within the report to drill down into more detailed information.
1. Click the Show build table icon to open the drilldown settings. 
1. Click Add Column to add additional columns to the drilldown table.

 >[!IMPORTANT]
>
>These changes only apply to your current session and do not affect the original report configuration. To make permanent these changes, you need to edit the report.

### Add additional columns to table reports


## View reports with grouped data

Report creators can configure reports to display grouped data. When viewing these reports on a Canvas Dashboard, you can expand or collapse the grouped data to see more or less detail.

Data within groups is sorted alphabetically or chronologically by default, depending on the data type. You can click the column headers to sort the data within each group based on different attributes. When you sort by a different attribute, the order of the groups remains unchanged.

When you sort by the same field that your report is grouped by, the group order can flip. For example, a text-based grouping that normally runs A–Z can switch to Z–A. This only happens when the sort column and the grouping attribute are the same.


## Saving and Sharing Dashboards

After customizing your Canvas Dashboard, you can save your changes. Additionally, you can share the dashboard with other users in your organization, provided you have the appropriate sharing permissions.

For more detailed instructions on creating, managing, and customizing Canvas Dashboards, refer to the related articles in the [Canvas Dashboards overview](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md) section.-->

## 查看包含分组数据的报表

报告创建者可以配置报告以显示分组数据。 当报表具有分组时，您可以展开或折叠分组的数据以查看更多或更少的详细信息。

默认情况下，分组本身将按字母顺序或时间顺序排序，具体取决于字段类型。 每个分组中的数据与分组排序顺序无关。

您可以单击列标题对每个组中的数据进行排序。 当按与分组字段不同的字段排序时，组的顺序不会更改。

但是，当您按报告分组依据的相同字段排序时，分组顺序可能会更改。 例如，通常运行A-Z的基于文本的分组可能会切换到Z-A。