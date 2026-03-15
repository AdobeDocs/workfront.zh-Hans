---
content-type: reference
navigation-topic: boards
title: 将Agile小组看板卡迁移到Workfront看板
description: 您可以将工作物料从Agile团队看板面板迁移到新的或现有的Workfront看板。
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 4%

---

# 将Agile团队看板卡迁移到Workfront展示板

您可以将工作物料从Agile团队看板面板迁移到新的或现有的Workfront看板。 运行迁移时，看板面板中的所有卡都将复制到Workfront看板。 您不得选择特定卡。

卡片在Workfront委员会上的放置是根据列政策进行的。 (例如，策略可以将状态为“进行中”的所有信息卡移到特定列。 有关列策略的更多信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。)如果没有策略或信息卡与策略不匹配，信息卡将置于展示板最左侧的列中。 此时，旧版展示板的“积压”列中的信息卡不会添加到Workfront展示板。

看板卡不会从Agile团队看板中删除，并且卡状态更改将同步到两个看板。 您可以使两个展示板保持活动状态，直到您准备好切换到Workfront展示板。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>参与者或更高</p> 
   <p>请求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的详细信息，请参阅[Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将看板卡迁移到新展示板

{{step1-to-team}}

1. 访问看板面板。
1. 单击&#x200B;[!UICONTROL **添加到展示板**]，然后选择&#x200B;[!UICONTROL **新展示板**]。
1. 在[!UICONTROL 添加到新展示板]对话框中，键入新展示板的名称（自动显示当前[!UICONTROL 看板]展示板的名称），然后单击&#x200B;[!UICONTROL **添加**]。

   ![将看板卡添加到新展示板](assets/add-kanban-cards-to-new-board-dialog.png)

1. （可选）在显示的成功消息中，单击链接以打开新展示板。

## 将看板卡迁移到现有展示板

{{step1-to-team}}

1. 访问看板面板。
1. 单击&#x200B;[!UICONTROL **添加到讨论区**]&#x200B;并选择&#x200B;[!UICONTROL **现有讨论区**]。
1. 在[!UICONTROL 添加到现有展示板]对话框中，搜索并选择要将信息卡迁移到的展示板。 然后，单击&#x200B;[!UICONTROL **添加**]。

   ![将看板卡添加到现有展示板](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （可选）在显示的成功消息中，单击链接以打开展示板。
