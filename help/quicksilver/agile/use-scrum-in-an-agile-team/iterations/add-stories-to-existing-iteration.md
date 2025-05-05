---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 将故事添加到现有迭代
description: 您可以通过多种方式将故事添加到开发周期。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 91dc9946566e15bf32d0d89975e3e6b66b39e873
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# 将故事添加到现有迭代

您可以通过以下任意方式将故事添加到开发周期：

* 创建迭代后的积压工作，如[管理Agile积压工作](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)中的[将故事从积压工作移动到迭代[!UICONTROL Kanban]展示板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board)部分所述

* 从单个任务或问题的[!UICONTROL 详细信息]页面
* 从任务或问题列表
* 从报表
* 从功能板

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [!UICONTROL Standard]</p> 
   或
   <p>当前： [!UICONTROL Work]或更高版本</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[!UICONTROL Manage]对文章所在项目的访问权限 </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 了解添加故事如何影响任务日期

默认情况下，将现有任务添加到开发周期时，该任务的[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]设置如下：

### 任务[!UICONTROL 计划开始日期]

* 在以下情况下，任务使用迭代的开始日期：

   * 项目未设置[!UICONTROL 计划开始日期]。
   * 项目的[!UICONTROL 计划开始日期]为&#x200B;*早于*&#x200B;或&#x200B;*于*&#x200B;迭代的开始日期。

* 任务在以下情况下使用项目的[!UICONTROL 计划开始日期]：

   * 项目的[!UICONTROL 计划开始日期]晚于&#x200B;*迭代的开始日期*。

### 任务[!UICONTROL 计划完成日期]

* 在以下情况下，任务使用迭代的结束日期：

   * 项目未设置[!UICONTROL 计划完成日期]。
   * 项目的[!UICONTROL 计划开始日期]早于&#x200B;*或晚于*&#x200B;迭代的开始日期，或项目的[!UICONTROL 计划完成日期]早于&#x200B;*或晚于*&#x200B;迭代的结束日期。

* 任务在以下情况下使用项目的[!UICONTROL 计划完成日期]：

   * 项目的[!UICONTROL 计划开始日期]晚于&#x200B;*迭代的开始日期，项目的[!UICONTROL 计划完成日期]晚于*&#x200B;迭代的结束日期。**

您可以将单个Scrum团队配置为默认使用项目日期，而不是迭代日期。 有关信息，请参阅[配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[配置将工作项添加到迭代时应用日期的方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)部分。

## 将故事添加到现有迭代

如果您拥有项目的“管理”访问权限，则可以向任何开发周期添加任何任务或问题。 将任务或问题移动到开发周期时，请牢记以下几点：

* 如果添加多个团队，则任务或问题只能显示在一个团队的迭代中。 这是您在下面的步骤3中选择的小版本。
* 如果任务或问题被分配给Agile团队并移动到其他团队的迭代，则团队分配不会更改。
* 如果任务或问题未分配给团队，则任务或问题将分配给拥有开发周期的团队。
* 您无法将父任务添加到开发周期。 如果添加任何子任务，父任务将作为泳道显示在Scrum展示板上。

>[!IMPORTANT]
>
>任务移至迭代后，无法更新[!UICONTROL 持续时间类型]或[!UICONTROL 任务约束]。 [!UICONTROL 持续时间类型]设置为[!UICONTROL 简单]，[!UICONTROL 任务限制]设置为[!UICONTROL 固定日期]，以使任务时间表与迭代的时间表保持一致。

1. 打开要添加到开发周期的任务或问题。
或
转到项目、报告或仪表板，其中包含要添加到开发周期的任务或问题。 然后选择一个或多个任务或问题。

1. 单击&#x200B;**[!UICONTROL 更多]** ![更多图标](assets/more-icon.png) > **[!UICONTROL 添加到迭代]**。
您无法将任务或问题分配给非敏捷团队。

1. 在&#x200B;**[!UICONTROL 添加到]**&#x200B;框中，开始键入迭代的名称，并在该迭代出现在列表中时将其选定。

   >[!NOTE]
   >
   >您可以将故事从现有小版本移动到新小版本。

1. 单击&#x200B;**[!UICONTROL 添加]**。
