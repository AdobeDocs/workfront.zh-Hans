---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 将子任务添加到看板板上的现有文章
description: 查看本文，了解如何在看板板上为现有文章创建子任务。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 将子任务添加到看板板上的现有文章

在为现有文章创建子任务时，请记住以下事项：

**当 [!UICONTROL 摘要完成模式] 项目的设置设置为 [!UICONTROL 手动]:**

* 您可以将包含子任务的父文章移动到 [!UICONTROL 完成]，这会将父文章更新为100%, [!UICONTROL 状态] to [!UICONTROL 完成]. 子任务未更新。
* 要更新 [!UICONTROL 完成百分比] 对于故事，必须从 [!UICONTROL 故事] 选项卡或 [!UICONTROL 详细信息] 对象的页面。

**当 [!UICONTROL 摘要完成模式] 项目的设置设置为 [!UICONTROL 自动]:**

* 你不能把父文章全面搬走。 要更新 [!UICONTROL 完成百分比] 对于故事，您必须更新 [!UICONTROL 完成百分比] 子任务。 的 [!UICONTROL 完成百分比] ，根据 [!UICONTROL 完成百分比] 所有子任务的子任务。
* 将包含子任务的父文章移动到 [!UICONTROL 完成] 将父文章更新为100%, [!UICONTROL 状态] to [!UICONTROL 完成]. 子任务也会更新为100%，并且 [!UICONTROL 状态] 已更新为 [!UICONTROL 完成].

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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL Contribute]或[!UICONTROL Manage]对子任务所在任务的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 将子任务添加到 [!UICONTROL 看板] 展示板

1. 转到 [!UICONTROL 看板] 包含要添加子任务的文章的展示板。
1. 单击 [!UICONTROL 看板] 展示板。
1. 向任务中添加子任务，就像在 [!DNL Workfront]，如 [创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md).
