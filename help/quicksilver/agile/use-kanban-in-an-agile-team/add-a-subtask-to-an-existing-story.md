---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 将子任务添加到Kanban展示板上的现有故事
description: 阅读本文，了解如何为Kanban展示板上的现有故事创建子任务。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 将子任务添加到Kanban展示板上的现有故事

在为现有文章创建子任务时，请牢记以下事项：

**当项目的[!UICONTROL 摘要完成模式]设置设置为[!UICONTROL 手动]：**&#x200B;时

* 您可以将包含子任务的父故事移动到[!UICONTROL 完成]，这样会将父故事更新为100%，并将[!UICONTROL 状态]更新为[!UICONTROL 完成]。 子任务未更新。
* 若要更新文章的[!UICONTROL 完成百分比]，必须从[!UICONTROL 故事]选项卡或对象的[!UICONTROL 详细信息]页面对其进行更新。

**当项目的[!UICONTROL 摘要完成模式]设置设置为[!UICONTROL 自动]：**&#x200B;时

* 无法跨版移动父故事。 要更新故事的[!UICONTROL 完成百分比]，您必须更新任何子任务的[!UICONTROL 完成百分比]。 故事的[!UICONTROL 完成百分比]是根据所有子任务的[!UICONTROL 完成百分比]计算的。
* 将包含子任务的父故事移动到[!UICONTROL 完成]会将父故事更新为100%，将[!UICONTROL 状态]更新为[!UICONTROL 完成]。 子任务也更新为100%，[!UICONTROL 状态]更新为[!UICONTROL 完成]。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p> 
   或
   <p>当前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[！UICONTROL Contribute]或[！UICONTROL Manage]对子任务所在任务的访问权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将子任务添加到[!UICONTROL Kanban]展示板上的现有故事中

1. 转到包含要添加子任务的故事的[!UICONTROL Kanban]展示板。
1. 单击[!UICONTROL Kanban]展示板上故事拼贴上任务的名称。
1. 将子任务添加到该任务中，就像在[!DNL Workfront]内的任何其他任务列表中一样，如[创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md)中所述。
