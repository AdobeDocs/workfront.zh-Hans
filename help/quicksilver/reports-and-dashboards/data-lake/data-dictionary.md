---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: 数据湖数据字典
description: 本页包含有关Workfront数据湖中数据的结构和内容的信息。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 7%

---

# Workfront数据湖数据字典

本页包含有关Workfront数据湖中数据的结构和内容的信息。

>[!NOTE]
>
>Workfront数据湖中的数据每四小时刷新一次，因此可能不会立即反映最近的更改。

## 表类型

您可以使用许多表类型以最深入地查看Workfront数据。

* **当前表**

  当前表反映的数据与Workfront中的数据、每个对象及其当前状态类似。 但是，与Workfront相比，它可以以低得多的延迟进行导航。

* **事件表**

  “事件”表格将跟踪Workfront中的每个更改记录：即，每次对象更改状态时，都将创建一个记录以显示更改的时间、进行更改的人员以及更改的内容。 因此，此表对于时间点比较很有用。 此表仅包括过去三年的记录。

* **“每日历史记录”表**

  “每日历史记录”表提供了“事件”表的缩写版本，它以每日为基础显示每个对象的状态，而不是显示每个单独事件发生时的状态。 因此，此表可用于趋势分析。

<!-- Custom table -->

## 实体关系图

Workfront中的对象（因此也是数据湖中的对象）不仅由其单个值定义，而且还由其与其他对象的关系定义。 下面的实体关系图提供了Workfront数据湖中对象关系的高级映射。 可以使用以下链接查看和下载图表：

[Workfront数据湖实体关系图](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>实体关系图是正在进行的工作 — 因此，它仅供参考，并且可能会发生更改。

## 术语表

下表将Workfront中的对象名称（以及它们在接口和API中的名称）与其在数据湖中的等效名称相关联。

<table>
<thead>
  <tr>
    <th>Workfront实体名称</th>
    <th>界面引用</th>
    <th>API参考 | 标签</th>
    <th>数据湖表</th>
    <th>注释</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>任务</td>
    <td>任务</td>
    <td>分配 | 指定任务</td>
    <td>ASSIGNATIONS_CURRENT<br>ASSIGNMENTS_DAY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>条件、优先级、严重性、状态</td>
    <td>系统 | 自定义枚举</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>记录类型通过“enumClass”属性标识。 以下是预期类型：<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>文档</td>
    <td>文档</td>
    <td>DOCU | 文档</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>文档版本</td>
    <td>文档版本</td>
    <td>DOCV | 文档版本</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>组</td>
    <td>组</td>
    <td>组 | 组</td>
    <td>组_当前<br>GROUPS_DAY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>小时</td>
    <td>小时</td>
    <td>HOUR | 小时</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>小时数类型</td>
    <td>小时数类型</td>
    <td>小时 | 小时类型</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>里程碑</td>
    <td>里程碑</td>
    <td>英里 | 里程碑</td>
    <td>MILESTONE_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>里程碑路径</td>
    <td>里程碑路径</td>
    <td>MPATH | 里程碑路径</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATH_DAILY_HISTORY<br>MILESTONEPATH_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>注释</td>
    <td>注释</td>
    <td>注意 | 注意</td>
    <td>注释_当前<br>NOTES_DAILY_HISTORY<br>注释事件</td>
    <td></td>
  </tr>
  <tr>
    <td>Op 任务</td>
    <td>问题，请求</td>
    <td>OPTASK | 问题</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>项目组合</td>
    <td>项目组合</td>
    <td>端口 | Portfolio</td>
    <td>Portfolio当前<br>Portfolio_每日_历史记录<br>Portfolio事件<br><br>Portfolio_自定义_值_当前<br>Portfolio_CUSTOM_VALUE_DAILY_HISTORY<br>Portfolio_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>项目群</td>
    <td>项目群</td>
    <td>PRGM | 项目</td>
    <td>程序_当前<br>PROGRAMS_DAY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>项目</td>
    <td>项目</td>
    <td>项目 | 项目</td>
    <td>项目当前<br>PROJECTS_DAY_HISTORY<br>项目事件<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>角色</td>
    <td>工作角色</td>
    <td>角色 | 工作角色</td>
    <td>ROLES_CURRENT<br>ROLES_DAY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>计划</td>
    <td>计划</td>
    <td>时间表 | 计划</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>任务</td>
    <td>任务</td>
    <td>任务 | 任务</td>
    <td>任务_当前<br>TASKS_DAY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>团队</td>
    <td>团队</td>
    <td>TEAMOB | 团队</td>
    <td>团队当前<br>TEAMS_DAY_HISTORY<br>团队事件</td>
    <td></td>
  </tr>
  <tr>
    <td>时间表</td>
    <td>时间表</td>
    <td>TSHET | 工时表</td>
    <td>TIMESHEETS_CURRENT<br>工时表_每日_历史记录<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>用户</td>
    <td>用户</td>
    <td>用户 | 用户</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
