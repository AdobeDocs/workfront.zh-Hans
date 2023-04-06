---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流
description: 工作流是一组可配置的展示板和卡片，用于协作处理工作。
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 3%

---

# 管理工作流

工作流是一组可配置的展示板和卡片，用于协作处理工作。 工作流可以包括根据模板创建的不同类型的展示板以及工作项的卡片列表。 在工作流中，您可以跟踪小版本或短划分中的工作。

有关更多信息，请参阅 [使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 和 [在工作流中创建小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

工作流会与您有权访问的各个展示板一起显示在功能板上，这些展示板不属于工作流的一部分。 有关展示板仪表板的信息，请参阅 [使用展示板仪表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). 您可以单击功能板上的任何展示板名称以将其打开。

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
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建工作流

{{step1-to-boards}}

1. 单击 **[!UICONTROL 添加工作流]** 在 [!UICONTROL 工作流] 中。
1. 键入要替换的名称 **[!UICONTROL 无标题工作流]** 按Enter键。

   您可以向工作流中添加展示板，或单击 [!UICONTROL **所有展示板**] 返回功能板。

## 在工作流中创建新展示板

1. 如果您尚未在工作流中，请单击 [!UICONTROL **查看工作流**] 在功能板中打开现有工作流。
1. 单击 **[!UICONTROL 添加展示板]** 在 [!UICONTROL 展示板] 选项卡。
1. 为展示板选择模板。

| 模板 | 描述 |
|---------|----------|
| 基本展示板 | 展示板上提供了三个默认列。 您可以添加新列，并重命名或删除默认列。 <p>未应用列策略。 |
| Kanban 展示板 | 展示板上提供了以下列：积压、新增、进行中、完成和暂挂。 您可以添加新列，并重命名或删除默认列。<p>要使用积压工作，必须为进气列设置过滤器。 有关信息，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>要查看每列的默认策略，请单击 [!UICONTROL **更多** 菜单] 在列中，然后选择 [!UICONTROL **编辑**]. 您可以更改其中任何预设策略。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| 回顾展示板 | 展示板上提供了以下列：什么进展顺利？ 有什么可以改进的? 我们应该为谁庆祝? 我们可以做些什么来加快步伐？? 您可以添加新列，并重命名或删除默认列。 <p>未应用列策略。 |
| 迭代过程 | 这是用于定义和运行迭代的展示板。 <p>展示板上提供了以下列：积压、新增、进行中、完成和暂挂。 不能向展示板添加任何列。 <p>要查看每列的默认策略，请单击 [!UICONTROL **更多**] 菜单，然后选择 [!UICONTROL **编辑**]. 您可以更改其中任何预设策略。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

有关设置展示板的更多信息，请参阅 [创建或编辑展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 在工作流中筛选展示板列表

当在展示板列表中应用默认值以外的过滤器时，过滤器图标上会显示一个指示器 ![已应用过滤器](assets/boards-filterapplied-30x30.png). 单击 [!UICONTROL **全部清除**] 删除所有过滤器，然后单击 [!UICONTROL **隐藏过滤器**] 来关闭过滤器面板。

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 打开工作流。
1. 单击 [!UICONTROL **展示板**] 选项卡。
1. 单击 [!UICONTROL **过滤器**].
1. 选择要按状态显示的展示板（存档的展示板、活动展示板或所有展示板）。
1. 选择要按模板查看的展示板。

## 向工作流添加成员

必须将人员和团队作为成员添加到工作流中，然后才能查看工作流及其内容。 工作流成员可以添加和删除工作流上的成员，并查看工作流中的展示板。

>[!NOTE]
>
>工作流成员只有在作为成员添加到该特定工作流中后，才能在该工作流中打开展示板。

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 打开工作流。
1. 单击 **[!UICONTROL 添加成员]** 图标 ![添加成员](assets/boards-addmember-spectrum-25x25.png) 向工作流中添加成员和团队。

   这与向展示板添加成员的过程相同。 有关更多信息，请参阅 [在展示板中添加或删除成员](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## 配置工作流

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 打开工作流。
1. 单击 [!UICONTROL **配置**] 打开 [!UICONTROL 配置工作流] 的上界。
1. （可选）键入工作流的描述。 此描述显示在功能板中。

   卡片总数、指向的卡片数和小版本数显示在“卡片列表”部分。 单击 [!UICONTROL **查看列表**] 打开列表并添加信息卡。 有关更多信息，请参阅 [使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   如果已定义小版本，则会显示其开始日期、卡数和点数。 单击 [!UICONTROL **查看迭代展示板**] 打开展示板。 有关更多信息，请参阅 [在工作流中创建小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. 单击 [!UICONTROL **添加源**] 定义将信息卡导入工作流的源。 此时，唯一可用的源是 [!DNL Adobe Workfront].
1. 添加过滤器以将任务和问题从Workfront导入为信息卡。

   为工作流源添加过滤器与为基本板或看板板上的进纸列添加过滤器相同。 有关更多信息，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

