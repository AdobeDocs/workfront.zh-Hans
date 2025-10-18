---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 管理Agile积压
description: 任务和问题可分配给Agile团队，并作为故事添加到该团队的积压中，具体取决于团队使用的敏捷方法。
author: Jenny
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 0%

---

# 管理Agile积压

以下工作项可以分配给Agile团队，并作为故事添加到该团队的积压中，具体取决于团队使用的敏捷方法：

* **[!UICONTROL Scrum Agile团队]：**&#x200B;任务和问题可以分配给Agile团队并添加到积压中。
* **[!UICONTROL Kanban Agile团队]：**&#x200B;任务可以分配给Agile团队并添加到积压中。 用户可以直接从Agile故事板查看积压，如[[!UICONTROL 将积压]添加到Kanban板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)中所述。 团队使用此积压事项来排列工作队列的优先顺序并管理其工作队列。

任务或问题可以从[!DNL Adobe Workfront]中的任何位置分配给团队（并随后添加到团队积压）。 例如，一个团队可能从多个项目中分配了工作分派。

>[!NOTE]
>
>如果将多个团队添加到积压项目，则任务或问题仅显示在主要团队的积压中。 主要团队是首先分配的团队。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作或更高</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理对文章所在项目的访问权限 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建和管理积压中的故事

* [重新排序故事](#reorder-stories)
* [[!UICONTROL 划分]个故事](#break-down-stories)
* [编辑故事](#edit-stories)

### 重新排序故事 {#reorder-stories}

您可以使用拖放方法重新排序积压事项列表中的故事。

1. 转到要重新排序故事的Agile积压。
1. 在&#x200B;**[!UICONTROL 视图]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 积压]**&#x200B;视图或包含&#x200B;**[!UICONTROL 顺序]**&#x200B;列的自定义视图。

   >[!NOTE]
   >
   >如果任务或问题分配了Agile团队，且项目未处于与当前相同的状态，则它们不会显示在积压中。 但是，它们仍会影响“顺序”列中的积压计数。

1. 选择一个或多个故事，然后将故事拖到您希望它们在积压中显示的顺序上。
   ![拖放积压工作项](assets/agile-backlog-drag-and-drop.png)

### 分解故事 {#break-down-stories}

由于积压中的故事大小不同，因此用户可以将其细分为开发周期的有效大小。 分解故事会在故事所代表的任务上创建子任务，并替换积压中的原始任务。 您可以将父任务或其子任务分配给Agile团队，但不能将两者同时分配给团队。

>[!NOTE]
>
>在划分故事时，请考虑以下限制：
>
>* 只有代表任务的故事才能细分。 您无法细分代表问题的故事。
>* 只有当故事与项目相关联时，才能对其进行划分。


要分解故事，请执行以下操作：

1. 转到包含要细分的故事的积压。
1. 选择要分解的故事，然后单击&#x200B;**[!UICONTROL 分解故事]**。
显示[!UICONTROL 划分故事]对话框。
   ![分解故事对话框](assets/backlog-breakdown-dialog.png)

1. 指定文章的名称和估计值，然后选择文章是否已准备就绪。
1. 单击&#x200B;**[!UICONTROL 添加故事]**&#x200B;以从原始故事创建另一个故事。
1. 单击&#x200B;**[!UICONTROL 保存]**。

### 编辑故事 {#edit-stories}

可以直接从积压中的[!UICONTROL 故事]或[!UICONTROL 问题]选项卡编辑故事，就像要批量编辑项目中的任何任务或问题一样，如[编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk)中的[批量编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md)和[编辑问题](../../manage-work/issues/manage-issues/edit-issues.md)中所述。

## 在积压工作中创建新故事 {#create-new-stories-on-the-backlog}

通过直接从积压创建故事，或将现有任务或问题分配给Agile团队，可以在积压中创建新故事。

* [从积压创建故事](#create-a-story-from-the-backlog)
* [将任务或问题分配给Agile团队](#assign-a-task-or-issue-to-an-agile-team)

### 从积压创建故事 {#create-a-story-from-the-backlog}

从积压创建故事时，故事将作为项目中的任务或问题创建。

要从积压创建故事，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 团队]**。

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择一个新的Scrum团队，或者在搜索栏中搜索一个团队并在它出现时将其选定。

1. 从左侧面板中选择&#x200B;**[!UICONTROL 积压工作]**。
1. 执行以下操作之一，具体取决于您是要创建任务还是创建问题：

   * **要创建任务：**&#x200B;请单击&#x200B;**[!UICONTROL 故事]**。

   * **要创建问题：**，请单击&#x200B;**[!UICONTROL 问题]**。

1. 单击&#x200B;**[!UICONTROL 新建故事]**&#x200B;或&#x200B;**[!UICONTROL 新建问题]**。

1. 指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 文章名称]</strong></td>
      <td> 键入故事的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 描述]</strong></td>
      <td>（可选）键入文章的描述。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 就绪]</strong></td>
      <td> 选择文章是否准备好添加到开发周期。 此设置仅供参考。 可以将故事添加到开发周期，而不管此设置的状态如何。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 估计]</strong></td>
      <td>指定文章的分值或每小时估计值。 估计值会影响燃尽图。 仅当每个故事都包含准确的估计值时，迭代的燃尽图才准确。 （如果提供点估计值，则必须在团队设置中指定每个点表示的小时数。）</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 父项目]</strong></td>
      <td>开始键入将在其中创建此文章的项目名称，然后在名称出现在下拉列表中时单击该名称。<br>项目的状态必须设置为[!UICONTROL 当前]。 如果项目的状态不是[!UICONTROL 当前]，则它不会显示在下拉菜单中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 父任务]</strong></td>
      <td>（可选）开始键入此文章从属的父任务的名称，然后在名称出现在下拉列表中时单击该名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 自定义Forms]</strong></td>
      <td> （可选）选择要添加到此文章的任何自定义表单。</td>
     </tr>
    </tbody>
   </table>

1. 单击&#x200B;**[!UICONTROL 保存故事]**。

### 将任务或问题分配给Agile团队 {#assign-a-task-or-issue-to-an-agile-team}

您可以将任务或问题分配给Agile团队。 分配任务或问题后，该任务或问题会在团队积压中显示为新故事。

要向Agile团队分配任务或问题，请执行以下操作：

1. 转到包含要分配的任务的项目。
1. 在列表中选择任务或问题。
1. 单击&#x200B;**[!UICONTROL 编辑]**。
1. 单击&#x200B;**[!UICONTROL 分配]**。
1. （可选）删除任何现有的被分配人。
1. 单击&#x200B;**[!UICONTROL 添加代理人]**。
1. 开始键入要分配给任务或问题的Agile团队名称，然后单击出现在下拉列表中的团队名称。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。
任务或问题现在可在团队积压中找到。

## 将故事移入或移出积压

* [将故事从积压工作移动到迭代或展示板](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [将现有故事移至积压](#move-existing-stories-to-the-backlog)
* [从积压中导出故事](#export-stories-from-the-backlog)

### 将故事从积压工作移动到迭代或展示板

1. 转到Agile团队的积压。
1. 选择要移动到开发周期或Kanban展示板的故事，然后单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 移动到]**。
如果将故事移动到[!UICONTROL Kanban]展示板，则会显示[!UICONTROL 将故事移动到Kanban]展示板。
如果将文章移动到迭代，则显示[!UICONTROL 将文章移动到迭代]对话框。
   ![移动故事对话框](assets/agile-backlog-addtoiteration.png)

1. 执行以下任一操作：

   * **对于Scrum团队：**&#x200B;在&#x200B;**[!UICONTROL 选择迭代]**&#x200B;字段中，选择要移动故事的迭代。

   * **对于Kanban团队：**&#x200B;在&#x200B;**[!UICONTROL 选择Kanban展示板]**&#x200B;字段中，选择您的团队[!UICONTROL Kanban]展示板。 （Kanban团队只能有一个[!UICONTROL Kanban]展示板。）

1. 单击&#x200B;**[!UICONTROL 移动故事]**。

### 将现有故事移至积压 {#move-existing-stories-to-the-backlog}

如果您确定您的团队尚未准备好处理故事，您可以将故事移至积压。

有关详细信息，请参阅[移动敏捷故事](../../agile/work-in-an-agile-environment/move-an-agile-story.md)。

### 从积压中导出故事 {#export-stories-from-the-backlog}

您可以直接从积压中导出一个或多个故事（包括任务和问题）。

从积压中导出故事的方式与在[!DNL Workfront]中导出其他数据的方式相同，如[导出数据](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)中所述。
