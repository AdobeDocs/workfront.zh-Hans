---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 将故事添加到现有迭代
description: 您可以通过多种方式将故事添加到开发周期。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# 将故事添加到现有迭代

您可以通过以下任意方式将故事添加到开发周期：

* 创建迭代后的积压工作，如[管理Agile积压工作](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)中的[将故事从积压工作移动到迭代[!UICONTROL Kanban]展示板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog)部分所述

* 从单个任务或问题的[!UICONTROL 详细信息]页面
* 从任务或问题列表
* 从报表
* 从功能板

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Manage]对文章所在项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

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

您可以将单个Scrum团队配置为默认使用项目日期，而不是迭代日期。 有关信息，请参阅[配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[配置将工作项添加到迭代时应用日期的方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)部分。

## 将故事添加到现有迭代

要直接从任务或问题将故事添加到开发周期，请执行以下操作：

>[!IMPORTANT]
>
>任务移至迭代后，无法更新[!UICONTROL 持续时间类型]或[!UICONTROL 任务约束]。 [!UICONTROL 持续时间类型]设置为[!UICONTROL 简单]，[!UICONTROL 任务限制]设置为[!UICONTROL 固定日期]，以使任务时间表与迭代的时间表保持一致。

### 从任务或问题选项卡

如果您拥有项目的“管理”访问权限，则可以向任何开发周期添加任何任务或问题。 将任务或问题移动到开发周期时，请牢记以下几点：

* 如果添加多个团队，则任务或问题只能显示在一个团队的迭代中。 这是您在下面的步骤3中选择的小版本。
* 如果任务或问题被分配给Agile团队并移动到其他团队的迭代，则团队分配不会更改。
* 如果任务或问题未分配给团队，则任务或问题将分配给拥有开发周期的团队。
* 您无法将父任务添加到开发周期。 如果添加任何子任务，父任务将作为泳道显示在Scrum展示板上。

1. 转到项目、报告或仪表板，其中包含要添加到开发周期的任务或问题。
1. 选择一个或多个任务或问题。
1. 单击&#x200B;**[!UICONTROL 更多]** ![](assets/more-icon.png) > **[!UICONTROL 添加到迭代]**。\
   您无法将任务或问题分配给非敏捷团队。

1. 在&#x200B;**[!UICONTROL 添加故事]**&#x200B;框中，键入迭代的名称。

   >[!NOTE]
   >
   >您可以将故事从现有小版本移动到新小版本。

1. 如果要添加任务，请单击&#x200B;**[!UICONTROL 添加故事]**。\
   或\
   如果要添加问题，请单击&#x200B;**[!UICONTROL 添加问题]**。
