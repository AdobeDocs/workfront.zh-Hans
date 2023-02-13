---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：计算时间和日期差异'
description: 您可以计算以下项之间的差异 — “编辑我”。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# 查看：计算时间和日期差异

>[!IMPORTANT]
>
>您不能计算Adobe Workfront中同一种类的两个不同对象之间的时间和日期差。 例如，您无法计算两个不同项目、任务或问题上两个日期之间的时间和日期差异。

您可以计算以下项之间的差异：

* 同一对象上两个日期字段之间的时间和日期差异
* 对象上的字段与父对象上的其他字段之间的时间和日期差异

>[!TIP]
>
>这些计算显示两个日期之间的天数差。 结果以天为单位显示。 日期字段上的时间戳也会被考虑在内，如果时间戳不匹配，则天数后跟小数。 如果任务延迟完成，则天数将显示为负值。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 计算同一对象上两个日期字段之间的时间和日期差

例如，您可以计算任务的计划完成日期与实际完成日期之间的差值。

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. 转到任务列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列** 并开始在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **添加列** 并开始在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **添加列**，然后单击 **切换到文本模式**.

1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. 单击 **保存**，则 **保存视图**.

## 计算对象上的字段与父对象上的另一个字段之间的时间和日期差异

有关对象及其父项的列表，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
例如，您可以计算任务的计划完成日期与其父任务的计划完成日期或任务所在项目的计划完成日期之间的差异。

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. 转到任务列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列** 并开始在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **添加列** 并开始在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **添加列**，然后单击 **切换到文本模式**.

1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码之一：

   * 要显示项目的计划完成日期与任务计划完成日期之间的差异，请执行以下操作：

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * 要显示父任务的计划完成日期与任务的计划完成日期之间的差异，请执行以下操作：

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. 单击 **保存**，则 **保存视图**.
