---
title: 创建或自定义问题严重性
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您的用户可以使用严重性来定义问题的严重程度。 您可以自定义Adobe Workfront中现有的五个默认严重性中的任何一个，或为用户创建新的严重性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# 创建或自定义问题严重性

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

您的用户可以使用严重性来定义问题的严重程度。 您可以自定义Adobe Workfront中现有的五个默认严重性中的任何一个，或为用户创建新的严重性。

>[!NOTE]
>
>任务和项目不具有严重性。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 内置问题严重性

Workfront有五个内置的问题严重性：

* 轻微
* 导致混淆
* 有变通方案的问题
* 没有变通方案的问题
* 致命错误

<p>您可以为这些严重性编辑以下内容：</p>

* 名称
* 颜色

   如果按问题严重性对结果进行分组，则严重性的颜色将保留在图表报表中。 有关图表报表的信息，请参阅 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 默认严重性为

   有关默认严重性的更多信息，请参阅 [创建或编辑问题严重性](#create-or-edit-an-issue-severity) 在本文中。
* 描述
* 是否在Workfront中隐藏严重性

   有关隐藏严重性的详细信息，请参阅 [创建或编辑问题严重性](#create-or-edit-an-issue-severity")

* 删除严重性

   执行此操作时，必须选择替换严重性。

## 创建或编辑问题严重性 {#create-or-edit-an-issue-severity}

作为Workfront管理员，您可以创建和编辑问题严重性以满足用户的需求。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **项目首选项** > **严重性**.

1. 如果要创建新的严重性，请单击 **添加新的严重性**.
1. 为新严重性配置以下选项，或对现有严重性进行编辑：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">严重程度名称</td> 
      <td>键入严重性的名称</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要性</td> 
      <td>提高或降低最初由Workfront分配的严重性级别。
      <p>每个严重性的重要性编号必须唯一。 最高值对应于最高严重级别。</p> <p>保存严重性后，便无法编辑此数字。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>选择严重性的颜色。</p> 
      <p>按问题严重性对结果进行分组时，将在图表报表中使用严重性的颜色。 有关图表报表的信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">将图表添加到报表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认严重程度</td> 
      <td>选择您希望Workfront自动选择所有新创建问题的严重性。</p>
      <p>外观是Workfront中问题的默认严重性。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入严重性的描述以解释其函数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐藏</td> 
      <td> 隐藏不再需要的严重性。 
      <p>隐藏的严重性在Workfront中的任何位置都不显示，因此用户无法针对自己的问题进行选择。</p> 
      <p><b>重要信息</b>:我们建议您隐藏不再希望使用的严重性，而不是删除这些严重性。 这样，您就可以保留关于已填写且严重性为的对象的所有历史数据，同时防止将来使用严重性。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）按所需顺序拖放服务器的列表顺序，以更改其列表顺序。

   这会更改问题的显示顺序。 它不会更改 **重要性** 数字。

1. 单击&#x200B;**保存**。

有关如何在处理问题时使用严重性的详细信息，请参阅 [更新问题严重性](../../../manage-work/issues/issue-information/update-issue-severity.md).
