---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流
description: 工作流是一组可配置的展示板和信息卡，用于协作处理工作。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: dd1bd5a27a2ed29af29b88b028d8fd34a592aae2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# 管理工作流

工作流是一组可配置的展示板和信息卡，用于协作处理工作。 工作流可以包含从模板创建的不同类型的展示板和工作项的卡片列表。 在工作流中，您可以跟踪迭代或冲刺中的工作。

有关更多信息，请参阅 [使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 和 [在工作流中创建迭代](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

在仪表板上显示工作流，以及您有权访问的不属于工作流的各个展示板。 有关展示板仪表板的信息，请参阅 [使用展示板功能板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). 您可以单击操控板上的任意展示板名称以将其打开。

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
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建工作流

{{step1-to-boards}}

1. 单击 **[!UICONTROL 添加工作流]** 在 [!UICONTROL 工作流] 仪表板区域。
1. 键入要替换的名称 **[!UICONTROL 无标题工作流]** 并按Enter。

   您可以将展示板添加到工作流中或单击 [!UICONTROL **所有讨论区**] 以返回到仪表板。

## 在工作流中创建新展示板

1. 如果您尚未在工作流中，请单击 [!UICONTROL **查看工作流**] ，以打开现有的工作流。
1. 单击 **[!UICONTROL 添加展示板]** 在 [!UICONTROL 讨论区] 工作流选项卡。
1. 为展示板选择模板。

| 模板 | 描述 |
|---------|----------|
| 基本展示板 | 展示板上提供了三个默认列。 可以添加新列，也可以重命名或删除缺省列。 <p>未应用任何列策略。 |
| Kanban 展示板 | 展示板上提供了以下列：“积压”、“新建”、“进行中”、“完成”和“暂停”。 可以添加新列，也可以重命名或删除缺省列。<p>要使用积压，必须为引入列设置过滤器。 有关信息，请参阅 [向展示板添加引入列](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>要查看每列的默认策略，请单击 [!UICONTROL **更多** 菜单] 在列上并选择 [!UICONTROL **编辑**]. 您可以更改这些预设策略中的任何一个。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| 回顾展示板 | 展示板上提供了以下列：哪些方面进展顺利？ 有什么可以改进的? 我们应该为谁庆祝? 我们可以做些什么来加快步伐？? 可以添加新列，也可以重命名或删除缺省列。 <p>未应用任何列策略。 |
| 迭代过程 | 这是用于定义和运行小版本的展示板。 <p>展示板上提供了以下列：“积压”、“新建”、“进行中”、“完成”和“暂停”。 不能向展示板添加任何列。 <p>要查看每列的默认策略，请单击 [!UICONTROL **更多**] 列上的菜单并选择 [!UICONTROL **编辑**]. 您可以更改这些预设策略中的任何一个。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

有关设置讨论区的详细信息，请参阅 [创建或编辑展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 过滤工作流中的讨论区列表

当电路板列表应用除默认值以外的过滤器时，过滤器图标上会显示一个指示符 ![已应用筛选器](assets/boards-filterapplied-30x30.png). 单击 [!UICONTROL **全部清除**] 以删除所有筛选器，然后单击 [!UICONTROL **隐藏筛选器**] 以关闭过滤器面板。

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 以打开工作流。
1. 单击 [!UICONTROL **讨论区**] 选项卡。
1. 单击 [!UICONTROL **筛选条件**].
1. 按状态选择要查看的展示板（已存档展示板、活动展示板或所有展示板）。
1. 选择要按模板查看的展示板。

## 将成员添加到工作流

必须将人员和团队作为成员添加到工作流中，然后才能查看工作流及其内容。 工作流成员可以在工作流中添加和移除成员，并查看哪些展示板位于工作流中。

>[!NOTE]
>
>在工作流成员作为成员添加到该特定展示板之前，他们无法在工作流上打开展示板。

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 以打开工作流。
1. 单击 **[!UICONTROL 添加成员]** 图标 ![添加成员](assets/boards-addmember-spectrum-25x25.png) 将成员和团队添加到工作流。

   此过程与向展示板添加成员相同。 有关更多信息，请参阅 [在讨论区中添加或移除成员](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## 将源添加到工作流

源确定工作流中信息卡的来源。

{{step1-to-boards}}

1. 单击 [!UICONTROL **源**] 图标 ![“源”图标](assets/sources-icon.png) 定义将信息卡导入工作流的源。 此时，唯一可用的源是 [!DNL Adobe Workfront].
1. 添加筛选器以卡片形式从Workfront导入任务和问题。

   为工作流源添加过滤器与为基本展示板或Kanban展示板上的摄取列添加高级过滤器相同。 有关更多信息，请参阅 [向展示板添加引入列](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 配置工作流

{{step1-to-boards}}

1. 在功能板上，单击 [!UICONTROL **查看工作流**] 以打开工作流。
1. 单击 [!UICONTROL **配置**] 以打开 [!UICONTROL 配置工作流] 面板。
1. （可选）展开 [!UICONTROL **工作流**] 并键入工作流的描述。 此描述显示在仪表板上。
1. （可选）展开 [!UICONTROL **迭代**] 以为此工作流定义迭代进程。

   信息卡总数、指向的信息卡数和迭代数都显示在“信息卡列表”部分。 单击 [!UICONTROL **查看列表**] 以打开列表并添加卡片。 有关更多信息，请参阅 [使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   如果已定义迭代，则会显示其开始日期、卡片数和点数。 单击 [!UICONTROL **查看展示板**] 以打开开发周期展示板。 有关更多信息，请参阅 [在工作流中创建迭代](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. （可选）展开 [!UICONTROL **标记**] 以将标记添加到工作流。 搜索标记，或在搜索框中键入新标记名称，然后按Enter创建标记。
