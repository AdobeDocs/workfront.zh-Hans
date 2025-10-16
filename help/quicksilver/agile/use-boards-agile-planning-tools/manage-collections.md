---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流
description: 工作流是一组可配置的展示板和卡片，用于协作处理工作。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 1%

---

# 管理工作流

>[!IMPORTANT]
>
>工作流仅适用于特定的客户组。

工作流是一组可配置的展示板和卡片，用于协作处理工作。 工作流可以包括从模板创建的不同类型的展示板和工作项的卡片列表。 在工作流中，您可以跟踪迭代或冲刺中的工作。

有关详细信息，请参阅[使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)和[在工作流中创建迭代](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

工作流，以及您有权访问的不属于工作流的各个展示板都会显示在仪表板上。 有关展示板仪表板的信息，请参阅[使用展示板仪表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)。 您可以单击仪表板上的任何电路板名称来将其打开。

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

## 创建工作流

{{step1-to-boards}}

1. 在仪表板的&#x200B;**[!UICONTROL 工作流]**&#x200B;区域单击[!UICONTROL 添加工作流]。
1. 键入名称以替换&#x200B;**[!UICONTROL 无标题工作流]**，然后按Enter。

   您可以将展示板添加到工作流，或单击&#x200B;[!UICONTROL **所有展示板**]&#x200B;返回到仪表板。

## 在工作流中创建新讨论区

1. 如果您尚未在工作流中，请单击仪表板上的&#x200B;[!UICONTROL **查看工作流**]&#x200B;以打开现有的工作流。
1. 在工作流的&#x200B;**[!UICONTROL 讨论区]**&#x200B;选项卡上单击[!UICONTROL 添加讨论区]。
1. 为展示板选择模板。

| 模板 | 描述 |
|---------|----------|
| 基本展示板 | 主板上有三个默认列。 您可以添加新列，并重命名或删除默认列。 <p>不应用任何列策略。 |
| Kanban 展示板 | 以下列显示在展示板上：积压、新增、进行中、完成和搁置。 您可以添加新列，并重命名或删除默认列。<p>要使用积压，必须为引入列设置过滤器。 有关信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。 <p>要查看每列的默认策略，请单击列上的&#x200B;[!UICONTROL **更多**&#x200B;菜单]，然后选择&#x200B;[!UICONTROL **编辑**]。 您可以更改这些预设策略中的任何一个。 有关信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |
| 回顾展示板 | 讨论区上提供了以下各列：哪些方面进展顺利？ 可以改进什么？ 我们应该为谁庆祝？ 我们可以做些什么来加快步伐？ 您可以添加新列，并重命名或删除默认列。 <p>不应用任何列策略。 |
| 迭代过程 | 这是用于定义和运行迭代的展示板。 <p>以下列显示在展示板上：积压、新增、进行中、完成和搁置。 不能向展示板添加任何列。 <p>要查看每列的默认策略，请单击列上的&#x200B;[!UICONTROL **更多**]&#x200B;菜单，然后选择&#x200B;[!UICONTROL **编辑**]。 您可以更改这些预设策略中的任何一个。 有关信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |

有关设置讨论区的详细信息，请参阅[创建或编辑讨论区](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)。

## 过滤工作流中的讨论区列表

将默认以外的筛选器应用于展示板列表时，筛选器图标![应用的筛选器](assets/boards-filterapplied-30x30.png)上将显示指示符。 单击&#x200B;[!UICONTROL **全部清除**]&#x200B;可删除所有筛选器，单击&#x200B;[!UICONTROL **隐藏筛选器**]&#x200B;可关闭筛选器面板。

{{step1-to-boards}}

1. 在仪表板上，单击&#x200B;[!UICONTROL **查看工作流**]&#x200B;以打开工作流。
1. 单击&#x200B;[!UICONTROL **展示板**]&#x200B;选项卡（如果尚未显示）。
1. 单击&#x200B;[!UICONTROL **筛选器**]。
1. 选择要按状态查看的展示板（已存档展示板、活动展示板或所有展示板）。
1. 选择要按模板查看的展示板。

## 将成员添加到工作流

必须将人员和团队作为成员添加到工作流中，然后才能查看工作流及其内容。 工作流成员可以在工作流中添加和移除成员，并查看哪些展示板位于工作流中。

>[!NOTE]
>
>在工作流成员作为成员添加到该特定展示板之前，他们无法在工作流上打开展示板。

{{step1-to-boards}}

1. 在仪表板上，单击&#x200B;[!UICONTROL **查看工作流**]&#x200B;以打开工作流。
1. 单击&#x200B;**[!UICONTROL 添加成员]**&#x200B;图标![添加成员](assets/boards-addmember-spectrum-25x25.png)以将成员和团队添加到工作流。

   此过程与将成员添加到展示板相同。 有关详细信息，请参阅[添加或移除讨论区中的成员](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md)。

## 将源添加到工作流

源确定工作流中卡片的来源。

{{step1-to-boards}}

1. 单击&#x200B;[!UICONTROL **源**]&#x200B;图标![源图标](assets/sources-icon.png)定义将信息卡导入工作流的源。 此时，唯一可用的源是[!DNL Adobe Workfront]。
1. 添加筛选器以将任务和问题作为信息卡从Workfront导入。

   为工作流源添加筛选器与为基本展示板或Kanban展示板上的摄取列添加高级筛选器相同。 有关详细信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

## 配置工作流

{{step1-to-boards}}

1. 在仪表板上，单击&#x200B;[!UICONTROL **查看工作流**]&#x200B;以打开工作流。
1. 单击&#x200B;[!UICONTROL **配置**]&#x200B;以打开[!UICONTROL 配置工作流]面板。
1. （可选）展开&#x200B;[!UICONTROL **工作流**]&#x200B;并键入工作流的说明。 此描述将显示在仪表板上。
1. （可选）展开&#x200B;[!UICONTROL **迭代**]&#x200B;以定义此工作流的迭代进程。

   信息卡总数、针尖信息卡数和迭代数都显示在Card List部分。 单击&#x200B;[!UICONTROL **查看列表**]&#x200B;打开列表并添加卡片。 有关详细信息，请参阅[使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)。

   如果已定义迭代，则会显示其开始日期、卡片数和点数。 单击&#x200B;[!UICONTROL **查看展示板**]&#x200B;以打开迭代展示板。 有关详细信息，请参阅[在工作流中创建迭代](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

1. （可选）展开&#x200B;[!UICONTROL **标记**]&#x200B;以将标记添加到工作流。 搜索标记，或在搜索框中键入新标记名称，然后按Enter创建标记。
