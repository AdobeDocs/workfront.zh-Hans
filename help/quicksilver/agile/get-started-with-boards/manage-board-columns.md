---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理展示板列
description: 默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列以及删除不需要的任何列。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 05cac2441474e0f6ecf18aa777a5a66fefb2dba8
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# 管理展示板列

默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列以及删除不需要的任何列。

列设置包括策略，这些策略允许您定义卡片被移动到该列时卡片所发生的变化的选项。

有关按列对卡片进行排序的信息，请参见 [在展示板中过滤和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 向展示板添加列

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 讨论区]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 添加列]** 位于现有列的右侧。
1. 在新列中，键入名称并单击 **[!UICONTROL 添加列]**.

   ![添加新列](assets/boards-add-column.png)

>[!TIP]
>
>要添加引入列，请参见 [向展示板添加引入列](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 重新排序展示板上的列

1. 访问展示板。
1. 按正确的顺序拖放列。 在将该列拖到其他位置之前，请务必选择列的顶部。

   ![拖放列](assets/boards-dragdropcolumn.png)

## 重命名展示板列

1. 访问展示板。
1. 单击列名，键入新名称，然后按Enter。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) 在列中选择 **[!UICONTROL 编辑]**. 在“设置”区域中，在 **[!UICONTROL 列名称]** 字段，然后单击 **[!UICONTROL 关闭]**.

## 删除展示板列

从展示板中删除列时，无法恢复该列。

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) 列上，并选择 **[!UICONTROL 删除]**.

   >[!NOTE]
   >
   >无法删除包含信息卡（包括已存档的信息卡）的列。 如果尝试删除包含信息卡的列，则必须为这些信息卡选择另一列。

## 显示卡计数

您可以使用配置设置显示每列中的卡片数量。

如果对列使用WIP限制，则不会添加单独的卡片计数器。 有关WIP限制的详细信息，请参阅 [管理 [!UICONTROL 工作进行中] 主板上的(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 访问展示板。
1. 单击 **[!UICONTROL 配置]** ，打开“配置”面板。
1. 展开 **[!UICONTROL 列]**.
1. 打开 **[!UICONTROL 显示列卡片计数]**.

   ![打开卡片计数器](assets/display-card-count.png)

   卡片计数器显示在每列的顶部。

1. 单击 **[!UICONTROL 隐藏配置]** 关闭 [!UICONTROL 配置] 面板。

## 定义列设置和策略

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) 列上，并选择 **[!UICONTROL 编辑]**.

   此 [!UICONTROL 设置] 区域显示。 此 **[!UICONTROL 列名称]** 让您知道要为哪一列定义设置。

1. 启用 **[!UICONTROL 自动更新字段值]** 策略，用于在将信息卡移动到此列时自动更改某些字段值。

   ![列设置和策略](assets/boards-column-policies-enabled.png)

1. （可选）设置信息卡状态的值：

   1. 选择 **[!UICONTROL 状态]** 复选框。

   1. 选择信息卡移动到此列时应用于该信息的状态。

      ![列的状态](assets/boards-column-status.png)

      还会显示已连接信息卡的状态转换选项。 （状态转换不适用于临时信息卡。） 这些选项决定应用于中任务或问题的自定义状态 [!DNL Workfront] 将已连接的卡片移动到此列时。

   1. 选择 [!UICONTROL **自定义**] 任务和问题的信息卡要应用的状态。

      将信息卡移动到此列时， [!DNL Workfront] 首先尝试应用自定义状态（例如，已解决）。 如果选定的自定义状态不适用于该卡，系统会提示您选择与系统状态对应的其他状态（从上面的步骤b）。 有关状态的更多信息，请参阅 [状态概述](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      此外，如果所连接任务或问题的状态更改为列策略中设置的自定义或系统状态，信息卡会自动移动到列。

1. （可选）为卡片被分派人设置值：

   1. 选择 **[!UICONTROL 被分派人]** 复选框。
   1. 选择一个操作。

      * **[!UICONTROL 添加被分派人]：** 当信息卡移动到此列时，您选择的被分配人将被添加到信息卡上的现有被分配人列表中。
      * **[!UICONTROL 覆盖被分派人]：** 您选择的被分配人将覆盖所有其他被分配人，并在信息卡移动到此列时成为信息卡上的唯一被分配人。
   1. 从下拉列表中选择被分配人。 只有董事会成员可以从中进行选择。 有关更多信息，请参阅 [在讨论区中添加或移除成员](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![列的被分派人](assets/boards-column-assignees.png)


1. （可选）设置卡片标记的值：

   1. 选择 **[!UICONTROL 卡片]** 复选框。
   1. 选择一个操作。

      * **[!UICONTROL 在标记上添加]：** 当您将信息卡移动到此列时，您选择的标记会添加到信息卡上的现有标记列表中。
      * **[!UICONTROL 覆盖标记]：** 您选择的标记将覆盖所有其他标记，并在卡片移至此列时成为卡片上的唯一标记。
   1. 从下拉列表中选择标记。 仅已在中创建标记 [!UICONTROL 标记管理器] 可供选择。 有关添加新标记的信息，请参阅 [添加标记](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![列的标记](assets/boards-column-tags.png)


1. 启用 **[!UICONTROL 工作进行中限制]** 用于限制可添加到列中的卡片数量的策略。 然后，在 **[!UICONTROL 设置限制]** 字段。

   ![列的WIP限制](assets/boards-wip-limit-in-column.png)

   有关更多信息，请参阅 [管理展示板上的正在进行的工作(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 单击 **[!UICONTROL 关闭]** 以退出“设置”区域并查看列及其卡片。
