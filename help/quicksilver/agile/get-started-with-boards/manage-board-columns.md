---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理展示板列
description: 默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列，以及删除您不需要的任何列。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: df0e23de7ed84d8c13b60866e1814fe19a877c0b
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# 管理展示板列

默认情况下，新展示板包含三列。 您可以添加更多列、更改列的顺序、重命名列，以及删除您不需要的任何列。

列设置包括策略，利用策略可定义信息卡在移入该列后所发生情况的选项。

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

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 向展示板添加列

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 展示板]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 **[!UICONTROL 添加列]** 列的右侧。
1. 在新列中，键入名称并单击 **[!UICONTROL 添加列]**.

   ![添加新列](assets/boards-add-column.png)

>[!TIP]
>
>要添加进气列，请参阅 [向展示板添加进气柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 对展示板上的列重新排序

1. 访问展示板。
1. 将列拖放到正确的顺序中。 在将列拖至其他位置之前，请务必选择列的顶部。

   ![拖放列](assets/boards-dragdropcolumn.png)

## 重命名展示板列

1. 访问展示板。
1. 单击列名称，键入新名称，然后按Enter。

   或

   单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 编辑]**. 在“设置”区域的 **[!UICONTROL 列名称]** ，然后单击 **[!UICONTROL 关闭]**.

## 删除展示板列

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 删除]**.

   >[!NOTE]
   >
   >无法删除包含卡（包括已存档的卡）的列。 如果尝试删除包含卡的列，则必须为这些卡选择另一列。

## 显示卡计数

您可以使用配置设置来显示每列的信息卡数量。

如果对列使用WIP限制，则不会添加单独的卡片计数器。 有关WIP限制的详细信息，请参阅 [管理 [!UICONTROL 正在进行的工作] 展示板上的(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 访问展示板。
1. 单击 **[!UICONTROL 配置]** 打开“配置”面板。
1. 展开 **[!UICONTROL 列]**.
1. 打开 **[!UICONTROL 显示列卡计数]**.

   ![打开卡计数器](assets/display-card-count.png)

   卡片计数器显示在每列的顶部。

1. 单击 **[!UICONTROL 隐藏配置]** 关闭 [!UICONTROL 配置] 的上界。

## 定义列设置和策略

1. 访问展示板。
1. 单击 **[!UICONTROL 更多]** 菜单 ![“更多”菜单](assets/more-icon-spectrum.png) ，然后选择 **[!UICONTROL 编辑]**.

   的 [!UICONTROL 设置] 中。 的 **[!UICONTROL 列名称]** 可让您知道要为哪个列定义设置。

1. 启用 **[!UICONTROL 自动更新字段值]** 策略来在信息卡被移动到此列时自动更改某些字段值。

   ![列设置和策略](assets/boards-column-policies-enabled.png)

1. （可选）为卡状态设置值：

   1. 选择 **[!UICONTROL 状态]** 复选框。

   1. 选择要在信息卡移动到此列时应用到的状态。

      ![列的状态](assets/boards-column-status.png)

      此外，还会显示连接卡的状态转换选项。 （状态转换不适用于临时信息卡。） 这些选项可确定应用于中任务或问题的自定义状态 [!DNL Workfront] 将连接的卡移至此列时。

   1. 选择 [!UICONTROL **自定义**] 状态。

      当信息卡被移动到此列时， [!DNL Workfront] 首先尝试应用自定义状态（例如，“已解析”）。 如果所选的自定义状态不适用于该卡，则系统会提示您选择与系统状态对应的其他状态（从上面的步骤b中）。 有关状态的更多信息，请参阅 [状态概述](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      此外，如果连接任务或问题的状态更改为列策略中设置的自定义或系统状态，则卡会自动移至列。

1. （可选）为卡片分配者设置值：

   1. 选择 **[!UICONTROL 受聘者]** 复选框。
   1. 选择一个操作。

      * **[!UICONTROL 在受分配人上添加]:** 将您选择的受分配人移动到此列后，会将其添加到卡上的现有受分配人列表中。
      * **[!UICONTROL 覆盖受分配者]:** 您选择的受分配人将覆盖所有其他受分配人，并在被移动到此列时成为卡片上的唯一受分配人。
   1. 从下拉列表中选择受分配者。 只有董事会成员可供选择。 有关更多信息，请参阅 [在展示板中添加或删除成员](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![列的分配者](assets/boards-column-assignees.png)


1. （可选）为卡片标记设置值：

   1. 选择 **[!UICONTROL 卡片]** 复选框。
   1. 选择一个操作。

      * **[!UICONTROL 添加标记]:** 将您选择的标记移动到此列后，会将其添加到卡片上的现有标记列表。
      * **[!UICONTROL 覆盖标记]:** 您选择的标记会覆盖所有其他标记，并在信息卡移到此列后成为信息卡上的唯一标记。
   1. 从下拉列表中选择标记。 仅已在 [!UICONTROL 标签管理器] 可供选择。 有关添加新标记的信息，请参阅 [添加标记](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![列的标记](assets/boards-column-tags.png)


1. 启用 **[!UICONTROL 正在进行的工作限制]** 策略来限制可添加到列的卡数。 然后，在 **[!UICONTROL 设置限制]** 字段。

   ![列的WIP限制](assets/boards-wip-limit-in-column.png)

   有关更多信息，请参阅 [在展示板上管理在制品(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 单击 **[!UICONTROL 关闭]** 退出“设置”区域，并查看列及其卡片。
