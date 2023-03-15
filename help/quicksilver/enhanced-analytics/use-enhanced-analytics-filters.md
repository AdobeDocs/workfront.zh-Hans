---
title: 在增强的分析中应用过滤器
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “增强的分析”区域中的过滤器可帮助您重点关注特定项目或特定类型的数据。 您使用的过滤器类型可以让您深入了解 — 编辑我。
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 1%

---

# 在增强的分析中应用过滤器

“增强的分析”区域中的过滤器可帮助您重点关注特定项目或特定类型的数据。 您使用的过滤器类型可让您分析以下内容：

* 您拥有的项目
* 特定的组合或项目群查看次数
* 特定时间范围（周、季度、会计年度）的关键绩效指标

您可以根据需要添加和删除过滤器，而Adobe Workfront将保留您应用的过滤器，即使您注销也是如此。

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
   <td>业务或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</p> </td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>访问级别*</b> </td> 
   <td> <p>查看项目访问权限</p> <p>您还必须拥有“查看”权限才能访问“任务”、“Portfolio”和“用户”，才能查看特定项目字段过滤器选项。</p> <p>注意：如果在“编辑访问级别”对话框的“设置其他限制”部分中选择了限制，则在应用过滤器后，您可能无法在过滤器或“增强的分析”页面中看到所有信息。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>对象权限</b> </p> </td> 
   <td> <p>查看</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [先决条件](../enhanced-analytics/enhanced-analytics-overview.md#prerequi) in [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 更改日期范围过滤器 {#change-the-date-range-filter}

默认情况下，“增强分析”区域中的可视化图表会显示过去60天和未来15天的数据。 您可以选择新的日期范围，并将其应用于“增强分析”区域中的所有可视化。 如果您从页面导航到其他位置，则会在您下次导航回页面时应用默认日期范围。

>[!TIP]
>
>您还可以使用键盘上的键，从日历小组件导航到、打开并选择日期范围。\
>有关更多信息，请参阅 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 章节 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

要选择新的日期范围，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 单击屏幕右上角的日期范围字段以打开日历视图。
1. 使用日历上方的箭头找到开始日期的月份，然后选择开始日期。

   ![](assets/filters-select-date-range-350x344.png)

1. 使用日历上方的箭头找到结束日期的月份，然后选择结束日期。
1. （可选）要放大较小的日期范围，请将鼠标从一个特定日期拖到其中一个可视化图表上的另一个特定日期。

   屏幕上的所有可视化图表都会更新以匹配所选的时间范围，并且“时间范围”过滤器会显示在任何现有过滤器旁边。 如果您注销或导航到“增强的分析”区域之外，则不会保留此过滤器。

   ![](assets/timeframe-filter-350x220.png)

## 添加筛选器

您可以根据默认项目字段、自定义表单字段和分配给项目的主团队添加过滤器。

>[!TIP]
>
>您还可以使用键盘上的键导航到并添加新过滤器。\
>有关更多信息，请参阅 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 章节 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

* [添加项目字段过滤器](#add-a-project-field-filter)
* [添加项目字段过滤器](#add-a-project-field-filter)
* [添加团队过滤器](#add-a-team-filter)

### 添加项目字段过滤器 {#add-a-project-field-filter}

利用项目字段筛选器，可根据在默认项目包含的字段中输入的值，筛选项目和任务的数据。

以下项目字段过滤器类型可用：

| **项目** | 仅显示选定项目的数据 |
|---|---|
| **项目群** | 仅显示选定项目中项目的数据 |
| **项目组合** | 仅显示选定项目组合中项目的数据 |
| **完成情况** | 仅显示最近满足选定条件（在目标项目上、面临风险或遇到问题）的项目的数据 |
| **状态** | 仅显示最近处于选定状态（完成、当前、暂挂、取消等）的项目的数据 |
| **发起人** | 仅显示具有选定赞助商的项目的数据 |
| **项目所有者** | 仅显示具有选定项目所有者的项目的数据 |

{style="table-layout:auto"}

自定义表单过滤器的工作方式不同。 有关更多信息，请参阅 [添加项目字段过滤器](#add-a-project-field-filter).

要添加项目字段过滤器，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 在屏幕的左上角，单击 **添加过滤器**，然后选择所需的过滤器类型。

   >[!NOTE]
   >
   >不同的过滤器类型显示不同的数据。 一个过滤器中只能使用一种过滤器类型。 选择后，无法在其他项目字段筛选器中使用筛选器类型。

1. 通过在 **搜索** 字段，然后选择要包含在过滤器中的每个值。

   要选择所有当前值，请单击 **全选**.

   ![](assets/select-filter-value-350x251.png)

1. 选择所有所需值后，单击 **应用过滤器**.\
   页面更新右上角的项目计数可反映您应用的过滤器。
1. 对要添加的每个过滤器重复这些步骤。

   添加过滤器时，数据会显示在下面的可视化中，最多50个项目。

   >[!TIP]
   >
   >要查看默认显示的50个以上项目的数据，您可以：
   >
   >   
   >   
   >   * 使用左下角的箭头可显示该可视化图表中接下来的50个项目。\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的排序方式下拉菜单按不同的顺序查看项目。\
      >     ![](assets/sort-by-menu-350x247.png)


   要调整日期范围，请参阅 [更改日期范围过滤器](#change-the-date-range-filter).

### 添加项目自定义表单过滤器

使用“自定义表单”过滤器类型，可以根据在项目的“自定义表单”字段中输入的值过滤项目和任务的数据。 与其他增强型分析过滤器类型不同，您可以添加多个自定义表单过滤器。 每个自定义表单过滤器都包含仅在特定自定义表单的选定字段中输入的值。

添加自定义表单过滤器：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 在屏幕的左上角，单击 **添加过滤器**，然后选择 **自定义表单**.

   ![](assets/select-custom-form-filter-350x271.png)

1. 在 **搜索** 字段，然后选择自定义表单。
1. 选择所需的字段，然后根据要添加到过滤器的字段类型完成以下操作之一：

   >[!NOTE]
   >
   >并非所有自定义表单字段类型都可以添加到过滤器中。 目前，增强型分析仅支持上面列出的字段类型。

   * **复选框**, **下拉列表**&#x200B;或 **单选按钮**:在选定的字段中选择要包含在过滤器中的每个值，或单击 **全选** 复选框。\
      ![](assets/custom-form-filter-checkbox-350x255.png)

   * **日期**:使用箭头导航到特定月份，然后在要包含在过滤器中的选定字段中选择日期。\
      ![](assets/custom-form-filter-date-350x348.png)

   * **文本**:在选定字段中输入要包含在过滤器中的文本。\
      ![](assets/custom-form-filter-text-350x90.png)

   * **数值**:在选定的字段中输入要包含在过滤器中的数字。\
      ![](assets/custom-form-filter-number-350x93.png)

1. 在输入或选择要筛选的值后，单击 **应用过滤器**.

   页面更新右上角的项目计数可反映您应用的过滤器。

1. 对要添加的每个过滤器重复这些步骤。

   添加过滤器时，数据会显示在下面的可视化中，最多50个项目。

   >[!TIP]
   >
   >要查看默认显示的50个以上项目的数据，您可以：
   >
   >   
   >   
   >   * 使用左下角的箭头可显示该可视化图表中接下来的50个项目。\
      >     ![](assets/pagination-350x118.png)
   >   
   >   * 使用可视化图表上的排序方式下拉菜单按不同的顺序查看项目。\
      >     ![](assets/sort-by-menu-350x247.png)


   要调整日期范围，请参阅 [更改日期范围过滤器](#change-the-date-range-filter).

### 添加团队过滤器 {#add-a-team-filter}

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 在左侧面板中，单击 **人员**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. 在屏幕的左上角，单击 **添加过滤器**，然后选择 **团队** 过滤器。
1. 在 **搜索** 字段，然后选择要包含在过滤器中的每个团队。 要选择所有团队，请单击 **全选**.

   ![](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >无论您的访问级别如何，所有团队都将作为过滤器选项包含在内。


1. 选择所有所需的团队后，单击 **应用过滤器**.

   添加过滤器时，数据会显示在下面的可视化中。

   要调整日期范围，请参阅 [更改日期范围过滤器](#change-the-date-range-filter).

## 删除过滤器

您可以随时删除过滤器。 如果删除过滤器，则下次访问增强分析区域时，该过滤器不会显示。

>[!TIP]
>
>您还可以使用键盘上的键导航到并删除现有过滤器。\
>有关更多信息，请参阅 [键盘快捷键](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 章节 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

要删除过滤器，请执行以下操作：

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 如果要删除工作过滤器，请保留在 **工作** 的上界。

   或

   如果要删除人员过滤器，请选择 **人员** 中。

1. 找到所需的过滤器，然后单击 **X** 来删除它。

   ![](assets/remove-filter-350x213.png)

   该过滤器不再处于活动状态，并且除非再次添加，否则不会显示该过滤器。
