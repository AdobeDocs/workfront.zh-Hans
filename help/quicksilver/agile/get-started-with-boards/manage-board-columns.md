---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理展示板上的列
description: 默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列以及删除任何不需要的列。 您还可以定义列策略。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 0%

---

# 管理展示板上的列

<!-- Audited: 05/2024 -->

默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列以及删除任何不需要的列。

列设置包括策略，这些策略允许您定义卡片被移动到该列时卡片所发生的变化。

有关对列中的卡片进行排序的信息，请参阅 [在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档：参与者或更高版本 </p>
        <p>或</p> 
        <p>当前： [！UICONTROL Request]或更高版本 </p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 向展示板添加列

{{step1-to-boards}}

1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 添加列]** 位于现有列的右侧。
1. 在新列中，键入名称并单击 **[!UICONTROL 添加列]**.

   ![添加新列](assets/boards-add-column.png)

>[!TIP]
>
>要添加引入列，请参见 [将引入列添加到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 对展示板上的列重新排序

1. 访问展示板。
1. 按正确的顺序拖放各列。 在将该列拖到其他位置之前，请务必选择列的顶部。

   ![拖放列](assets/boards-dragdropcolumn.png)

## 重命名展示板列

1. 访问展示板。
1. 单击列名，键入新名称，然后按Enter键。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) 在列上并选择 **[!UICONTROL 编辑]**. 在“设置”区域中，在 **[!UICONTROL 列名称]** 字段，然后单击 **[!UICONTROL 关闭]**.

## 删除展示板列

从展示板中删除列时，无法恢复该列。

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) 在列上，并选择 **[!UICONTROL 删除]**.

   >[!NOTE]
   >
   >无法删除包含信息卡的列，包括已存档的信息卡。 如果尝试删除包含信息卡的列，则必须为这些信息卡选择另一列。

## 显示卡计数

您可以使用配置设置显示每列中的卡片数量。

如果对列使用WIP限制，则不会添加单独的卡计数器。 有关WIP限制的详细信息，请参阅 [管理 [!UICONTROL 工作进行中] 展示板上的(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 访问展示板。
1. 单击 **[!UICONTROL 配置]** ，打开“配置”面板。
1. 展开 **[!UICONTROL 列]**.
1. 打开 **[!UICONTROL 显示列卡片计数]**.

   ![打开卡计数器](assets/display-card-count.png)

   卡片计数器显示在每列的顶部。

1. 单击 **[!UICONTROL 隐藏配置]** 关闭 [!UICONTROL 配置] 面板。

## 定义列设置和策略

列策略包括自动更新字段值，以及设置进行中的工作限制。

更新状态的策略将自动同时适用于卡和列：

* 当信息卡移动到具有策略的列时，信息卡状态将更新为策略中定义的状态。 这同时适用于ad hoc卡和连接的卡。
* 当信息卡上的临时或已连接信息卡状态更新以匹配策略中的列状态时，或Workfront中的其他位置更新已连接信息卡状态时，信息卡会自动移动到该列。 此外，如果信息卡上的自定义状态与分配给该列的系统状态匹配，则信息卡将被移动到该列。

如果信息卡状态与任何现有列策略中设置的任何状态都不匹配，则该信息卡将保留在放置它的列中。

>[!NOTE]
>
>动态展示板始终将信息卡放在与其状态匹配的列中，无论列策略是启用还是禁用。 当您刷新展示板时，信息卡将返回到其分配的列。
> 
>此外，对于所有展示板类型，如果将信息卡从一列移动到另一列（状态相同），则当您刷新展示板时，信息卡将返回到原始列。

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![更多菜单](assets/more-icon-spectrum.png) 在列上，并选择 **[!UICONTROL 编辑]**.

   此 [!UICONTROL 设置] 区域显示。 此 **[!UICONTROL 列名称]** 让您知道要为哪一列定义设置。

1. 启用 **[!UICONTROL 自动更新字段值]** 策略，用于在将卡片移至此列时自动更改某些字段值。

   ![列设置和策略](assets/boards-column-policies-enabled.png)

1. （可选）设置信息卡状态的值：

   1. 选择 **[!UICONTROL 状态]** 复选框。

   1. 选择卡片移动到此列时应用到该卡片的状态。

      ![列的状态](assets/boards-column-status.png)

      还会显示已连接信息卡的状态转换选项。 （状态翻译不适用于临时信息卡。） 这些选项决定应用于中任务或问题的自定义状态 [!DNL Workfront] 将已连接的卡片移动到此列时。

   1. 选择 [!UICONTROL **自定义**] 适用于任务和问题的卡的状态。

      将信息卡移动到此列时， [!DNL Workfront] 首先尝试应用自定义状态（例如，已解决）。 如果该卡无法使用选定的自定义状态，系统将提示您选择与系统状态对应的其他状态（从上面的步骤b）。 有关状态的更多信息，请参阅 [状态概述](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      此外，如果所连接任务或问题的状态更改为列策略中设置的自定义或系统状态，信息卡会自动移至列。

1. （可选）为卡片被分配人设置值：

   1. 选择 **[!UICONTROL 被分派人]** 复选框。
   1. 选择操作。

      * **[!UICONTROL 添加被分派人]：** 当信息卡移动到此列时，您选择的被分配人会添加到信息卡上的现有被分配人列表中。
      * **[!UICONTROL 覆盖被分派人]：** 您选择的被分配人将覆盖所有其他被分配人，并在信息卡移至此列时成为该信息卡上的唯一被分配人。

   1. 单击 [!UICONTROL **添加工作**] 和搜索用户。 从搜索结果中选择被分配人。 所有Workfront用户和团队都可以选择。

      ![列的被分派人](assets/boards-column-assignees.png)

1. （可选）设置卡片标记的值：

   1. 选择 **[!UICONTROL 卡片]** 复选框。
   1. 选择操作。

      * **[!UICONTROL 在标记上添加]：** 将信息卡移动到此列时，您选择的标记会添加到信息卡上的现有标记列表中。
      * **[!UICONTROL 覆盖标记]：** 您选择的标记将覆盖所有其他标记，并在卡片移至此列时成为卡片上的唯一标记。

   1. 从下拉列表中选择标记。 仅已在中创建标记 [!UICONTROL 标记管理器] 可供选择。 有关添加新标记的信息，请参阅 [添加标记](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![列的标记](assets/boards-column-tags.png)

1. 启用 **[!UICONTROL 工作进行中限制]** 策略来限制可添加到列中的卡片的数量。 然后，在 **[!UICONTROL 设置限制]** 字段。

   ![列的WIP限制](assets/boards-wip-limit-in-column.png)

   有关更多信息，请参阅 [管理展示板上的正在进行的工作(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 单击 **[!UICONTROL 关闭]** 以退出“设置”区域并查看列及其卡片。
