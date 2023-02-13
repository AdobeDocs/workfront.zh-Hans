---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 将文章添加到现有小版本
description: 您可以通过多种方式将文章添加到小版本中。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 将文章添加到现有小版本

您可以通过以下任一方式将文章添加到小版本：

* 根据创建小版本后的积压工作，如 [将文章从积压工作移到迭代或 [!UICONTROL 看板] 展示板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) 部分 [管理敏捷积压](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* 从 [!UICONTROL 详细信息] 单个任务或问题的页面
* 从任务或问题列表
* 从报表
* 从功能板

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL管理]对文章所在项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 了解添加文章如何影响任务日期

默认情况下，将现有任务添加到小版本时，该任务的 [!UICONTROL 计划开始日期] 和 [!UICONTROL 计划完成日期] 如下所示：

### 任务 [!UICONTROL 计划开始日期]

* 在以下情况下，任务会使用小版本的开始日期：

   * 项目没有 [!UICONTROL 计划开始日期] 设置。
   * 项目的 [!UICONTROL 计划开始日期] is *之前* 或 *on* 迭代的开始日期。

* 任务使用项目的 [!UICONTROL 计划开始日期] 时间：

   * 项目的 [!UICONTROL 计划开始日期] is *after* 迭代的开始日期。

### 任务 [!UICONTROL 计划完成日期]

* 在以下情况下，任务会使用小版本的“结束日期”(End Date):

   * 项目没有 [!UICONTROL 计划完成日期] 设置。
   * 项目的 [!UICONTROL 计划开始日期] is *之前或开* 小版本的开始日期或项目的 [!UICONTROL 计划完成日期] is *之前或开* 小版本的结束日期。

* 任务使用项目的 [!UICONTROL 计划完成日期] 时间：

   * 项目的 [!UICONTROL 计划开始日期] is *after* 小版本的开始日期和项目的 [!UICONTROL 计划完成日期] is *after* 小版本的结束日期。

您可以配置单个Scrum团队以使用默认项目日期，而不是迭代日期。 有关信息，请参阅 [配置在向小版本添加工作项时如何应用日期](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 在文章中 [配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## 将文章添加到现有小版本

要直接从任务或问题向小版本添加文章，请执行以下操作：

>[!IMPORTANT]
>
>任务移至小版本后，您无法更新 [!UICONTROL 持续时间类型] 或 [!UICONTROL 任务约束]. [!UICONTROL 持续时间类型] 设置为 [!UICONTROL 简单] 和 [!UICONTROL 任务约束] 设置为 [!UICONTROL 固定日期] 使任务时间线与小版本的时间线一致。

### 从“任务”或“问题”选项卡中

如果您对项目具有“管理”(Manage)访问权限，则可以向任何小版本添加任何任务或问题。 在将任务或问题移动到小版本时，请牢记以下几点：

* 如果添加多个团队，则任务或问题只能在一个团队的小版本中显示。 这是您在下面步骤3中选择的小版本。
* 如果任务或问题被分配给敏捷团队并移至另一个团队的小版本，则团队分配不会更改。
* 如果任务或问题未分配给团队，则任务或问题将分配给小版本的所有者团队。
* 无法将父任务添加到小版本。 如果添加任何子任务，则父任务将在Scrum展示板中显示为一个泳道。

1. 转到包含要添加到小版本的任务或问题的项目、报表或功能板。
1. 选择一个或多个任务或问题。
1. 单击 **[!UICONTROL 更多]** ![](assets/more-icon.png) > **[!UICONTROL 添加到迭代]**.\
   您不能分配分配给非敏捷团队的任务或问题。

1. 在 **[!UICONTROL 添加文章]** 框中，键入小版本的名称。

   >[!NOTE]
   >
   >可以将文章从现有小版本移动到新小版本。

1. 如果要添加任务，请单击 **[!UICONTROL 添加文章]**.\
   或\
   如果添加问题，请单击 **[!UICONTROL 添加问题]**.
