---
content-type: reference
navigation-topic: boards
title: 将敏捷团队Kanban卡迁移到Workfront展示板
description: 您可以将工作项从Agile团队Kanban展示板迁移到新的或现有的Workfront展示板。
author: Lisa
feature: Agile
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# 将敏捷团队Kanban卡迁移到Workfront展示板

您可以将工作项从Agile团队Kanban展示板迁移到新的或现有的Workfront展示板。 运行迁移时，Kanban展示板上的所有信息卡都会复制到Workfront展示板。 您不得选择特定卡。

在Workfront展示板上置入信息卡取决于列策略。 (例如，策略可以将所有状态为“进行中”的信息卡移动到特定列。 有关列策略的详细信息，请参见 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) 如果没有策略或信息卡与策略不匹配，则信息卡会放置在展示板最左侧的列中。 目前，旧版展示板上积压工作列中的信息卡未添加到Workfront展示板中。

未从敏捷团队Kanban展示板中删除信息卡，信息卡状态更改将同步到两个展示板。 在准备好切换到Workfront展示板之前，您可以保持两个展示板处于活动状态。

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
   <td> <p>任何</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td>
   <td> <p>[！UICONTROL Request]或更高版本</p> </td>
  </tr>
 </tbody>
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 将Kanban卡迁移到新展示板

{{step1-to-team}}

1. 访问Kanban板。
1. 单击 [!UICONTROL **添加到展示板**] 并选择 [!UICONTROL **新讨论区**].
1. 在 [!UICONTROL 添加到新讨论区] 对话框，键入新讨论区的名称（当前讨论区的名称） [!UICONTROL Kanban] 板会自动显示)，然后单击 [!UICONTROL **添加**].

   ![将Kanban卡添加到新讨论区](assets/add-kanban-cards-to-new-board-dialog.png)

1. （可选）在显示的成功消息上，单击链接以打开新展示板。

## 将Kanban卡迁移到现有板

{{step1-to-team}}

1. 访问Kanban板。
1. 单击 [!UICONTROL **添加到展示板**] 并选择 [!UICONTROL **现有讨论区**].
1. 在 [!UICONTROL 添加到现有展示板] 对话框，搜索并选择要将信息卡迁移到的展示板。 然后，单击 [!UICONTROL **添加**].

   ![将Kanban卡添加到现有展示板](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （可选）在显示的成功消息上，单击链接以打开展示板。
