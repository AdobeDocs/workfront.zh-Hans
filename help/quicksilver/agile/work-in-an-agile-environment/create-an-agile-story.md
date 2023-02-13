---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 创建敏捷的故事
description: 您可以通过各种方式在迭代中创建敏捷故事。 创建敏捷文章后，可向文章添加子任务。
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 创建敏捷的故事

您可以通过各种方式在迭代中创建敏捷故事。 创建敏捷文章后，可向文章添加子任务。

在小版本中添加文章或子任务时，持续时间类型将设置为 [!UICONTROL 简单] 任务约束设置为固定日期，并且日期在小版本中锁定。 您不能在小版本中修改持续时间类型或任务约束。 此外，任务持续时间必须大于0分钟。

有关如何在将文章添加到小版本后管理文章的信息，请参阅 [迭代](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

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

## 在迭代中创建敏捷故事

1. 转到要创建文章的敏捷迭代：

   1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

   1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

   1. 在左侧面板中，选择 **[!UICONTROL 迭代]** 选择特定小版本，或选择 **[!UICONTROL 当前迭代]**.
   1. 单击要在其中创建文章的特定小版本的名称。

   ![向迭代中添加新文章](assets/iteration-add-story.png)

1. 单击 **[!UICONTROL 新文章].**
1. 指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL文章名称]</strong></td>
      <td>键入文章的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>键入文章的描述。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>如果文章已准备好添加到小版本，请选择此选项。 选择此选项后，它会向用户指示哪些积压工作中的文章已准备好添加到小版本中。<br>无论文章是否标记，都可以将其添加到小版本中 <strong>[!UICONTROL Ready]。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估计]（点）</strong></td>
      <td>指定文章的估计值。 如果您的敏捷团队配置为以点为单位估计文章，则默认情况下1点等于8小时。 估计值在文章中添加为[!UICONTROL计划时数]。<br>例如，如果您将文章估计为3分，则默认行为是向文章添加24 [!UICONTROL计划时数]。<br>如果文章包含子任务，请记住，所有子任务的组合估计决定了父文章的估计。 有关更多信息，请参阅 <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">将文章添加到现有小版本</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父项目]</strong></td>
      <td>开始键入将与此文章关联的项目的名称。<br>默认情况下，文章颜色显示为与此项目中其他文章相同的颜色。<br>项目的状态必须设置为[!UICONTROL Current]。 如果项目的状态除[!UICONTROL Current]之外，它不会显示在下拉菜单中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父任务]</strong></td>
      <td>选择父项目后，您可以选择父任务。 选择父任务时，文章将作为所选项目上父任务的子任务创建。<br>开始为文章键入父任务的名称，然后在下拉列表中显示该名称时单击该名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL自定义Forms]</strong></td>
      <td>选择要添加到文章的任何自定义表单。</td>
     </tr>
    </tbody>
   </table>

1. 单击 **[!UICONTROL 保存文章]**.

## 在积压工作中创建敏捷故事

您可以根据敏捷积压工作创建敏捷故事，如一节中所述 [为积压工作创建新文章](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) 在文章中 [[!UICONTROL 管理] 敏捷的积压工作](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## 将任务或问题添加为敏捷故事

您可以将现有任务或问题作为文章添加到小版本中。 有关更多信息，请参阅 [将文章添加到现有小版本](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) 或 [添加 [!UICONTROL Scrum] 展示板](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 创建敏捷故事的子任务

您可以使用以下任一方法创建敏捷文章的子任务：

* 通过使用 **[!UICONTROL 子任务]** 选项卡，如 [创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md).

* 直接从文章展示板，如 [创建迭代](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
