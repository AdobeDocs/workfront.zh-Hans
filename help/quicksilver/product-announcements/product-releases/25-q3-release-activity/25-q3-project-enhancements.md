---
title: 2025年第三季度项目增强功能
description: 2025年第三季度项目增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: f02a07c0bc4568d7e0fa25ca6e880024423527b7
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# 2025年第三季度项目增强功能

本页介绍了在2025年第三季度版本中对“预览”环境所做的项目增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第三季度发布周期中此时可用的所有更改列表，请参阅[2025年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 用旧版实际小时数替换了现有实际小时数字段，并创建了新的实际小时数字段

>[!NOTE]
>
> 预览和生产： 2025年6月24日 

我们添加了一个新的实际小时数字段，该字段以小时为单位存储为项目、任务和问题记录的时间，具有小数精度。 字段作为`actualWorkRequiredDouble`存储在Workfront数据库中。

现有实际小时数字段已重命名为旧版实际小时数。 该字段存储项目、任务和问题记录的时间（以分钟为单位），并作为`actualWorkRequired`存储在Workfront数据库中。

实际小时数和旧版实际小时数字段在项目、任务和问题视图和报告中均可见。

项目、任务和问题详细信息部分中显示的实际小时数字段表示新的实际小时数。

>[!IMPORTANT]
>
>根据记录小时数的时间，项目、任务或问题的实际小时数和旧版实际小时数之间可能存在差异。<br>
>&#x200B;>存在以下情况：
>
>* 实际小时数表示自2021年5月以来为项目、任务和问题记录的小时数。
>* 旧版实际小时数表示在项目、任务或问题的生命周期内为项目、任务和问题记录的小时数。 这包括2021年5月之前记录到当前时间的小时数。
>  &#x200B;><br>您可能需要更新报表以反映新字段及其值。
>  &#x200B;><br>Workfront使用旧版实际小时数计算实际劳力成本。

有关信息，请参阅[查看实际小时数](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)。


## 更改API调用实际小时数在数据库中的存储方式

>[!NOTE]
>
>* 预览：下一版API计划于2025年晚些时候发布
>* 生产快速发布：带有下一版API，计划于2025年晚些时候发布
>* 面向所有客户的生产：下一版API计划于2025年晚些时候推出

此更新对项目、任务和问题的实际小时数在数据库中的存储方式进行了更改。 从此更新开始，实际小时数将使用`actualWorkRequiredDouble`的valuefield（值以小时为单位）。

在此更新之前，实际小时数存储在`actualWorkRequired`的valuefield中（其值以分钟为单位）。 此更新将确保在使用API调用计算实际小时数时更准确地计算实际小时数。

由于此更改，您可能需要更新引用原始值字段的任何API调用。 如果您在API调用中使用`actualWorkRequiredExpression`的valuefield，则不应进行任何更改。

此更新不会更改计算自定义字段列中的项目、任务和问题的实际小时数的计算。

## 使用任务或问题标题中的完成百分比滑块在中更新

>[!NOTE]
>
>* 预览： 2025年5月27日
>* 生产快速发布： 2025年5月27日
>* 适用于所有客户的生产： 2025年5月27日

我们更新了完成百分比滑块用于任务和问题的方式。

以下功能现已可用：

* 当您在任务或问题的标题中滑动完成百分比蓝色气泡时，任务或问题的完成百分比现在将以5点增量更新。 在此更新之前，滑动蓝色完成百分比气泡以一点为增量更新任务或问题。

* 您可以双击蓝色气泡，然后手动将其更新为任何所需的数字，而无需使用滑块。 此功能未发生更改。

对于更新Workfront其他区域中任务和问题的完成百分比，没有引入其他更改。

有关信息，请参阅[查看和更新任务的完成百分比](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md)。

## 在项目、任务和问题中使用AI助手时提高透明度

>[!NOTE]
>
>* 预览： 2025年5月19日
>* 生产快速发布： 2025年5月19日
>* 适用于所有客户的生产： 2025年5月19日

为了更清楚地说明AI Assistant如何查找有关Workfront项目、任务和问题的答案，我们在问题响应中添加了此信息。 现在，AI Assistant将其搜索信息包含在输出中。 您可以使用此信息检查AI助手是否正确识别了您提出的问题，并了解答案的上下文。

以前，AI助理的响应中无法获取此信息。

有关使用AI助手获取有关Workfront项的信息，请参阅[使用AI助手处理项目、任务和问题](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)。
