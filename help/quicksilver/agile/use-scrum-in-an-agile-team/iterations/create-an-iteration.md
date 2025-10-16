---
product-area: agile-and-teams
navigation-topic: iterations
title: 创建迭代
description: 迭代是Scrum敏捷团队规划工作容量的关键组件。 [!DNL Adobe Workfront] 允许Scrum敏捷团队通过创建多个迭代以适应团队需求来管理其工作。
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 创建迭代

迭代是Scrum敏捷团队规划工作容量的关键组件。 [!DNL Adobe Workfront]允许Scrum敏捷团队通过创建多个迭代以适应团队需求来管理其工作。

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
   <td> <p>浅色或更高</p> 
   <p>审核或更高</p> </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 添加迭代

可在列表中添加开发周期以快速创建开发周期，并稍后向其添加任务和问题。

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

1. 在&#x200B;**[!UICONTROL 迭代]**&#x200B;选项卡上，单击&#x200B;**[!UICONTROL 添加迭代]**。

   ![单击“添加迭代”](assets/click-add-iteration.png)

1. 指定以下内容：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL迭代名称]</strong></td> 
      <td>输入迭代的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL目标]</strong></td> 
      <td>添加任何迭代目标。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL开始日期]</strong></td> 
      <td>输入迭代应开始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL结束日期]</strong></td> 
      <td><p>输入迭代应结束的日期。 [!DNL Workfront]建议设置的结束日期从开始日期起不超过4周。</p><p>提示：请确保选择工作日作为结束日期。 燃尽图的计算只使用工作日。<br>默认情况下，燃尽图使用默认时间表来定义工作日（如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建时间表</a>中所述）。 或者，为了合并团队特定的非工作日，Agile团队可以选择使用替代计划（如<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建一个Agile团队</a>中的“为燃尽图定义替代团队计划”中所述）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL容量]</strong></td> 
      <td> 指定迭代的容量。 这是您的团队在迭代中能够完成的点数或小时数。 您输入的数字必须等于或大于迭代中所有故事的总和中的点数或小时数。默认情况下，<br>[!DNL Workfront]使用50个容量预填充此字段。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL焦点]</strong></td> 
      <td>指定团队的焦点百分比。 如果团队的所有成员都将完全专注于此迭代，则焦点将为100%。默认情况下，<br>[!DNL Workfront]会使用100%预填充此字段。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 添加迭代]**。 现在您已创建迭代，需要添加故事。 有关详细信息，请参阅[将故事添加到现有迭代](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)。

## 在[!UICONTROL 积压]选项卡上规划迭代

使用[!UICONTROL 计划迭代]功能，使用积压中的任务创建迭代。

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

1. 在左侧面板上选择&#x200B;**[!UICONTROL 积压]**。

1. 在&#x200B;**故事**&#x200B;或&#x200B;**问题**&#x200B;选项卡上，选择要添加到开发周期的工作项，然后单击&#x200B;**[!UICONTROL 计划开发周期]**。

>[!NOTE]
>
> 在“积压”选项卡上规划迭代时，无法在“故事”或“问题”选项卡之间切换或添加其他任务。 创建开发周期后，您可以添加现有故事或问题。 有关详细信息，请参阅下面的“积压”选项卡[上的](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab)将任务或问题添加到现有迭代。


1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL迭代名称]</strong></td> 
      <td>指定迭代的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL开始日期]</strong></td> 
      <td> 指定迭代应开始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL结束日期]</strong> </td> 
      <td><p>指定迭代应结束的日期。 [!DNL Workfront]建议设置的结束日期从开始日期起不超过4周。</p><p>提示：请确保选择工作日作为结束日期。 燃尽图的计算只使用工作日。<br>默认情况下，燃尽图使用默认时间表来定义工作日（如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建时间表</a>中所述）。 或者，要合并团队特定的非工作日，Agile团队可以选择使用替代计划（如<a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">为燃尽图使用替代团队计划</a>中所述）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL焦点]</strong></td> 
      <td>指定团队的焦点百分比。 如果团队的所有成员都将完全专注于此迭代，则焦点将为100%。<br>[!DNL Workfront]会使用您团队过去迭代的平均值预填充此字段。 如果这是您团队的第一个迭代，则默认情况下，此字段值为0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[！UICONTROL容量]</strong></td> 
      <td> 指定迭代的容量。 这是您的团队在迭代中能够完成的点数或小时数。 您输入的数字必须等于或大于迭代中所有故事的总和中的点数或小时数。<br>[!DNL Workfront]会使用您团队过去迭代的平均值预填充此字段。 如果这是您团队的第一个迭代，则默认情况下，此字段值为0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[！UICONTROL目标]</strong></td> 
      <td> 指定迭代的目标。 此字段不是必填字段。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]。**&#x200B;已创建迭代。

## 将任务或问题添加到积压工作选项卡上的现有迭代

1. 在&#x200B;**积压**&#x200B;选项卡中，单击&#x200B;**故事**&#x200B;或&#x200B;**问题**&#x200B;选项卡。

1. 选择要添加到开发周期的故事或问题。 积压工作顶部的故事优先级别更高。

   ![移动工作项](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  将任务添加到迭代时，任务的开始日期将按照[[!UICONTROL 了解]中所述计算任务开始日期的方式添加到迭代](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration)中。


## 了解将任务添加到开发周期后如何计算任务开始日期 {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

将任务作为故事添加到迭代时，每个故事都使用[!UICONTROL 必须完成任务]约束。 在大多数情况下，任务的计划开始日期会根据以下公式计算：

[!UICONTROL 迭代结束日期]减(-) [!UICONTROL 任务持续时间]等于(=) [!UICONTROL 任务计划开始日期]

如果项目开始日期在迭代开始日期之后，而项目结束日期在迭代结束日期之后，则使用[!UICONTROL 项目结束日期]而不是迭代结束日期。

您可以将单个Scrum团队配置为默认使用项目日期，而不是迭代日期。 有关信息，请参阅[配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)一文中的[配置将工作项添加到迭代时应用日期的方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)部分。
