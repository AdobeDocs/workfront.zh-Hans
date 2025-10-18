---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 向展示板添加临时信息卡
description: 您可以快速将临时信息卡添加到展示板并将其分配给展示板上的成员。 信息卡可以表示任务、问题、人员、组或要包含在展示板中的任何类型的项目。
author: Jenny
feature: Agile
exl-id: 9bc1f92a-85b0-44fd-b5de-09a69af6def5
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 向展示板添加临时信息卡

您可以快速将信息卡添加到展示板并将其分配给展示板上的成员。 信息卡可以表示任务、问题、人员、组或要包含在展示板中的任何类型的项目。

>[!NOTE]
>
>展示板上的临时信息卡未连接到[!DNL Adobe Workfront]中的工作项。 有关连接的卡的详细信息，请参阅[在展示板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 添加包含完整详细信息的临时信息卡

临时信息卡未连接到[!DNL Adobe Workfront]中的工作项。

{{step1-to-boards}}

1. 访问展示板。 有关信息，请参阅[创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 单击&#x200B;**[!UICONTROL 添加信息卡] > [!UICONTROL 新信息卡]**。

   出现[!UICONTROL 卡片详细信息]框。

   >[!NOTE]
   >
   >如果您在“名称”字段的外部单击，则临时信息卡会自动保存为“无标题”显示在最左列的底部。 要退出但不保存信息卡，您必须单击&#x200B;[!UICONTROL **取消**]，而不单击[!UICONTROL 信息卡详细信息]框中的其他位置。

1. 在&#x200B;**[!UICONTROL 卡片详细信息]**&#x200B;框中，添加以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL名称]</strong> </td> 
      <td>卡的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL描述]</strong> </td> 
      <td>信息卡的描述。 您可以在描述中添加URL，保存信息卡后，这些URL将成为可单击的链接。</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL列]</strong> </td> 
      <td>选择卡片的列。 如果将<strong>[！UICONTROL列]</strong>字段留空，则该卡片会放置在展示板左侧的第一列中。</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL状态]</strong> </td> 
      <td>选择卡的状态。 如果单击信息卡顶部的<strong>[！UICONTROL标记完成]</strong>，则状态会自动更改为[！UICONTROL完成]。</td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL到期日期]</strong></td> 
      <td>选择卡的到期日期。 </td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL估计]</strong></td> 
      <td>键入要完成的卡的估计小时数。 这只是一个手动输入。</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL分配]</strong> </td> 
      <td>要分配卡片，请单击<strong>[！UICONTROL添加分配]</strong>，然后在搜索字段中开始键入名称。 然后，当它显示在结果列表中时将其选中。 您可以同时添加个人和团队，也可以将多个人员或团队分配给信息卡。</td>
     </tr>     
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL标记]</strong></td> 
      <td>搜索并选择卡片的标记。 有关创建新标记的信息，请参阅<a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">添加标记</a>。</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL连接]</strong> </td>
      <td>您可以将临时信息卡连接到[!DNL Workfront]任务或问题。 有关详细信息，请参阅文章<a href="/help/quicksilver/agile/get-started-with-boards/connected-cards.md">在展示板上使用连接的信息卡</a>中的“将临时信息卡转换为连接的信息卡”。</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL清单]</strong> </td> 
      <td> <p>单击<strong>[！UICONTROL添加清单项目]</strong>。 然后，键入项目的标题并按Enter。 系统会自动添加另一个项目。 继续输入标题以添加更多项目。</p> <p>清单顶部的计数器显示已完成项目的数量和项目总数。</p> <p>有关清单项目的详细信息，请参阅<a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">管理卡片上的清单项目</a>。</p> </td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL Comments]</strong></td>
      <td><p>单击<strong>[！UICONTROL新建评论]</strong>字段并键入您的评论。 使用格式设置工具设置文本的格式。 （图像在临时信息卡上的评论中不可用。） 要标记人员或团队，请使用评论区域底部的搜索框。 用户不必是讨论区的成员。</p><p><strong>注意：</strong>目前，在临时信息卡上标记为评论的用户不接收电子邮件通知。
      </p><p>单击<strong>[！UICONTROL Submit]</strong>以将评论添加到卡片。</p>
      <p>有关评论的更多信息，请参阅<a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">更新工作</a>。</p></td>
     </tr>
    </tbody> 
   </table>

   ![临时信息卡详细信息](assets/ad-hoc-card-details-with-comments.png)

   使用左侧导航面板在信息卡详细信息中的字段部分之间移动。

1. 单击&#x200B;**[!UICONTROL 关闭]**&#x200B;以将卡添加到展示板。

   信息卡上会显示被分配人、标记、截止日期、清单计数器、估计小时数和状态。

## 快速添加临时信息卡

您可以添加只有标题的临时信息卡，以快速填充展示板。

1. 访问要将信息卡添加到的展示板。
1. 在要添加信息卡的列上单击&#x200B;**[!UICONTROL 添加]**&#x200B;图标![添加信息卡](assets/addicon-spectrum.png)。
1. 键入卡名称，然后按Enter。

   另一张信息卡会自动添加到新信息卡的下方。

1. 继续输入卡片名称以添加更多卡片。
1. 要停止添加信息卡，请单击列外部。
1. 要添加更多详细信息，您必须编辑卡片。 有关信息，请参阅本文中的[编辑现有信息卡](#edit-an-existing-card)。

## 编辑现有信息卡 {#edit-an-existing-card}

1. 访问展示板。
1. 单击卡片名称可编辑名称。
1. 要编辑信息卡的详细信息，请单击该信息卡（不在信息卡名称中）。

   或

   单击卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![[!UICONTROL 更多菜单]](assets/more-icon-spectrum.png)，然后选择&#x200B;**[!UICONTROL 编辑]**。

1. 在[!UICONTROL 卡片详细信息]框中，根据需要更新信息，然后单击&#x200B;**[!UICONTROL 关闭]**&#x200B;返回讨论区。

   如果您启用了列策略来更新字段值，则更改信息卡上的状态会自动将信息卡移动到相应的列。 有关详细信息，请参阅文章[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)中的“定义列设置和策略”。
