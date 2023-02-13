---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum展示板上的现有文章中添加子任务
description: 在为现有文章创建子任务时，请记住项目的“完成模式”设置，因为这会影响文章的更新方式。
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 将子任务添加到 [!UICONTROL Scrum] 展示板

在为现有文章创建子任务时，请记住以下事项：

**当 [!UICONTROL 完成模式] 项目的设置设置为 [!UICONTROL 手动]:**

* 将包含子任务的父文章移动到 [!UICONTROL 完成] 将父文章更新为100%, [!UICONTROL 状态] to [!UICONTROL 完成]. 子任务未更新。
* 要更新 [!UICONTROL 完成百分比] 对于故事，必须从 [!UICONTROL 故事] 选项卡或 [!UICONTROL 详细信息] 对象的页面。

**当 [!UICONTROL 完成模式] 项目的设置设置为 [!UICONTROL 自动]**:

* 将包含子任务的父文章移动到 [!UICONTROL 完成] 将父文章更新为100%, [!UICONTROL 状态] to [!UICONTROL 完成]. 子任务也会更新为100%，并且 [!UICONTROL 状态] 已更新为 [!UICONTROL 完成].
* 要更新 [!UICONTROL 完成百分比] 对于故事，您必须更新 [!UICONTROL 完成百分比] 子任务。 的 [!UICONTROL 完成百分比] ，根据 [!UICONTROL 完成百分比] 所有子任务的子任务。

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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL Contribute]或[!UICONTROL Manage]对子任务所在任务的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 在Scrum展示板上的现有文章中添加子任务

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

1. 转到包含要添加子任务的文章的敏捷小版本或项目。 有关如何导航到小版本的信息，请参阅 [查看小版本](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. 转到要添加子任务的文章展示板上的文章拼贴。
1. 单击 **[!UICONTROL 添加子任务]** 在主文章卡片上创建文章的子任务。

   ![添加子任务](assets/agile-story-addsubtask-NWE.png)

   或

   单击 **[!UICONTROL 添加子任务]** 在子任务拼贴上创建子任务。

   [!DNL Workfront] 支持无限级别的子任务，但敏捷文章展示板上只显示两个级别（子任务的子任务）。

   ![添加子任务](assets/agile-story-addsubtask2-NWE.png)

   向当前没有游泳道的文章添加子任务时，父任务将提升到 [!UICONTROL 父文章] 子任务在泳道内移动。

1. 指定以下信息：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL子任务名称]</strong></td>
      <td> 指定子任务的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>为子任务指定描述。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估计]</strong></td>
      <td>指定子任务的估计值。<br><p>在创建估计时，请牢记以下几点：</p>
       <ul>
        <li>如果您的敏捷团队配置为以点为单位估计文章，则默认情况下1点等于8小时。 估计值在文章中添加为[!UICONTROL计划时数]。</li>
        <li>所有子任务的组合估计确定父文章的估计。 有关更多信息，请参阅 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">更新Scrum展示板上的文章和子任务的状态</a>.</li>
        <li>创建新子任务时，已设置[!UICONTROL估计]字段。 如果重置子任务的估计值，则将重置父文章的估计值（因为父文章是其所有子任务的总和）。</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL计划时数]</strong></td>
      <td> （仅在项目中可用）指定任务的计划小时数。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL分配]</strong></td>
      <td>开始键入要分配子任务的团队名称，然后在下拉列表中显示时单击该名称。</td>
     </tr>
    </tbody>
   </table>

1. 单击&#x200B;**[!UICONTROL 创建]**。
