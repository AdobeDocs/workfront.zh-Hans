---
title: 在增强的分析中应用过滤器
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Adobe Workfront的“增强分析”区域中的过滤器可帮助您将注意力集中在特定项目或特定类型的数据上。
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# 在增强的分析中应用过滤器

>[!IMPORTANT]
>
>增强型分析已于5月27日从Workfront中删除。 Workfront Data Connect是一种新的替代解决方案，可用于复制您当前使用的任何Enhanced Analytics可视化图表。 <br>有关详细信息，请参阅[Enhanced Analytics弃用](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)指南。


<!-- Audited: 12/2023 -->

Adobe Workfront的“增强分析”区域中的过滤器可帮助您将注意力集中在特定项目或特定类型的数据上。 您使用的过滤器类型可以让您对以下内容进行分析：

* 您拥有的项目
* 特定的项目组合或项目群视图
* 特定时间范围（周、季度、财政年度）的关键绩效指标

您可以根据需要添加和删除筛选器，Workfront会保留您应用的筛选器，即使您注销也是如此。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>
      <p>新建：任何</p>
      <p>或</p>
      <p>当前：业务或更高</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
      <p>新增：浅色或更高</p>
      <p>或</p>
      <p>当前：审阅或更高版本</p>
   </td> 
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>查看对项目的访问权限</p> <p>您还必须具有“任务”、“项目组合”和“用户”的“查看”权限才能查看特定项目字段筛选选项。</p> <p>注意：如果在“编辑访问级别”对话框的<strong>设置其他限制</strong>部分中选择了限制，在应用筛选器后，您可能无法看到筛选器或“增强分析”页面上的所有信息。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>查看</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的[先决条件](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites)。

## 更改日期范围筛选器 {#change-the-date-range-filter}

默认情况下，“增强分析”区域中的可视化图表显示过去60天和未来15天的数据。 您可以选择新日期范围，并将其应用于增强分析区域中的所有可视化图表。 如果您离开页面，则会在下次导航回该页面时应用默认日期范围。

>[!TIP]
>
>您还可以使用键盘上的键导航、打开并从日历小组件中选择日期范围。\
>有关详细信息，请参阅文章[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的[键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts)部分。

要选择新的日期范围，请执行以下操作：

{{step1-to-analytics}}

1. 单击右上角的日期范围字段以打开日历视图。
1. 使用日历上方的箭头查找开始日期的月份，然后选择开始日期。

   ![选择日期范围](assets/filters-select-date-range-350x344.png)

1. 使用日历上方的箭头查找结束日期的月份，然后选择结束日期。
1. （可选）要放大较小的日期范围，请将鼠标从一个可视化图表上的特定日期拖动到另一个特定日期。

   屏幕上的所有可视化都会更新以匹配选定的时间范围，并且时间范围过滤器将显示在任何现有过滤器旁边。 如果您注销或离开增强型分析区域，则不会保留此过滤器。

   ![时间范围筛选器](assets/timeframe-filter-350x220.png)

## 添加筛选器

您可以添加基于默认项目字段、自定义表单字段和分配给项目的主团队的筛选器。

>[!TIP]
>
>您还可以使用键盘上的键导航到并添加新筛选器。\
>有关详细信息，请参阅文章[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的[键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard)部分。

* [添加项目字段筛选器](#add-a-project-field-filter)
* [添加项目自定义表单筛选器](#add-a-project-custom-form-filter)
* [添加团队筛选器](#add-a-team-filter)

### 添加项目字段筛选器 {#add-a-project-field-filter}

项目字段筛选器允许您根据默认包含在项目中的字段中输入的值来筛选项目和任务的数据。

以下项目字段筛选器类型可用：

| 字段 | 显示的数据 |
|---|---|
| **项目** | 仅显示选定项目的数据 |
| **计划** | 仅显示选定项目群中的项目数据 |
| **Portfolio** | 仅显示选定项目组合中的项目数据 |
| **条件** | 仅显示最近具有选定完成情况（符合目标、存在风险或存在问题）的项目的数据 |
| **状态** | 仅显示最近具有选定状态（完成、当前、暂挂、已取消等）的项目的数据 |
| **发起人** | 仅显示具有选定赞助者的项目的数据 |
| **项目所有者** | 仅显示具有选定项目所有者的项目的数据 |

自定义表单过滤器的工作方式不同。 有关详细信息，请参阅[添加项目自定义表单筛选器](#add-a-project-custom-form-filter)。

要添加项目字段筛选器，请执行以下操作：

{{step1-to-analytics}}

1. 单击左上角的&#x200B;**添加筛选器**，然后选择所需的筛选器类型。

   >[!NOTE]
   >
   >不同的过滤器类型显示不同的数据。 一个过滤器只能使用一个过滤器类型。 选择筛选器类型后，该筛选器类型将不可用于其他项目字段筛选器。

1. 通过在&#x200B;**搜索**&#x200B;字段中输入至少三个字符的文本，找到要查看其数据的值，然后选择要包含在筛选器中的每个值。

   要选择所有当前值，请单击&#x200B;**全选**。

   ![选择筛选器值](assets/select-filter-value-350x251.png)

1. 选择所有所需值后，单击&#x200B;**应用筛选器**。

   右上方的项目计数将更新，以反映应用的过滤器。

1. 对要添加的每个筛选器重复这些步骤。

   添加过滤器时，数据会显示在下面最多50个项目的可视化图表中。

   >[!TIP]
   >
   >要查看默认显示的50多个项目的数据，您可以：
   >
   >   * 使用左下方的箭头可在该可视化图表中显示接下来的50个项目。\
   >     ![分页箭头](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的&#x200B;**排序方式**&#x200B;下拉菜单以不同顺序查看项目。\
   >     ![按菜单排序](assets/sort-by-menu-350x247.png)

   要调整日期范围，请参阅[更改日期范围筛选器](#change-the-date-range-filter)。

### 添加项目自定义表单过滤器

自定义表单筛选器类型允许您根据在项目的自定义表单字段中输入的值筛选项目和任务的数据。 与其他增强型分析过滤器类型不同，您可以添加多个自定义表单过滤器。 每个自定义表单过滤器仅包含在特定自定义表单的选定字段中输入的值。

要添加自定义表单筛选器：

{{step1-to-analytics}}

1. 单击屏幕左上角的&#x200B;**添加筛选器**，然后选择&#x200B;**自定义表单**。

   ![选择自定义表单筛选器](assets/select-custom-form-filter-350x271.png)

1. 通过在&#x200B;**搜索**&#x200B;字段中输入至少三个字符的文本，找到所需的自定义表单，然后选择该自定义表单。
1. 选择所需的字段，然后根据要添加到过滤器的字段类型完成以下操作之一：

   >[!NOTE]
   >
   >并非所有自定义corm字段类型都可以添加到过滤器。 目前，增强型分析仅支持下面列出的字段类型。

   * **复选框**、**下拉列表**&#x200B;或&#x200B;**单选按钮**：选择筛选器要包含的字段中的每个值，或单击&#x200B;**全选**&#x200B;复选框。\
     ![复选框值](assets/custom-form-filter-checkbox-350x255.png)

   * **日期**：使用箭头导航到特定月份，然后在字段中选择要包含在筛选器中的日期。\
     ![日期值](assets/custom-form-filter-date-350x348.png)

   * **文本**：在要包含在筛选器中的字段中输入文本。\
     ![文本值](assets/custom-form-filter-text-350x90.png)

   * **数字**：在要包括在筛选器中的字段中输入数字。\
     ![数值](assets/custom-form-filter-number-350x93.png)

1. 输入或选择要筛选的值后，单击&#x200B;**应用筛选器**。

   右上方的项目计数将更新，以反映应用的过滤器。

1. 对要添加的每个筛选器重复这些步骤。

   添加过滤器时，数据会显示在下面最多50个项目的可视化图表中。

   >[!TIP]
   >
   >要查看默认显示的50多个项目的数据，您可以：
   >  
   >   * 使用左下方的箭头可在该可视化图表中显示接下来的50个项目。\
   >     ![分页箭头](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的&#x200B;**排序方式**&#x200B;下拉菜单以不同顺序查看项目。\
   >     ![按菜单排序](assets/sort-by-menu-350x247.png)

   要调整日期范围，请参阅[更改日期范围筛选器](#change-the-date-range-filter)。

### 添加团队筛选器 {#add-a-team-filter}

{{step1-to-analytics}}

1. 在左侧面板中，单击&#x200B;**人员**。

   ![选择人员](assets/people-area-cropped-qs-350x276.png)

1. 在屏幕的左上方，单击&#x200B;**添加筛选器**，然后选择&#x200B;**团队**&#x200B;筛选器。
1. 通过在&#x200B;**搜索**&#x200B;字段中输入至少三个字符的文本，找到要查看其数据的团队，然后选择要包含在筛选器中的各个团队。 要选择所有团队，请单击&#x200B;**全选**。

   ![选择团队](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >所有团队都作为过滤器选项包含在内，无论您的访问级别如何。

1. 选择所有所需团队后，单击&#x200B;**应用筛选器**。

   添加过滤器时，数据会显示在下面的可视化图表中。

   要调整日期范围，请参阅[更改日期范围筛选器](#change-the-date-range-filter)。

## 删除筛选器

您可以随时删除过滤器。 如果删除筛选器，该筛选器在您下次访问增强型分析区域时不会显示。

>[!TIP]
>
>您还可以使用键盘上的键导航到现有筛选器并将其删除。\
>有关详细信息，请参阅文章[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的[键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard)部分。

要删除过滤器，请执行以下操作：

{{step1-to-analytics}}

1. 如果要删除项目字段或自定义表单筛选器，请保留在&#x200B;**工作**&#x200B;区域。

   或

   如果要删除团队筛选器，请在左侧面板中选择&#x200B;**人员**。

1. 找到所需的筛选器并单击&#x200B;**X**&#x200B;将其删除。

   ![移除](assets/remove-filter-350x213.png)

   该过滤器不再处于活动状态，除非您再次添加，否则不会显示。
