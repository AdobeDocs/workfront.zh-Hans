---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 管理敏捷积压
description: 任务和问题可以分配给敏捷团队，并作为故事添加到该团队的积压工作中，具体取决于团队使用的敏捷方法。
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# 管理敏捷积压

根据团队使用的敏捷方法，可以将以下工作项分配给敏捷团队并将其作为文章添加到该团队的积压工作中：

* **[!UICONTROL 敏捷团队]:** 任务和问题可以分配给敏捷团队并添加到积压工作中。
* **[!UICONTROL 看板敏捷团队]:** 任务可分配给敏捷团队并添加到积压工作中。 用户可以直接从敏捷文章展示板查看积压工作，如 [[!UICONTROL 添加积压] 看板板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). 团队使用此积压工作来排定优先级并管理其工作队列。

可以从中的任意位置将任务或问题分配给团队（并随后添加到团队积压） [!DNL Adobe Workfront]. 例如，可能会从多个项目中为单个团队分配工作分配。

>[!NOTE]
>
>如果向积压项目添加多个团队，则任务或问题仅显示在主团队的积压项目上。 主团队是最先分配的团队。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL管理]对文章所在项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建和管理积压文章

* [重新排序文章](#reorder-stories)
* [[!UICONTROL 中断] 故事](#break-down-stories)
* [编辑文章](#edit-stories)
* [为积压工作创建新文章](#create-new-stories-on-the-backlog)
* [将文章从积压件移至小版本或看板板](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### 重新排序文章 {#reorder-stories}

您可以使用拖放方法对积压工作列表中的文章重新排序。

1. 转到要重新排序文章的敏捷积压工作。
1. 在 **[!UICONTROL 查看]** 下拉菜单中，选择 **[!UICONTROL 积压]** 视图或包含 **[!UICONTROL 订购]** 列。

   >[!NOTE]
   >
   >如果任务或问题分配了敏捷的团队，并且项目的状态不等于“当前”，则它们不会显示在积压工作中。 但是，它们仍会影响“订单”列中的积压计数。

1. 选择一个或多个文章，然后将文章拖到您希望它们在积压工作中显示的顺序。\
   ![拖放积压项目](assets/agile-backlog-drag-and-drop.png)

### 划分文章 {#break-down-stories}

由于积压的文章大小不同，用户可以将它们细分为迭代的可操作大小。 划分文章会在文章表示的任务上创建子任务，并替换积压工作中的原始任务。 您可以将父任务或其子任务分配给敏捷团队，但不能同时将两者分配给团队。

>[!NOTE]
>
>划分文章时请考虑以下限制：
>
>* 只能对表示任务的文章进行划分。 不能对代表问题的故事进行细分。
>* 仅当文章与项目关联时，才能对其进行划分。



要分析故事，请执行以下操作：

1. 转到包含要划分的文章的积压工作。
1. 选择要划分的文章，然后单击 **[!UICONTROL 划分文章]**.\
   的 [!UICONTROL 划分文章] 对话框。\
   ![“划分文章”对话框](assets/backlog-breakdown-dialog.png)

1. 指定文章的名称和估计，然后选择文章是否已准备就绪。
1. 单击 **[!UICONTROL 添加文章]** 从原始故事中再创一个故事。
1. 单击&#x200B;**[!UICONTROL 保存]**。

### 编辑文章 {#edit-stories}

您可以直接从 [!UICONTROL 故事] 或 [!UICONTROL 问题] 与批量编辑项目中的任何任务或问题时使用的选项卡，如 [批量编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md) 和 [编辑问题](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [编辑问题](../../manage-work/issues/manage-issues/edit-issues.md).

## 为积压工作创建新文章 {#create-new-stories-on-the-backlog}

您可以通过直接从积压工作中创建文章，或将现有任务或问题分配给灵活的团队来创建积压工作的新文章。

* [根据积压工作创建文章](#create-a-story-from-the-backlog)
* [将任务或问题分配给敏捷团队](#assign-a-task-or-issue-to-an-agile-team)

### 根据积压工作创建文章 {#create-a-story-from-the-backlog}

在从积压工作中创建文章时，该文章将作为任务或项目中的问题创建。 您不能从积压工作中创建文章作为问题。

要从积压工作中创建文章，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

1. 选择 **[!UICONTROL 积压]** 中。
1. 根据您是要创建任务还是创建问题，执行以下任一操作：

   * **要创建任务，请执行以下操作：** 单击 **[!UICONTROL 故事]**.

   * **要创建问题，请执行以下操作：** 单击 **[!UICONTROL 问题]**.

1. 单击 **[!UICONTROL 新文章]** 或 **[!UICONTROL 新问题]**.

1. 指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL文章名称]</strong></td>
      <td> 键入文章的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>（可选）键入文章的描述。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> 选择文章是否已准备好添加到小版本中。 此设置仅供参考。 无论此设置的状态如何，都可以将文章添加到小版本中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估计]</strong></td>
      <td>为文章指定点数或每小时估计数。 估计值影响燃耗图。 只有在每个文章包含准确估计时，迭代的燃尽图才准确。 （如果提供点估计，则必须已在团队设置中指定每个点表示的小时数。）</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父项目]</strong></td>
      <td>开始键入将在其中创建此文章的项目名称，然后在下拉列表中显示该名称时单击该名称。<br>项目的状态必须设置为[!UICONTROL Current]。 如果项目的状态除[!UICONTROL Current]之外，它不会显示在下拉菜单中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父任务]</strong></td>
      <td>（可选）开始键入此文章所下属的父任务的名称，然后在下拉列表中显示该名称时单击该名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL自定义Forms]</strong></td>
      <td> （可选）选择要添加到此文章的任何自定义表单。</td>
     </tr>
    </tbody>
   </table>

1. 单击 **[!UICONTROL 保存文章]**.

### 将任务或问题分配给敏捷团队 {#assign-a-task-or-issue-to-an-agile-team}

您可以将任务或问题分配给敏捷的团队。 分配任务或问题后，该任务或问题将显示为有关团队积压工作的新文章。

要将任务或问题分配给敏捷团队，请执行以下操作：

1. 转到包含要重新分配的任务的项目。
1. 在列表中选择任务或问题。
1. 单击 **[!UICONTROL 编辑]**.
1. 单击 **[!UICONTROL 分配]**.
1. （可选）删除任何现有的受让人。
1. 单击 **[!UICONTROL 添加被分派人]**.
1. 开始键入要分配给任务或问题的敏捷团队的名称，然后在下拉列表中显示团队名称时单击该名称。
1. 单击 **[!UICONTROL 保存更改]**.\
   任务或问题现在可用于团队积压工作。

## 将文章从积压工作移到迭代或+展示板 {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [将现有文章移至积压文件](#move-existing-stories-to-the-backlog)
* [导出积压文章](#export-stories-from-the-backlog)

1. 去找敏捷团队的积压。
1. 选择要移动到小版本或看板板的文章，然后单击 **[!UICONTROL 更多]** > **[!UICONTROL 移动到]**.\
   如果把故事移到 [!UICONTROL 看板] 展示板， [!UICONTROL 将文章移到看板] 显示展示板。\
   如果将文章移动到迭代，则 [!UICONTROL 将文章移动到迭代] 对话框。\
   ![“移动文章”对话框](assets/agile-backlog-addtoiteration.png)

1. 执行以下任一操作：

   * **对于Scrum团队：** 在 **[!UICONTROL 选择迭代]** 字段中，选择要移动文章的小版本。

   * **对于看板团队：** 在 **[!UICONTROL 选择看板板]** 字段，选择您的团队 [!UICONTROL 看板] 展示板。 (看板团队只能有一个 [!UICONTROL 看板] 展示板。)

1. 单击 **[!UICONTROL 移动文章]**.

### 将现有文章移至积压文件 {#move-existing-stories-to-the-backlog}

如果您决定您的团队尚未准备好处理文章，则可以将文章移至积压工作。

有关更多信息，请参阅 [移动敏捷的故事](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### 导出积压文章 {#export-stories-from-the-backlog}

您可以直接从积压工作中导出一个或多个文章（包括任务和问题）。

导出积压文章的方式与导出 [!DNL Workfront]，如 [导出数据](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
