---
title: 创建或自定义问题严重程度
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您的用户可使用严重程度来定义问题的严重程度。 您可以自定义Adobe Workfront中存在的五种默认严重性中的任意一种，或者为用户创建新严重性。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 4%

---

# 创建或自定义问题严重性

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

您的用户可使用严重程度来定义问题的严重程度。 您可以自定义Adobe Workfront中存在的五种默认严重性中的任意一种，或者为用户创建新严重性。

>[!NOTE]
>
>任务和项目没有严重性。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

## 内置问题严重性

Workfront有五个内置的问题严重性：

* 轻微
* 导致混淆
* 有变通方案的错误
* 没有变通方案的错误
* 致命错误

您可以对这些严重程度编辑以下内容：

* 名称
* 颜色

  如果您按“问题严重性”对结果进行分组，则严重性的颜色将保留在图表报告中。 有关图表报表的信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 默认严重程度

  有关默认严重程度的更多信息，请参阅本文中的[创建或编辑问题严重程度](#create-or-edit-an-issue-severity)。

* 描述
* 严重程度是否隐藏在Workfront中

  有关隐藏严重程度的详细信息，请参阅本文中的[创建或编辑问题严重程度](#create-or-edit-an-issue-severity)。

* 删除严重程度

  执行此操作时，必须选择替换严重性。

## 创建或编辑问题严重性 {#create-or-edit-an-issue-severity}

作为Workfront管理员，您可以根据用户的需求创建和编辑问题严重性。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项** > **严重程度**。

1. 如果要创建新的严重程度，请单击表&#x200B;<span class="preview">**底部的**&#x200B;新行</span>，或单击&#x200B;**添加新严重程度**。
1. 为新严重性配置以下选项或编辑现有严重性的选项：

   * **严重性名称**：键入严重性的名称。
   * **重要性**：提高或降低由Workfront最初分配的严重性级别。

     每个严重程度的重要性数字必须是唯一的。 最高编号对应于最高级别的严重性。

     保存严重性后无法编辑此数字。

   * **颜色**：选择严重程度的颜色。

     当您按“问题严重性”对结果进行分组时，会在图表报告中使用严重性的颜色。 有关图表报表的信息，请参阅[将图表添加到报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

   * **默认严重性**：选择您希望Workfront自动应用于所有新创建问题的严重性。

     在Workfront中，**表面**&#x200B;是问题的默认严重程度。

     您不能将隐藏严重性设置为默认值。

     <div class="preview">

     默认严重性以图标![默认严重性图标](assets/default-icon.png)表示。 要选择新的缺省值，请执行下列操作之一：

      * 选中严重性名称旁边的复选框，然后在屏幕底部的操作栏中选择&#x200B;**设为默认值**。
      * 将鼠标悬停在严重性名称上，然后单击出现的&#x200B;**更多**&#x200B;菜单。 然后，选择&#x200B;**设为默认值**。

        新的默认严重性带有图标的标签。

     </div>

   * **描述**：键入严重程度的描述以说明其功能。
   * <span class="preview">**隐藏选择**</span>&#x200B;或&#x200B;**隐藏**： <span class="preview">选择&#x200B;**是**</span>&#x200B;或选中此复选框以隐藏不再需要的严重程度。

     隐藏的严重性未在Workfront的任何位置显示，因此用户无法为其问题选择它。

     >[!IMPORTANT]
     >
     >我们建议您隐藏严重程度，而不要删除您不想再使用的严重程度。 这样，您就可以保留已使用严重性完成对象的所有历史数据，同时防止他人将来使用严重性。

1. （可选）通过按所需顺序拖放严重程度来更改其列表顺序。

   这会更改它们在问题中的显示顺序。 它不会更改&#x200B;**重要性**&#x200B;数字。

1. 单击&#x200B;**保存**。

有关如何在处理问题时使用严重程度的更多信息，请参阅[更新问题严重性](../../../manage-work/issues/issue-information/update-issue-severity.md)。
