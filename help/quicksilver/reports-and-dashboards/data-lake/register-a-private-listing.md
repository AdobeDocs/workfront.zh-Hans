---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: 注册Workfront Data Connect的专用列表
description: 注册Snowflake私有列表以直接与贵组织的Snowflake帐户共享您的Workfront Data Connect数据。
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
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
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%
---
# 注册Workfront Data Connect的专用列表

通过注册个人列表，您可以直接与组织的Snowflake帐户共享Workfront Data Connect数据。 此连接方法使用Snowflake的私有列表功能在组织之间安全地共享数据而不公开披露数据，并且可以跨区域和托管平台工作。

当您要将Workfront数据与企业数据仓库中的其他数据联接时，私有列表非常有用。 由于数据位于您自己的Snowflake帐户中，因此您可以将其与您的其余数据一起查询。

## 访问权限要求

+++ 展开以查看访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>Ultimate</p>
    <p>工作流 Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

您还需要一个有权接受列表和创建数据库的Snowflake帐户，以及一个Workfront Data Connect权利。

## 非公开上市股票

通过非公开上市，您可以访问以下内容：

* Workfront对象的数据视图超过100个。 有关每个视图的说明，请参阅[Workfront Data Connect数据字典](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)。
* `*_event`数据视图，其中包含交付给Data Connect数据管道的每个更改事务。
* 数据可扩展对象的自定义数据值。 有关示例，请参阅[Workfront Data Connect查询示例](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md)中的自定义数据查询示例。

## 与读取器帐户连接的区别

私有上市共享一组与读者帐户连接不同的视图，并且数据到达不同的计划。 请记住以下差异：

* 个人上市仅共享`*_event`查看。 `*_current`和`*_daily_history`视图可通过读者帐户使用，但不能通过个人列表使用。 您可以在自己的Snowflake帐户中构建这些库。 有关详细信息，请参阅本文中的[设置当前和每日历史记录视图](#set-up-current-and-daily-history-views)。
* 非公开上市可能不包括通过读者账户提供的每个视图。 未共享的视图示例包括Workfront Planning对象`MONITORING_DATA_REFRESHES`、`BOOKINGS`和`CLASSIFIER`。 这份清单并非详尽无遗。
* Data Connect每4小时加载一次更改事件。 由于私有列表需要额外的复制步骤才能呈现数据，因此预计数据到达该列表将需要比通过读取器帐户到达的数据多大约1小时。
* 数据复制在01:01、05:01、09:01、13:01、17:01和21:01 UTC运行。 数据通常在每次运行后约10分钟内可用。
* `MONITORING_DATA_REFRESHES`和`JOB_HISTORY`视图不反映通过私有列表提供数据的时间。 尽管`JOB_HISTORY`视图是通过专用列表共享的，但我们建议通过读者帐户阅读该视图，以便更快地识别失败的作业。

## 注册个人分发名单

要注册个人分发名单，请先收集您的Snowflake帐户详细信息，然后在Workfront中添加该名单。

### 收集您的Snowflake帐户详细信息

Workfront使用您的Snowflake帐户详细信息将列表定向到您的帐户。 收集以下详细信息：

* 帐户定位器
* 帐户URL
* 帐户组织
* 帐户名称

这些值都可以从Snowflake中的“帐户详细信息”模式获得。

要查找您的帐户详细信息，请执行以下操作：

1. 登录Snowflake帐户时，单击左下角的用户菜单。

1. 在菜单的&#x200B;**帐户**&#x200B;部分中选择您的帐户。

1. 单击&#x200B;**查看帐户的帐户详细信息**。

1. 记录上面列出的每个值。

此外，还要确定您要通过访问链接的Workfront数据的数据库的名称。 在注册列表时输入此名称。

### 在Workfront中添加个人分发名单

您可通过Adobe Workfront界面注册个人分发名单。

>[!IMPORTANT]
>
>每个帐户货位只能创建一个专用列表。

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 单击&#x200B;**Snowflake连接**&#x200B;选项卡。

1. 单击&#x200B;**添加个人分发名单**。

1. 使用您收集的帐户详细信息（包括首选数据库名称）填写表单。

1. 单击&#x200B;**添加个人分发名单**。

### 连接到Snowflake中的列表

在您的Snowflake帐户中，建立与专用清单的连接作为外部数据源。 然后，您可以连同其余数据一起查询Workfront数据。

## 设置当前和每日历史记录视图

读取器帐户连接为每个对象表提供三个数据视图：

* **当前** — 数据当前存在于源应用程序中的低延迟表示形式。
* **每日历史记录** — 表示每天晚上11:59 UTC的数据。
* **事件** — 每个已交付到Data Connect数据管道的更改事务。

非公开上市仅共享事件视图。 本节提供SQL来在您自己的Snowflake帐户中构建当前、每日历史记录和事件视图。

此列表中包含的所有事件视图都具有以下视图逻辑所需的字段。 这些示例假定您已在目标Snowflake帐户中创建了您选择的新数据库和架构，并且它们使用`projects_event`视图。 在每个示例中，将`<listing_db>`和`<listing_schema>`替换为您自己的值。

>[!TIP]
>
>我们建议您将`select *`替换为您用于分析的列的列表。 如果您使用`select *`，并且稍后将列添加到列表的事件视图中，则必须重新创建视图以启用新列。

### 当前视图

对象的“当前”视图是存储在“数据连接”中的最后一个变更事件记录。 如果最后一个记录处于已删除状态，则从“当前”视图中忽略该记录。 所有事件视图都具有相同的结构。

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

当前视图中不需要`deleted`和`end_effective_timestamp`列。 视图将数据过滤为一个值，如果删除记录，则完全删除记录。

### 每日历史记录视图

“每日历史记录”视图标识在给定日期的23:59:59处于活动状态的变更事件记录，因此您可以跟踪记录状态随时间的变化趋势。 以下示例给出了每个日历天结束时项目记录的状态。

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### 事件查看

为保持一致性，我们建议您从列表数据库创建事件视图的副本，并将其放在与“当前历史记录”和“每日历史记录”视图相同的架构中。

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
