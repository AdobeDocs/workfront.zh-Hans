---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 使用卡片列表
description: 您可以在工作流中创建卡列表，并将卡添加到小版本中。
author: Lisa
feature: Agile
source-git-commit: 96819e5d81a063ad623350a0a75428629d6f7b6d
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 使用卡片列表

{{highlighted-preview-article-level}}

您可以在工作流中创建卡列表，并将卡添加到小版本中。

卡列表可用作工作流的积压工作。

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

## 将信息卡添加到信息卡列表

{{step1-to-boards}}

1. 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 单击 [!UICONTROL **卡片列表**] 选项卡。
1. 单击 [!UICONTROL **添加卡片**].
1. 在 [!UICONTROL **创建/编辑信息卡**] 对话框，添加以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL名称]</strong></td> 
      <td>卡片的名称。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL描述]</strong></td> 
      <td>卡的描述。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL估计]</strong></td> 
      <td>卡片的预计完成小时数。 这只是手动输入。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL状态]</strong></td> 
      <td>选择卡的状态。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL迭代]</strong></td> 
      <td>选择要将卡分配到的小版本。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL任务负责人]</strong></td> 
      <td><p>要分配信息卡，请开始在搜索字段中键入名称，然后在信息卡显示在列表中时将其选中。 您可以添加个人和团队，并且可以为信息卡分配多个人员或团队。</p><p>受分配者必须是工作流中的成员，否则他们不会显示在选择列表中。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 单击&#x200B;[!UICONTROL **保存**]。
1. 继续添加信息卡，直到您生成信息卡列表。

## 查看卡片

要在单个列表中查看工作流的所有信息卡，请单击 [!UICONTROL **列表视图**] 选项卡。

要查看按小版本分组的工作流的所有卡，请单击 [!UICONTROL **迭代视图**]. 计划外卡片显示在其自己的组中。

要编辑现有信息卡，请在列表中选择该信息卡，然后单击 [!UICONTROL **编辑**].

要删除信息卡，请在列表中选择该信息卡，然后单击 [!UICONTROL **删除**].

### 筛选卡片

卡只能从迭代展示板存档。 存档信息卡后，信息卡不会显示在信息卡列表中，除非您进行过滤以显示已存档的信息卡。 有关存档信息卡的信息，请参阅 [从展示板中删除或存档信息卡](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. 访问工作流的卡列表。
1. 单击 [!UICONTROL **过滤器**] 选择 [!UICONTROL **全部**], [!UICONTROL **活动卡**]&#x200B;或 [!UICONTROL **存档的卡片**].

   当在卡片列表中应用除默认值以外的过滤器时，过滤器图标上会显示一个指示器 ![已应用过滤器](assets/boards-filterapplied-30x30.png).

### 在卡片列表中搜索

1. 访问工作流的卡列表。
1. 单击 [!UICONTROL **搜索**] 并键入搜索词。 然后，按Enter。

   将显示包含搜索词的所有卡片。
单击X以清除搜索。

   ![在展示板中搜索信息卡](assets/boards-searchbox.png)

## 向小版本添加卡

>[!NOTE]
>
>必须先创建小版本，然后才能向其添加卡片。 有关信息，请参阅 [在工作流中创建小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. 访问工作流的卡列表。
1. 选择 [!UICONTROL **迭代视图**] 查看哪些卡被分配到小版本以及哪些卡是计划外的。
1. 在列表中选择计划外卡片，然后单击 [!UICONTROL **编辑**].
1. 在 [!UICONTROL **迭代**] 字段。
1. 如果您使用文章点，请在 [!UICONTROL **估计**] 字段。
1. 单击&#x200B;[!UICONTROL **保存**]。

   卡片将移至小版本，小版本量度反映卡片和点数。

   您还可以将卡从计划外卡片组拖放到小版本中，或单击 [!UICONTROL **添加卡片**] 向小版本中添加新卡。

>[!TIP]
>
>如果已创建迭代流程板，则卡列表上的所有计划外卡都将显示在 [!UICONTROL 积压] 列。 当信息卡移入另一列时，它将成为活动小版本的一部分。 您添加到卡片列表中小版本的卡片将根据其状态添加到列中。

