---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 在增强型分析中查看项目树状图可视化
description: “项目树状图”可视化是在特定时间范围内与其他工作量相比，已在特定时间范围内工作的小时或天数视图。 这有助于您了解用户对项目的投入时间。
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# 在增强型分析中查看项目树状图可视化

“项目树状图”可视化是在特定时间范围内与其他工作量相比，已在特定时间范围内工作的小时或天数视图。 这有助于您了解用户对项目的投入时间。

![](assets/project-treemap-350x126.png)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>业务或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看项目访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解项目树状图可视化图表

项目树状图可视化图表中的框表示项目，而框的大小则显示不同项目花费的时间对比。 框越大，在项目上花费的时间就越多。

项目树状图可视化由以下部分组成：

* **较小的浅蓝色框**:小时或天数较少的项目显示为具有浅蓝色的较小框。

   ![](assets/project-treemap-smaller-box.png)

* **更大的深蓝色框**:具有更多小时或天数的项目，会以深蓝色显示为较大的框。

   ![](assets/project-treemap-larger-box-350x205.png)

* **中型蓝盒**:属于这两个类别的项目显示为中等大小的框，在深蓝色和浅蓝色之间具有蓝色阴影。 中型盒有3种可能的蓝色阴影。

右侧的图例显示每个蓝色阴影的已完成小时数的划分。 此图例是动态的，会根据数据进行更新。

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>如果您按持续时间而不是按计划小时数查看项目树状图可视化图表，此图例将显示每个蓝色阴影的工作天数细目。\
>![](assets/project-treemap-days-worked.png)>

查看此信息可帮助您确定：

* 在选定日期范围内处理的项目的优先级。
* 哪些团队花时间。
* 如果团队关注正确的事情。
* 单击特定项目后，该时间段内项目的范围发生了多少更改。

要了解如何获取此可视化图表的最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看项目树状图可视化

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您需要限制项目数据集，请选择并应用您要使用的过滤器。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. （可选）要更改项目的排序方式，请单击 **排序依据** 菜单，然后选择新的排序选项：

   * **A - Z**
   * **Z - A**
   * **计划的完成日期**
   * **计划的开始日期**

   页面上的所有其他可视化图表将进行更新，以匹配您的排序选择。

1. （视情况而定）如果数据集中有50个以上的项目，请使用可视化左下角的箭头从一组50个项目导航到下一个项目。

   页面上的所有其他可视化图表都会进行更新，以匹配您选择的页面。

   ![](assets/pagination-350x118.png)

1. （可选）将视图从 **计划时间** to **持续时间**.

   默认情况下，会选择计划小时数。

1. 将鼠标悬停在项目上可查看项目条件，以及总计划小时数、总完成小时数以及每天在项目上花费的平均小时数。

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >如果您选择了 **持续时间** 查看，您将看到以下持续时间详细信息：
   >
   >* **计划时间范围**:计划完成项目的天数。
   >* **工作天数**:在顶部选定的日期范围内完成的每项任务的计划持续时间除以一天中的小时数。

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >有关持续时间的更多信息，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

1. （可选）要导出可视化数据，请单击 **导出图标** ![](assets/export.png) 在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**

1. 单击某个项目以打开飞行可视化中的“燃尽”和“任务”，以便更深入地了解任务和小时数（或天数）对项目大小的贡献。

有关“燃耗”可视化图表的详细信息，请参阅 [在Enhanced Analytics中查看燃耗可视化](../enhanced-analytics/burndown-overview.md). 有关“飞行可视化中的任务”的详细信息，请参阅 [在增强分析中查看“飞行”可视化中的任务](../enhanced-analytics/tasks-in-flight-overview.md).

