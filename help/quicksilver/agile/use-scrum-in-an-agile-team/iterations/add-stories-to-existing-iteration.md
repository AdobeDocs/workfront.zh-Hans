---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 将文章添加到现有小版本
description: 可以通过多种方式向小版本中添加文章。
author: Courtney
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 3%

---

# 向现有小版本中添加文章

可以通过以下任何一种方式将文章添加到小版本：

* 创建迭代后从积压工作，如[管理敏捷积压工作[!UICONTROL 中的]将文章从积压工作移动到迭代或](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board)看板[展示板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)部分所述

* 从单个任务或问题的[!UICONTROL 详细信息]页面
* 从任务或问题列表中
* 从报表
* 从功能板

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作版或更高版本</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理对文章所在项目的访问权限 </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的详细信息，请参阅[Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 了解添加文章如何影响任务日期

默认情况下，将现有任务添加到小版本时，任务的[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]设置如下：

### 任务[!UICONTROL 计划开始日期]

* 当满足以下条件时，任务将使用小版本的开始日期：

   * 项目未设置[!UICONTROL 计划开始日期]。
   * 项目的[!UICONTROL 计划开始日期]早于&#x200B;*或*&#x200B;早于&#x200B;*迭代的开始日期。*

* 任务在以下情况下使用项目的[!UICONTROL 计划开始日期]:

   * 项目的[!UICONTROL 计划开始日期]在迭代的开始日期&#x200B;*之后*。

### 任务[!UICONTROL 计划完成日期]

* 当满足以下条件时，任务将使用小版本的结束日期：

   * 项目未设置[!UICONTROL 计划完成日期]。
   * 项目的[!UICONTROL 计划开始日期]早于&#x200B;*小版本的开始日期*&#x200B;或项目的[!UICONTROL 计划完成日期]早于&#x200B;*小版本的结束日期*。

* 任务在以下情况下使用项目的[!UICONTROL 计划完成日期]:

   * 项目的[!UICONTROL 计划开始日期]在迭代的开始日期&#x200B;*之后*，项目的[!UICONTROL 计划完成日期]在迭代的结束日期&#x200B;*之后*。

您可以将单个Scrum团队配置为默认使用项目日期，而不是迭代日期。 有关信息，请参阅文章[配置脚本](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)中的[配置在向小版本添加工作项时如何应用日期](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)部分。

## 向现有小版本中添加文章

如果您对项目具有“管理”(Manage)访问权限，则可以将任何任务或问题添加到任何小版本。 将任务或问题移动到小版本时，请牢记以下几点：

* 如果添加多个团队，则任务或问题只能显示在一个团队的小版本上。 这是您在下面步骤3中选择的小版本。
* 如果将任务或问题分配给Agile团队并移到另一个团队的小版本，则团队分配不会发生更改。
* 如果未将任务或问题分配给团队，则将该任务或问题分配给负责小版本的团队。
* 无法将父任务添加到小版本。 如果添加任何子任务，父任务将作为泳道显示在Scrum展示板上。

>[!IMPORTANT]
>
>任务转移到迭代后，无法更新[!UICONTROL 持续时间类型]或[!UICONTROL 任务约束]。 [!UICONTROL 持续时间类型]设置为[!UICONTROL 简单],[!UICONTROL 任务约束]设置为[!UICONTROL 固定日期]，以使任务时间轴与小版本的时间轴保持一致。

1. 打开要添加到小版本的任务或问题。
或
转到包含要添加到小版本的任务或问题的项目、报表或仪表板。 然后，选择一个或多个任务或问题。

1. 单击&#x200B;**[!UICONTROL 更多]** ![更多图标](assets/more-icon.png) > **[!UICONTROL 添加到迭代]**。
不能将任务或问题分配给非敏捷的团队。

1. 在&#x200B;**[!UICONTROL 添加到]**&#x200B;框中，开始键入小版本的名称，并在小版本出现在列表中时选择该小版本。

   >[!NOTE]
   >
   >可以将文章从现有小版本移动到新小版本。

1. 单击&#x200B;**[!UICONTROL 添加]**。
