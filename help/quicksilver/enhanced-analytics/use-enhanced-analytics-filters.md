---
title: 在增强的分析中应用过滤器
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 增强分析区域中的过滤器可帮助您专注于特定项目或特定类型的数据。
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 1%

---

# 在增强的分析中应用过滤器

增强分析区域中的过滤器可帮助您专注于特定项目或特定类型的数据。 您使用的过滤器类型可以让您对以下内容进行分析：

* 您拥有的项目
* 特定的项目组合或项目群视图
* 特定时间范围（周、季度、财政年度）的关键绩效指标

您可以根据需要添加和删除筛选器，Adobe Workfront会保留您应用的筛选器，即使您注销也是如此。

## 访问要求

要完成此任务，您必须具备以下条件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</p> </td> 
   <td>业务或更高</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</p> </td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td><b>访问级别*</b> </td> 
   <td> <p>查看对项目的访问权限</p> <p>您还必须具有“任务”、“Portfolio”和“用户”的“查看”权限才能查看特定项目字段筛选器选项。</p> <p>注意：如果在“编辑访问级别”对话框的“设置其他限制”部分中选择了限制，则在应用过滤器后，您可能无法看到过滤器或“增强分析”页面上的所有信息。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>对象权限</b> </p> </td> 
   <td> <p>查看</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

有关使用增强型分析的先决条件，请参阅 [先决条件](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) 在 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 更改日期范围筛选器 {#change-the-date-range-filter}

默认情况下，“增强分析”区域中的可视化图表显示过去60天和未来15天的数据。 您可以选择新日期范围，并将其应用于增强分析区域中的所有可视化图表。 如果您离开页面，则会在下次导航回该页面时应用默认日期范围。

>[!TIP]
>
>您还可以使用键盘上的键导航、打开并从日历小组件中选择日期范围。\
>欲了解更多信息，请参见 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 部分内容 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

要选择新的日期范围，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **分析**.
1. 在屏幕右上角，单击日期范围字段以打开日历视图。
1. 使用日历上方的箭头查找开始日期的月份，然后选择开始日期。

   ![](assets/filters-select-date-range-350x344.png)

1. 使用日历上方的箭头查找结束日期的月份，然后选择结束日期。
1. （可选）要放大较小的日期范围，请将鼠标从一个可视化图表上的特定日期拖动到另一个特定日期。

   屏幕上的所有可视化都会更新以匹配选定的时间范围，并且时间范围过滤器将显示在任何现有过滤器旁边。 如果您注销或离开增强型分析区域，则不会保留此过滤器。

   ![](assets/timeframe-filter-350x220.png)

## 添加筛选器

您可以添加基于默认项目字段、自定义表单字段和分配给项目的主团队的筛选器。

>[!TIP]
>
>您还可以使用键盘上的键导航到并添加新筛选器。\
>欲了解更多信息，请参见 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 部分内容 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

* [添加项目字段筛选器](#add-a-project-field-filter)
* [添加项目字段筛选器](#add-a-project-field-filter)
* [添加团队筛选器](#add-a-team-filter)

### 添加项目字段筛选器 {#add-a-project-field-filter}

项目字段筛选器允许您根据默认包含在项目中的字段中输入的值来筛选项目和任务的数据。

以下项目字段筛选器类型可用：

| **项目** | 仅显示选定项目的数据 |
|---|---|
| **项目群** | 仅显示选定项目群中的项目数据 |
| **项目组合** | 仅显示选定项目组合中的项目数据 |
| **完成情况** | 仅显示最近具有选定完成情况（符合目标、存在风险或存在问题）的项目的数据 |
| **状态** | 仅显示最近具有选定状态（完成、当前、暂挂、已取消等）的项目的数据 |
| **发起人** | 仅显示具有选定赞助者的项目的数据 |
| **项目所有者** | 仅显示具有选定项目所有者的项目的数据 |

{style="table-layout:auto"}

自定义表单过滤器的工作方式不同。 有关更多信息，请参阅 [添加项目字段筛选器](#add-a-project-field-filter).

要添加项目字段筛选器，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **分析**.
1. 在屏幕的左上角，单击 **添加筛选器**，然后选择所需的过滤器类型。

   >[!NOTE]
   >
   >不同的过滤器类型显示不同的数据。 一个过滤器只能使用一个过滤器类型。 选定后，某个筛选器类型不可用于其他项目字段筛选器。

1. 通过在“ ”中输入至少3个字符的文本，找到要查看其数据的值。 **Search** 字段中，然后选择要包含在过滤器中的每个值。

   要选择所有当前值，请单击 **全选**.

   ![](assets/select-filter-value-350x251.png)

1. 选择所有所需值后，单击 **应用筛选器**.\
   页面右上角的项目计数将更新，以反映应用的过滤器。
1. 对要添加的每个筛选器重复这些步骤。

   添加过滤器时，数据会显示在下面最多50个项目的可视化图表中。

   >[!TIP]
   >
   >要查看默认显示的50多个项目的数据，您可以：
   >
   >   
   >   
   >   * 使用左下角的箭头可在该可视化图表中显示接下来的50个项目。\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的排序方式下拉菜单，按不同顺序查看项目。\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   要调整日期范围，请参阅 [更改日期范围筛选器](#change-the-date-range-filter).

### 添加项目自定义表单过滤器

“自定义表单”筛选器类型允许您根据在项目的自定义表单字段中输入的值筛选项目和任务的数据。 与其他增强型分析过滤器类型不同，您可以添加多个自定义表单过滤器。 每个自定义表单过滤器仅包含在特定自定义表单的选定字段中输入的值。

要添加自定义表单筛选器：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **分析**.
1. 在屏幕的左上角，单击 **添加筛选器**，然后选择 **自定义表单**.

   ![](assets/select-custom-form-filter-350x271.png)

1. 通过在表单中输入至少3个字符的文本，找到所需的自定义表单 **Search** 字段，然后选择自定义表单。
1. 选择所需的字段，然后根据要添加到过滤器的字段类型完成以下操作之一：

   >[!NOTE]
   >
   >并非所有自定义表单字段类型都可以添加到过滤器。 目前，增强型分析仅支持上面列出的字段类型。

   * **复选框**， **下拉面板**，或 **单选按钮**：选择选定字段中要包含在过滤器中的各个值，或单击 **全选** 复选框。\
     ![](assets/custom-form-filter-checkbox-350x255.png)

   * **日期**：使用箭头导航到特定月份，然后在选定字段中选择要包含在过滤器中的日期。\
     ![](assets/custom-form-filter-date-350x348.png)

   * **文本**：在选定字段中输入要包含在过滤器中的文本。\
     ![](assets/custom-form-filter-text-350x90.png)

   * **数字**：在选定字段中输入要包含在过滤器中的数字。\
     ![](assets/custom-form-filter-number-350x93.png)

1. 输入或选择要过滤的值后，单击 **应用筛选器**.

   页面右上角的项目计数将更新，以反映应用的过滤器。

1. 对要添加的每个筛选器重复这些步骤。

   添加过滤器时，数据会显示在下面最多50个项目的可视化图表中。

   >[!TIP]
   >
   >要查看默认显示的50多个项目的数据，您可以：
   >
   >   
   >   
   >   * 使用左下角的箭头可在该可视化图表中显示接下来的50个项目。\
   >     ![](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的排序方式下拉菜单，按不同顺序查看项目。\
   >     ![](assets/sort-by-menu-350x247.png)
   >   
   >   
   >

   要调整日期范围，请参阅 [更改日期范围筛选器](#change-the-date-range-filter).

### 添加团队筛选器 {#add-a-team-filter}

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **分析**.
1. 在左侧面板中，单击 **人员**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. 在屏幕的左上角，单击 **添加筛选器**，然后选择 **团队** 筛选。
1. 通过在“ ”中输入至少3个字符的文本，找到要查看其数据的团队 **Search** 字段中，然后选择要包含在过滤器中的各个团队。 要选择所有团队，请单击 **全选**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >所有团队都作为过滤器选项包含在内，无论您的访问级别如何。


1. 选择所有所需团队后，单击 **应用筛选器**.

   添加过滤器时，数据会显示在下面的可视化图表中。

   要调整日期范围，请参阅 [更改日期范围筛选器](#change-the-date-range-filter).

## 删除筛选器

您可以随时删除过滤器。 如果删除筛选器，该筛选器在您下次访问增强型分析区域时不会显示。

>[!TIP]
>
>您还可以使用键盘上的键导航到现有筛选器并将其删除。\
>欲了解更多信息，请参见 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 部分内容 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

要删除过滤器，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **分析**.
1. 如果要删除工作筛选器，请保留在 **工作** 区域。

   或

   如果要删除“人员”筛选器，请选择 **人员** 在左侧面板中。

1. 找到所需的过滤器，然后单击 **X** 以删除它。

   ![](assets/remove-filter-350x213.png)

   该过滤器不再处于活动状态，除非您再次添加，否则不会显示。
