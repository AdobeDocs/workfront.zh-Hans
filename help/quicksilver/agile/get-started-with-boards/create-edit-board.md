---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 创建或编辑展示板
description: 从 [!UICONTROL 展示板] 功能板中，您可以创建新展示板或编辑现有展示板。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 3%

---

# 创建或编辑展示板

从 [!UICONTROL 展示板] 功能板中，您可以创建新展示板或编辑现有展示板。

要向工作流添加展示板，请参阅 [管理工作流](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建新展示板

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 展示板]**.
1. 要创建独立展示板，请单击 **[!UICONTROL 添加展示板]** 在 [!UICONTROL 展示板] 的上界。 要向工作流添加展示板，请参阅 [管理工作流](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. 为展示板选择模板。

   | 模板 | 描述 |
   |---------|----------|
   | 基本展示板 | 展示板上提供了三个默认列。 您可以添加新列，并重命名或删除默认列。 <p>展示板上提供了三个默认列。 您可以添加新列，并重命名或删除默认列。 |
   | Kanban 展示板 | 展示板上提供了以下列：积压、新增、进行中、完成和暂挂。 您可以添加新列，并重命名或删除默认列。<p>要使用积压工作，必须为进气列设置过滤器。 有关信息，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>要查看每列的默认策略，请单击 [!UICONTROL **更多** 菜单] 在列中，然后选择 [!UICONTROL **编辑**]. 您可以更改其中任何预设策略。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | 回顾展示板 | 展示板上提供了以下列：什么进展顺利？ 有什么可以改进的? 我们应该为谁庆祝? 我们可以做些什么来加快步伐？? 您可以添加新列，并重命名或删除默认列。 <p>未应用列策略。 |
   | 动态展示板 | 展示板上提供了以下列：未选择、新建、进行中、暂挂和完成。 您可以添加新列，并重命名或删除默认列。 (可以重命名“未选定”列，但不能删除。 此列包含状态与任何其他列状态不匹配的所有信息卡。) <p>默认列策略会根据列的状态将信息卡分配给列。 有关信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). <p>**注意：** 动态展示板仅通过Workfront展示板的早期功能选择加入提供。 |

1. 仅对于动态展示板，请按照安装向导的步骤操作：

   1. 搜索并选择 [!DNL Workfront] [!UICONTROL **项目**] 把任务和问题带到董事会。
   1. 搜索并选择 [!UICONTROL **分配**] 把任务和问题带到董事会。

      所有对象都以连接卡的形式显示在主板上。

      的 [!UICONTROL **添加的信息卡**] 计数器显示展示板上有多少张卡片。 例如，如果您选择的项目包含100个任务和问题，则计数器会显示100个。 如果您添加了用户分配，并且该人员被分配到项目上的5个任务，则计数器会显示5个任务。

   1. （可选）选择 [!UICONTROL **包括已完成的工作**] 在展示板上包含已填写的卡片。

      >[!NOTE]
      >
      >如果未选择此选项，则当其他状态的信息卡标记为完成时，它们将“掉下”展示板，不再显示。

   1. （可选）单击 [!UICONTROL **使用高级过滤器**] 以显示其他过滤器选项。

      这与在进气列上创建过滤器的过程相同。 有关更多信息，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. 添加过滤器后，单击 [!UICONTROL **创建展示板**].

1. 在 **[!UICONTROL 展示板]** 字段，然后按Enter。
1. 根据需要配置展示板。

   有关信息，请参阅 [在展示板中添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md), [管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md), [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md)和 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 单击 **[!UICONTROL 所有展示板]** 返回到展示板仪表板。

   您还可以找到标有当前展示板名称的下拉菜单，然后单击该菜单以切换到其他展示板。

   ![展示板列表](assets/boards-button-list-of-boards-350x188.png)

## 编辑现有展示板

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 展示板]**.
1. 在功能板上，选择要打开的展示板。
1. 根据需要编辑展示板。 您可以单击展示板名称以对其进行重命名。

   有关信息，请参阅 [在展示板中添加或删除成员](../../agile/get-started-with-boards/add-members-to-board.md), [管理展示板列](../../agile/get-started-with-boards/manage-board-columns.md)和 [将信息卡添加到展示板](../../agile/get-started-with-boards/add-card-to-board.md).

1. 单击 **[!UICONTROL 所有展示板]** 返回到展示板仪表板。

   您还可以找到标有当前展示板名称的下拉菜单，然后单击该菜单以切换到其他展示板。
