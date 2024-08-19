---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 创建或编辑展示板
description: 您可以从[!UICONTROL 展示板]仪表板创建新展示板或编辑现有展示板。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: efe636e14964cc8705839c9f534a9947327803d7
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 1%

---

# 创建或编辑展示板

<!-- Audited: 12/2023 -->

您可以从[!UICONTROL 展示板]仪表板创建新展示板或编辑现有展示板。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档：参与者或更高版本 </p>
 <p>或</p> 
<p>当前： [！UICONTROL Request]或更高版本 </p> 
</td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建新讨论区

{{step1-to-boards}}

1. 单击&#x200B;**[!UICONTROL 添加展示板]**。

1. 为展示板选择模板。

   | 模板 | 描述 |
   |---------|----------|
   | 基本展示板 | 主板上有三个默认列。 您可以添加新列，并重命名或删除默认列。 <p>主板上有三个默认列。 您可以添加新列，并重命名或删除默认列。 |
   | Kanban 展示板 | 以下列显示在展示板上：积压、新增、进行中、完成和搁置。 您可以添加新列，并重命名或删除默认列。<p>要使用积压，必须为引入列设置过滤器。 有关信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。 <p>要查看每列的默认策略，请单击列上的&#x200B;[!UICONTROL **更多**&#x200B;菜单]，然后选择&#x200B;[!UICONTROL **编辑**]。 您可以更改这些预设策略中的任何一个。 有关信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |
   | 回顾展示板 | 讨论区上提供了以下各列：哪些方面进展顺利？ 可以改进什么？ 我们应该为谁庆祝？ 我们可以做些什么来加快步伐？ 您可以添加新列，并重命名或删除默认列。 <p>不应用任何列策略。 |
   | 动态展示板 | 展示板上提供了以下列：未选择、新建、进行中、已暂挂和完成。 您可以添加新列，并重命名或删除默认列。 (可以重命名未选定的列，但不能将其删除。 此列包含状态与任何其他列状态均不匹配的所有信息卡。) <p>默认列策略根据列的状态为列分配信息卡。 有关信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |

1. 仅对于动态展示板，请按照设置向导中的步骤操作：

   1. 键入讨论区的名称，然后单击&#x200B;[!UICONTROL **下一步**]。
   1. 搜索并选择[!DNL Workfront] [!UICONTROL **项目**]&#x200B;以将任务和问题提交到讨论区。
   1. 搜索并选择&#x200B;[!UICONTROL **任务**]&#x200B;以将任务和问题载入讨论区。

      所有对象都以连接的卡片形式显示在展示板上。

      正在添加的&#x200B;[!UICONTROL **卡片**]&#x200B;计数器显示展示板上将有多少卡片。 例如，如果选择具有100个任务和问题的项目，则计数器显示100。 如果添加用户分配并且该用户被分配到项目中的5个任务，则计数器显示5。

      >[!NOTE]
      >
      >动态展示板的卡数量限制为700个任务和700个问题，共1,400张卡。 主板上的卡数量过多可能会影响主板性能。 所有已存档的卡片（包括隐藏和可见的）都计入此限制中。

   1. （可选）选择&#x200B;[!UICONTROL **不存档已完成的卡片**]&#x200B;以将已完成的任务和问题作为可见卡片带入展示板。 如果未选择此选项，则创建展示板时完成的卡片将作为存档卡片放入展示板中。

      >[!NOTE]
      >
      >默认情况下，已存档的信息卡不会显示在展示板上。 要显示已存档的信息卡，您必须打开配置设置，然后筛选展示板以显示已存档的信息卡。 有关详细信息，请参阅[自定义卡片上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)和[在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

   1. （可选）单击&#x200B;[!UICONTROL **使用高级筛选器**]&#x200B;以显示其他筛选器选项。

      此过程与在引入列上创建过滤器的过程相同。 有关详细信息，请参阅[将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

      如果在创建动态展示板后更新其上的筛选器，则未包含在Workfront任务或问题中的卡片设置（如标记）将被重置。

   1. 添加筛选器后，单击&#x200B;[!UICONTROL **创建展示板**]。

1. 在&#x200B;**[!UICONTROL 讨论区]**&#x200B;字段中键入讨论区的名称，然后按Enter。
1. 根据需要配置主板。

   有关信息，请参阅[在展示板上添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md)、[管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md)、[在展示板上添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md)和[在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

1. 单击&#x200B;**[!UICONTROL 所有讨论区]**&#x200B;以返回讨论区仪表板。

   您还可以找到标有当前主板名称的下拉菜单，然后单击该菜单切换到另一个主板。

   ![讨论区列表](assets/boards-button-list-of-boards-350x188.png)

## 编辑现有讨论区

{{step1-to-boards}}

1. 在仪表板上，选择要打开的面板。
1. 根据需要编辑展示板。 您可以单击电路板名称对其进行重命名。

   有关信息，请参阅[在展示板中添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md)、[管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md)和[向展示板添加信息卡](../../agile/get-started-with-boards/add-card-to-board.md)。

1. 单击&#x200B;**[!UICONTROL 所有讨论区]**&#x200B;以返回讨论区仪表板。

   您还可以找到标有当前主板名称的下拉菜单，然后单击该菜单切换到另一个主板。

