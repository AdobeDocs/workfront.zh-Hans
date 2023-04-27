---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在主板上使用连接的卡
description: 您可以在展示板上添加一个信息卡，该信息卡已连接到Workfront中的现有任务和问题。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 7d671fe66c6a23efad2e8f8f0fa3d2b7b1afcc86
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# 在主板上使用连接的卡

您可以在展示板上添加一个信息卡，该信息卡已连接到 [!DNL Workfront].

当在一个位置为信息卡更新以下任何一个详细信息时，该信息卡会在另一个位置自动更新：

* [!UICONTROL 名称]
* [!UICONTROL 描述]
* [!UICONTROL 被分派人]
* [!UICONTROL 状态]
* [!UICONTROL 计划的完成日期]
* [!UICONTROL 估计] / [!UICONTROL 故事点]

>[!NOTE]
>单个连接的任务或问题只能在每个主板上添加一次。 同一任务或问题可以连接到多个展示板。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>访问级别配置*</strong></td>
   <td><p>[!UICONTROL视图]或更高版本对任务和问题的访问权限</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>对象权限</strong></td>
   <td><p>[!UICONTROL视图]或更高对Workfront任务或问题的权限</p></td>
  </tr>
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 添加连接的卡

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 展示板]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 添加卡片] > [!UICONTROL 连接卡]**.
1. 选择一个项目，然后选择任务或问题以添加为展示板上的信息卡。

   您可以选择多个对象，这些对象都将作为单独的卡片添加。

   >[!NOTE]
   >
   >* 搜索结果中只有您有权访问的对象可用。 如果某个项目灰显，则它已添加到展示板。
   >* 过滤依据 **[!UICONTROL 我拥有的项目]** 或 **[!UICONTROL 我正在执行的项目]**，则不包括等同于“完成”、“已停用”或“已拒绝”状态的项目。 您仍可以使用 **[!UICONTROL 全部]** 过滤器。


1. 单击 **[!UICONTROL 添加]**.

   ![搜索要连接的任务或问题](assets/boards-tasksissues-350x94.png)

   卡片将添加在最左侧列的底部。 连接的 [!DNL Workfront] 对象及其受分配者显示在卡片上。

   >[!NOTE]
   >
   >如果在 [!DNL Workfront] 任务或问题不是董事会成员，它们未分配给卡。

   ![连接的信息卡](assets/boards-connected-card-first-added.png)

1. 单击 ![打开任务或问题](assets/boards-launch-icon.png) 打开 [!DNL Workfront] 任务或问题。
1. 要编辑卡片详细信息，请单击卡片（不在卡片名称中）。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 卡片详细信息]** 框中，添加或更新以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL名称]</strong></td> 
      <td>更改名称也会更改连接的名称 [!DNL Workfront] 对象。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td> 
      <td>更改描述还会更改连接的 [!DNL Workfront] 对象。 您可以在描述中添加URL，在保存卡片后，这些URL将变为可单击的链接。</td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL任务负责人]</strong></td>
      <td><p>要向信息卡分配更多人员或团队，请开始在搜索字段中键入名称，然后在列表中显示时选择该名称。 您可以添加个人和团队。 在连接的卡上只允许一个团队分配。</p>
      <p>受分配者必须是董事会成员，否则他们不会出现在选择列表中。 当团队是展示板上的成员时，可以将各个团队成员分配到卡片中。</p>
      <p>您选择的任何受分配人也会分配给 [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>选择卡的列。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL状态]</strong></td>
      <td><p>选择卡的状态。 默认值为[!UICONTROL New]、[!UICONTROL In Progress]和[!UICONTROL Complete]，但是在 [!DNL Workfront] 也可用。</p>
      <p>如果启用了列策略来更新字段值，则更改信息卡上的状态会自动将信息卡移至相应的列。 有关更多信息，请参阅文章中的“定义列设置和策略” <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">管理展示板列</a>.</p>
      <p>如果单击 <strong>[!UICONTROL标记结束]</strong> 在卡顶部，状态会自动更改为“完成”。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL计划完成]</strong></td>
      <td>更改此日期还会更改连接的计划完成日期 [!DNL Workfront] 对象。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL估计]</strong></td>
      <td><p>卡片要完成的小时数。</p><p>更改估计也会更改连接上的故事点值 [!DNL Workfront] 对象。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL标记]</strong></td>
      <td><p>搜索并选择卡的标记。</p>
      <p>有关创建新标记的信息，请参阅 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">添加标记</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL核对清单项]</strong> </td> 
      <td> <p>单击 <strong>[!UICONTROL添加核对清单项]</strong>. 然后，键入项目的标题并按Enter。 另一个项目会自动添加。 继续输入标题以添加更多项目。</p> <p>清单顶部的计数器显示已完成项目的数量和项目总数。</p> <p>有关核对清单项目的更多信息，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">管理信息卡上的核对清单项目</a>.</p></td>
     </tr>
    </tbody> 
   </table>

   使用左侧的导航面板可在卡片详细信息的字段组之间移动。

1. 单击 **[!UICONTROL 关闭]** 回到董事会。
卡片上会显示连接的对象、受让人、标记、到期日期、核对清单计数器、预计小时数和状态。

   ![信息卡已添加到展示板](assets/boards-connected-card-details-110922.png)

## 断开连接的卡

您可以从其Workfront对象中断开连接的信息卡，该信息卡会作为临时信息卡保留在展示板中，您可以对其进行编辑。

在主板级别断开连接：

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) 在连接的卡上，然后选择 **[!UICONTROL 断开连接]**.
1. 单击 **[!UICONTROL 断开连接]** 确认消息。

要在卡级别断开连接，请执行以下操作：

1. 访问主板并打开连接的卡。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) 在卡详细信息的“连接”区域中，选择 **[!UICONTROL 断开连接]**.
1. 单击 **[!UICONTROL 断开连接]** 确认消息。

## 将临时卡转换为连接的卡

创建临时信息卡后，可将其转换为连接的信息卡。 有关临时信息卡的详细信息，请参阅 [向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. 访问展示板并打开临时信息卡。
1. 验证卡上的名称和描述。 这些任务或问题将会添加到您在中创建的任务或问题中 [!DNL Workfront].
1. 在 [!UICONTROL 连接] ，单击 **[!UICONTROL 连接Workfront]**.
1. 在 [!UICONTROL 连接卡] ，选择创建任务还是问题。
1. 搜索并选择要将任务或问题添加到的项目。

   >[!NOTE]
   >
   >* 搜索结果中只有您有权访问的对象可用。
   >* 过滤依据 **[!UICONTROL 我拥有的项目]** 或 **[!UICONTROL 我正在执行的项目]**，则等同于 [!UICONTROL 完成], [!UICONTROL 死亡]或 [!UICONTROL 被拒绝] 状态未包含在内。 您仍可以使用 **[!UICONTROL 全部]** 过滤器。


1. 单击 **[!UICONTROL 连接]**.

   ![将临时卡连接到Workfront](assets/boards-connect-ad-hoc-card.png)

   项目名称显示在卡详细信息的“连接”区域中。

1. 单击 **[!UICONTROL 关闭]** 回到董事会。

## 在连接的卡上记录小时数

您必须拥有正确的权限，才能记录连接任务或问题的小时数。

默认情况下，时间日志记录字段不显示在连接的信息卡上。 必须启用 [!UICONTROL **小时**] 在 [!UICONTROL 配置] 区域 [!UICONTROL 卡片]. 有关更多信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 输入任务或问题的小时数。
1. 选择 [!UICONTROL 小时类型] （如果与默认值不同）。
1. 单击 [!UICONTROL **日志时间**].

   ![在卡上记录小时数](assets/log-hours-on-card.png)

   在卡上记录的时间也保存在连接的任务或问题上。

卡片上的日志记录时间与任务或问题上的日志记录时间相同。 有关更多信息，请参阅文章中的“记录项目、任务或问题的时间” [日志时间](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

