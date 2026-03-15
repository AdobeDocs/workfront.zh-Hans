---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中编辑报表
description: 您可以在创建画布功能板报表之后编辑该报表。
author: Courtney
feature: Reports and Dashboards
exl-id: fd659f56-d67f-4a0f-8735-b214934903ac
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 5%

---

# 在画布功能板中编辑报表

>[!IMPORTANT]
>
>画布功能板功能当前仅对参与测试版阶段的用户可用。 在此阶段中，特征的某些部分可能无法完成或按预期工作。 请按照“画布功能板”测试版概述文章[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分中的说明，提交有关您的体验的任何反馈。<br>
>如果您对可能的错误或技术问题有反馈意见，请向Workfront支持部门提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，此测试版在以下云提供商上不可用：
>
>* 自带钥匙Amazon Web Services
>* Azure
>* Google Cloud Platform

将报告添加到画布仪表板后，可以编辑报告的信息以更改仪表板中显示的数据。

对报告所做的任何更改都将影响有权访问包含该报告的仪表板的所有用户。


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
   <td><p>对报告、仪表板和日历的编辑访问权限</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>管理功能板的权限</p>
  </td> 
  </tr>
</tbody> 
</table>

有关此表中信息的详细信息，请参阅[Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

您必须先将报表添加到功能板，然后才能编辑该报表。

有关详细信息，请参阅[创建画布仪表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 编辑报告

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 在&#x200B;**画布功能板**&#x200B;页面上，单击要编辑的报表右上角的&#x200B;**更多** ![更多图标](assets/more-icon.png)图标，然后选择&#x200B;**编辑**。

   ![编辑报表](assets/edit-report-box.png)

1. 在&#x200B;**配置**&#x200B;对话框中，编辑左侧部分中的信息。 这些部分将因您编辑的报表类型而异。

1. （可选）如果编辑KPI报表，请根据需要在以下部分中编辑信息：

   * **详细信息**
   * **生成KPI**
   * **过滤器**
   * **向下钻取列设置**
   * **深入分析组设置**

   有关这些部分的详细信息，请参阅[构建KPI报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md)。

1. （可选）如果编辑图表报告，请根据需要编辑以下部分中的信息：

   * **详细信息**
   * **生成图表**
   * **过滤器**
   * **深入分析列设置**
   * **深入分析组设置**

   有关这些部分的详细信息，请参阅[生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)。

1. （可选）如果编辑表格报告，请根据需要编辑以下部分中的信息：

   * **详细信息**
   * **生成表**
   * **过滤器**
   * **组设置**

   有关这些部分的详细信息，请参阅[生成表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md)。

1. 单击&#x200B;**保存**&#x200B;以更新报告。

## 编辑现有报告

编辑现有报告时，您选择的报告数据将覆盖当前显示在小组件中的数据。 如果要添加其他现有报告而不是替换某个报告，建议您创建一个单独的报告小部件。

有关详细信息，请参阅[将现有报表添加到画布仪表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md)

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布仪表板**。

1. 在&#x200B;**画布仪表板**&#x200B;页面，单击要编辑的报告右上角的&#x200B;**更多** ![更多](assets/more-icon.png)图标，然后选择&#x200B;**编辑**。

1. 在“**报告选择**”框中，单击要用来替换现有报告小组件数据的报告的&#x200B;**直接添加**。
