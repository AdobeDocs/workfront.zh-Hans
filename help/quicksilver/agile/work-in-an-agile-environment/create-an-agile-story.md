---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 创建敏捷故事
description: 您可以通过各种方式在迭代上创建敏捷故事。 创建敏捷故事后，可以向故事添加子任务。
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# 创建敏捷故事

您可以通过各种方式在迭代上创建敏捷故事。 创建敏捷故事后，可以向故事添加子任务。

在迭代中添加故事或子任务时，“持续时间类型”设置为[!UICONTROL 简单]，“任务限制”设置为“固定日期”，且日期锁定在迭代中。 不能修改迭代中的持续时间类型或任务限制。 此外，任务持续时间必须大于0分钟。

有关在将文章添加到开发周期后如何管理文章的信息，请参阅[开发周期](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[！UICONTROL Manage]对文章所在项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 在开发周期中创建敏捷故事

1. 转到要创建故事的敏捷迭代：

   1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 团队]**。

   1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

   1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
   1. 单击要在其中创建文章的特定迭代的名称。

   ![将新故事添加到迭代](assets/iteration-add-story.png)

1. 单击&#x200B;**[!UICONTROL 新建故事]。**
1. 指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL文章名称]</strong></td>
      <td>键入故事的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL描述]</strong></td>
      <td>键入故事的描述。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL就绪]</strong></td>
      <td>如果文章已准备好添加到开发周期，请选择此选项。 选择此选项时，它会向用户指示哪些积压中的文章已准备好添加到开发周期。<br>可以将故事添加到迭代，无论它是否标记为<strong>[！UICONTROL就绪]。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL估计]（点数）</strong></td>
      <td>指定文章的估计值。 如果您的敏捷团队配置为以点为单位估计故事，则默认情况下，1点等于8小时。 预计值将在故事中添加为[！UICONTROL计划小时数]。<br>例如，如果您估计一个故事为3分，则默认行为是向故事添加24个[！UICONTROL计划小时数]。<br>如果文章包含子任务，请记住，所有子任务的组合估计值将决定父文章的估计值。 有关详细信息，请参阅<a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">将故事添加到现有迭代</a>。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父项目]</strong></td>
      <td>开始键入与此故事关联的项目的名称。<br>默认情况下，文章颜色与此项目中的其他文章显示相同的颜色。<br>项目的状态必须设置为[！UICONTROL当前]。 如果项目的状态不是[！UICONTROL当前]，则它不会显示在下拉菜单中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父任务]</strong></td>
      <td>选择父项目后，您可以选择父任务。 选择父任务后，故事将作为选定项目上父任务的子任务创建。<br>开始键入文章父级任务的名称，然后当该任务出现在下拉列表中时，单击它。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL自定义Forms]</strong></td>
      <td>选择要添加到文章中的任何自定义表单。</td>
     </tr>
    </tbody>
   </table>

1. 单击&#x200B;**[!UICONTROL 保存故事]**。

## 在积压中创建敏捷故事

您可以从Agile积压工作中创建Agile故事，如文章[[!UICONTROL 管理] Agile积压](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)中的[在积压工作中创建新故事](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories)部分所述。

## 将任务或问题添加为敏捷故事

您可以将现有任务或问题作为故事添加到开发周期。 有关详细信息，请参阅[将故事添加到现有迭代](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)或[从[!UICONTROL Scrum]展示板](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)添加故事和问题。

## 创建Agile故事的子任务

您可以使用以下任一方法为敏捷故事创建子任务：

* 通过使用&#x200B;**[!UICONTROL 子任务]**&#x200B;选项卡，如[创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md)中的[创建子任务](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks)中所述。

* 直接从故事板创建，如[创建迭代](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)中所述。
