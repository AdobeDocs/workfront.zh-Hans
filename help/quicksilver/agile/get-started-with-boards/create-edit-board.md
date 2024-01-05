---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 创建或编辑展示板
description: 从 [!UICONTROL 展示板] 图标板，您可以创建新展示板或编辑现有展示板。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 38715b9571206fd3621b5c078c3eebe380297e9b
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 1%

---

# 创建或编辑展示板

<!-- Audited: 12/2023 -->

从 [!UICONTROL 展示板] 图标板，您可以创建新展示板或编辑现有展示板。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新文档：参与者或更高版本 </p>
 <p>或</p> 
<p>当前： [！UICONTROL Request]或更高版本 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 创建新讨论区

{{step1-to-boards}}

1. 单击 **[!UICONTROL 添加展示板]**.

1. 为展示板选择模板。

   | 模板 | 描述 |
   |---------|----------|
   | 基本展示板 | 主板上有三个默认列。 您可以添加新列，并重命名或删除默认列。 <p>主板上有三个默认列。 您可以添加新列，并重命名或删除默认列。 |
   | Kanban 展示板 | 以下列显示在展示板上：积压、新增、进行中、完成和搁置。 您可以添加新列，并重命名或删除默认列。<p>要使用积压，必须为引入列设置过滤器。 有关信息，请参阅 [将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>要查看每列的默认策略，请单击 [!UICONTROL **更多** 菜单] 在列上并选择 [!UICONTROL **编辑**]. 您可以更改这些预设策略中的任何一个。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | 回顾展示板 | 讨论区上提供了以下各列：哪些方面进展顺利？ 可以改进什么？ 我们应该为谁庆祝？ 我们可以做些什么来加快步伐？ 您可以添加新列，并重命名或删除默认列。 <p>不应用任何列策略。 |
   | 动态展示板 | 展示板上提供了以下列：未选择、新建、进行中、已暂挂和完成。 您可以添加新列，并重命名或删除默认列。 (可以重命名未选定的列，但不能将其删除。 此列包含状态与任何其他列状态均不匹配的所有信息卡。) <p>默认列策略根据列的状态为列分配信息卡。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. 仅对于动态展示板，请按照设置向导中的步骤操作：

   1. 搜索并选择 [!DNL Workfront] [!UICONTROL **项目**] 将任务和问题提交到讨论区。
   1. 搜索并选择 [!UICONTROL **指定任务**] 将任务和问题提交到讨论区。

      所有对象都以连接的卡片形式显示在展示板上。

      此 [!UICONTROL **正在添加的卡片**] 计数器显示展示板上将包含多少张卡。 例如，如果选择具有100个任务和问题的项目，则计数器显示100。 如果添加用户分配并且该用户被分配到项目中的5个任务，则计数器显示5。

   1. （可选）选择 [!UICONTROL **将已完成的工作作为存档信息卡提供**] 将已完成的任务和问题作为存档信息卡载入展示板。

      >[!NOTE]
      >
      >默认情况下，已存档的信息卡不会显示在展示板上。 要显示已存档的信息卡，您必须打开配置设置，然后筛选展示板以显示已存档的信息卡。 有关详细信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) 和 [在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).
      >
      >如果未选择此选项，则展示板创建时完成的卡片不会显示在展示板上。 以后标记为完成的卡片会保留在展示板的“完成”列中，除非您设置卡片减少，否则不会存档。 有关更多信息，请参阅 [配置信息卡减少](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

   1. （可选）单击 [!UICONTROL **使用高级过滤器**] 以显示其他筛选器选项。

      此过程与在引入列上创建过滤器的过程相同。 有关更多信息，请参阅 [将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. 添加筛选器后，单击 [!UICONTROL **创建展示板**].

1. 在中键入讨论区的名称 **[!UICONTROL 展示板]** 字段，然后按Enter。
1. 根据需要配置主板。

   有关信息，请参阅 [在讨论区中添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md)， [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md)、和 [在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 单击 **[!UICONTROL 所有讨论区]** 以返回到展示板仪表板。

   您还可以找到标有当前主板名称的下拉菜单，然后单击该菜单切换到另一个主板。

   ![讨论区列表](assets/boards-button-list-of-boards-350x188.png)

## 编辑现有讨论区

{{step1-to-boards}}

1. 在仪表板上，选择要打开的面板。
1. 根据需要编辑展示板。 您可以单击电路板名称对其进行重命名。

   有关信息，请参阅 [在讨论区中添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md)、和 [向展示板添加信息卡](../../agile/get-started-with-boards/add-card-to-board.md).

1. 单击 **[!UICONTROL 所有讨论区]** 以返回到展示板仪表板。

   您还可以找到标有当前主板名称的下拉菜单，然后单击该菜单切换到另一个主板。
