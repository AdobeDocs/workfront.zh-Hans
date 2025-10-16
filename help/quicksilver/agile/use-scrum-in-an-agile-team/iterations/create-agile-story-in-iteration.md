---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 在开发周期中创建敏捷故事
description: 本文介绍了如何在迭代中创建新敏捷故事。
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 在开发周期中创建敏捷故事

本文介绍了如何在迭代中创建新敏捷故事。 有关从任务、问题或[!DNL Adobe Workfront]的其他区域创建Agile故事的信息，请参阅[将故事添加到现有迭代](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
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

## 在开发周期中创建敏捷故事

1. 转到要创建故事的敏捷迭代：

   {{step1-to-team}}

   1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

   1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**。
   1. 单击要在其中创建文章的特定迭代的名称。
   1. 在左侧面板中，选择&#x200B;**[!UICONTROL 故事]**。

1.  单击&#x200B;**[!UICONTROL 新建故事]**。
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
      <td>指定文章的估计值。 如果您的敏捷团队配置为以点为单位估计故事，则默认情况下，1点等于8小时。 预计值将在故事中添加为[！UICONTROL计划小时数]。<br>例如，如果您估计一个故事为3分，则默认行为是向故事添加24个计划小时数。<br>如果文章包含子任务，请记住，所有子任务的组合估计值将决定父文章的估计值。 有关详细信息，请参阅<a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">将子任务添加到[！UICONTROL Scrum]展示板上的现有文章</a>。</td>
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
