---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在展示板上使用连接的信息卡
description: 您可以在展示板上添加一张信息卡，该信息卡连接到Workfront中的现有任务和问题。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: e7b4fef2485f08df6655b5e441784ae84fc36de8
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 在展示板上使用连接的信息卡

{{preview-and-fast-release}}

您可以在展示板上添加一个连接到中现有任务和问题的信息卡 [!DNL Workfront].

当在一个位置更新信息卡的以下任何详细信息时，都会在另一个位置自动更新该信息卡：

* [!UICONTROL 名称]
* [!UICONTROL 描述]
* [!UICONTROL 被分派人]
* [!UICONTROL 状态]
* [!UICONTROL 计划的完成日期]
* [!UICONTROL 估计] / [!UICONTROL 故事点]
* <span class="preview">[!UICONTROL 文档]</span>

>[!NOTE]
>
>每个展示板只能添加一次单个连接的任务或问题。 同一任务或问题可以连接到多个讨论区。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>访问级别配置*</strong></td>
   <td><p>[！UICONTROL视图]或更高权限访问任务和问题</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>对象权限</strong></td>
   <td><p>[！UICONTROL View]或对Workfront任务或问题的更高权限</p></td>
  </tr>
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 添加连接的卡片

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 添加信息卡] > [!UICONTROL 已连接的信息卡]**.
1. 选择一个项目，然后选择要作为信息卡添加到展示板上的任务或问题。

   您可以选择多个对象，它们都将作为单独的卡片进行添加。

   >[!NOTE]
   >
   >* 搜索结果中只有您拥有权限的对象可用。 如果项目变暗，则表示该项目已被添加到展示板中。
   >* 当您按以下项筛选时 **[!UICONTROL 我拥有的项目]** 或 **[!UICONTROL 我在处理的项目]**，不包括等同于“完成”、“终止”或“拒绝”状态的项目。 您仍然可以使用搜索这些项目 **[!UICONTROL 全部]** 筛选。

1. 单击 **[!UICONTROL 添加]**.

   ![搜索要连接的任务或问题](assets/boards-tasksissues-350x94.png)

   卡片会添加到最左列的底部。 连接的 [!DNL Workfront] 对象及其任务负责人将显示在信息卡上。

   ![连接的信息卡](assets/boards-connected-card-first-added.png)

1. 单击 ![未结任务或问题](assets/boards-launch-icon.png) 以打开 [!DNL Workfront] 新浏览器选项卡中的任务或问题。
1. 要编辑信息卡的详细信息，请单击该信息卡（不在信息卡名称中）。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 信息卡详细信息]** 框中，添加或更新以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL名称]</strong></td> 
      <td>更改名称也会更改已连接的名称 [!DNL Workfront] 对象。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL描述]</strong></td> 
      <td>更改描述也会更改已连接设备上的描述 [!DNL Workfront] 对象。 您可以在描述中添加URL，保存信息卡后，这些URL将成为可单击的链接。</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL列]</strong></td>
      <td>选择卡片的列。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL状态]</strong></td>
      <td><p>选择卡的状态。 默认值为[！UICONTROL New]、[！UICONTROL In Progress]和[！UICONTROL Complete]，但是为中的项目定义的任何自定义状态。 [!DNL Workfront] 也提供。</p>
      <p>如果您启用了列策略来更新字段值，则更改信息卡上的状态会自动将信息卡移动到相应的列。 有关更多信息，请参阅文章中的“定义列设置和策略” <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">管理展示板列</a>.</p>
      <p>如果您单击 <strong>[！UICONTROL标记完成]</strong> 在信息卡顶部，状态会自动更改为“完成”。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL计划完成]</strong></td>
      <td>更改此日期也会更改连接的计划完成日期 [!DNL Workfront] 对象。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[！UICONTROL估计]</strong></td>
      <td><p>完成信息卡的小时数。</p><p>更改估计也会更改连接的故事点值 [!DNL Workfront] 对象。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL分配]</strong></td>
      <td><p>要将更多人员或团队分配给信息卡，请单击 <strong>[！UICONTROL Add Assignment]</strong> 并开始在搜索字段中键入名称。 然后，当它显示在结果列表中时将其选中。 您可以同时添加个人和团队。 一个已连接的信息卡上只允许一个团队分配。</p>
      <p>您选择的任何被分配者也会被分配到中的任务或问题 [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL标记]</strong></td>
      <td><p>搜索并选择卡片的标记。</p>
      <p>有关创建新标记的信息，请参阅 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">添加标记</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL自定义字段]</strong></td>
      <td><p>您添加的任何自定义字段都会显示在此区域中。</p>
      <p>有关更多信息，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">自定义信息卡上显示的字段</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[！UICONTROL Subtask]</strong></span></td>
      <td><span class="preview"><p>此部分将显示任务的任何现有子任务。 单击 <strong>[！UICONTROL添加子任务]</strong> 以添加新子任务。</p>
      <p>部分顶部的计数器显示已完成的子任务数和子任务总数。</p>
      <p>有关子任务的详细信息，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">管理展示板上的子任务</a>.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL核对清单]</strong></td>
      <td><p>单击 <strong>[！UICONTROL添加清单项目]</strong>. 然后，键入项目的标题并按Enter。 系统会自动添加另一个项目。 继续输入标题以添加更多项目。</p>
      <p>清单顶部的计数器显示已完成项目的数量和项目总数。</p> <p>有关清单项目的更多信息，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">管理信息卡上的清单项目</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[！UICONTROL文档]</strong></span></td>
      <td><span class="preview">对于现有文档，将鼠标悬停在文档缩略图上，然后单击 <strong>预览</strong> 在浏览器中查看文件，或者 <strong>下载</strong> 将文件下载到您的计算机。 有关新文档，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">在信息卡上添加文档</a>.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL小时]</strong></td>
      <td>请参阅下面的“在连接的卡上记录小时数”。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL Comments]</strong></td>
      <td><p>单击 <strong>[！UICONTROL新注释]</strong> 字段并键入您的评论。 使用格式设置工具设置文本格式，然后单击 <strong>添加附件</strong> 图标 <img src="assets/attachment-icon.png" alt="“附件”图标"> 将文件附加到注释。 要标记人员或团队，请使用评论区域底部的搜索框。 用户不必是讨论区的成员。 已连接信息卡上已标记的用户将收到电子邮件通知。</p><p>单击 <strong>[！UICONTROL提交]</strong> 以向卡片添加注释。</p>
      <p><strong>注意：</strong> 信息卡上的评论区域使用新的Adobe Workfront评论体验。 有关更多信息，请参阅 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">更新工作</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL系统活动]</strong></td> 
      <td><p>如果您拥有 <strong>系统活动</strong> 将活动启用为卡片部分，会在此区域显示活动。</p> <p>有关更多信息，请参阅 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">自定义信息卡上显示的字段</a> 和 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">系统跟踪更新</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   使用左侧导航面板在信息卡详细信息中的字段部分之间移动。

1. 单击 **[!UICONTROL 关闭]** 以回到董事会。
卡片上将显示连接的对象、任务接受者、标记、截止日期、清单计数器、估计小时数和状态。

   ![信息卡已添加到展示板](assets/boards-connected-card-details-110922.png)

## 断开连接的卡

您可以断开已连接信息卡与其Workfront对象的连接，并且该信息卡会作为可编辑的临时信息卡保留在展示板上。

要在主板级别断开连接，请执行以下操作：

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 断开连接]**.
1. 单击 **[!UICONTROL 断开连接]** 确认消息上。

要在卡级别断开连接，请执行以下操作：

1. 使用主板并打开连接的卡。
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) 在卡详细信息的“连接”区域，然后选择 **[!UICONTROL 断开连接]**.
1. 单击 **[!UICONTROL 断开连接]** 确认消息上。

## 将临时信息卡转换为连接的信息卡

创建临时信息卡后，可将其转换为已连接的信息卡。 有关临时信息卡的详细信息，请参阅 [向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. 访问展示板并打开Ad Hoc卡。
1. 验证卡上的名称和描述。 它们将被添加到您在中创建的任务或问题中 [!DNL Workfront].
1. 在 [!UICONTROL 连接] 信息卡详细信息区域，单击 **[!UICONTROL 与Workfront连接]**.
1. 在 [!UICONTROL 连接卡] 窗口中，选择您是创建任务还是创建问题。
1. 搜索并选择要将任务或问题添加到的项目。

   >[!NOTE]
   >
   >* 搜索结果中只有您拥有权限的对象可用。
   >* 当您按以下项筛选时 **[!UICONTROL 我拥有的项目]** 或 **[!UICONTROL 我在处理的项目]**，等同于 [!UICONTROL 完成]， [!UICONTROL 废弃]，或 [!UICONTROL 被拒绝] 不包括状态。 您仍然可以使用搜索这些项目 **[!UICONTROL 全部]** 筛选。

1. 单击 **[!UICONTROL 连接]**.

   ![将ad hoc卡连接到Workfront](assets/boards-connect-ad-hoc-card.png)

   项目名称显示在卡片详细信息的“连接”区域。

1. 单击 **[!UICONTROL 关闭]** 以回到董事会。

## 在连接的卡片上记录小时数

您必须具有正确的权限，才能在连接的任务或问题上记录小时数。

默认情况下，已连接的信息卡上不显示时间日志记录字段。 您必须启用 [!UICONTROL **小时**] 在 [!UICONTROL 配置] 区域在 [!UICONTROL 卡片]. 有关更多信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 输入任务或问题的小时数。
1. 选择 [!UICONTROL 小时类型] （如果不同于缺省值）。
1. 单击 [!UICONTROL **记录时间**].

   ![在信息卡上记录小时数](assets/log-hours-on-card.png)

   信息卡上的登录时间也会保存在连接的任务或问题上。

信息卡上的记录时间与任务或问题的记录时间相同。 有关更多信息，请参阅文章中的“在项目、任务或问题上记录时间” [记录时间](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

