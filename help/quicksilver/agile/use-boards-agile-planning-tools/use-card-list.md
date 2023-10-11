---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 使用信息卡列表
description: 您可以在工作流中创建信息卡列表并将信息卡添加到迭代。
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: d44eb048103e469bc072cc5287947fea471668b3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# 使用信息卡列表

>[!IMPORTANT]
>
>并非所有客户都可以使用工作流。

您可以在工作流中创建信息卡列表并将信息卡添加到迭代。

信息卡列表可用作工作流的积压工作。

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

## 将信息卡添加到信息卡列表

{{step1-to-boards}}

1. 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 单击 [!UICONTROL **信息卡列表**] 选项卡。
1. 单击 [!UICONTROL **添加信息卡**].
1. 在 [!UICONTROL **创建/编辑信息卡**] 对话框，添加以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[！UICONTROL名称]</strong></td> 
      <td>卡的名称。</td> 
     </tr> 
     <tr> 
      <td><strong>[！UICONTROL描述]</strong></td> 
      <td>信息卡的描述。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL估计]</strong></td> 
      <td>预计完成信息卡的小时数。 这只是一个手动输入。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL状态]</strong></td> 
      <td>选择卡的状态。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL迭代]</strong></td> 
      <td>选择要为其分配信息卡的迭代。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL被分派人]</strong></td> 
      <td><p>要分配卡，请在搜索字段中开始键入名称，然后在此卡显示在列表中时将其选定。 您可以同时添加个人和团队，也可以将多个人员或团队分配给信息卡。</p><p>被分派人必须是工作流中的成员，否则他们不会出现在选择列表中。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 单击&#x200B;[!UICONTROL **保存**]。
1. 继续添加信息卡，直到构建信息卡列表。

## 查看卡片

要在单个列表中查看工作流的所有卡片，请单击 [!UICONTROL **列表视图**] 在“信息卡列表”选项卡上。

要查看按迭代分组的工作流的所有卡片，请单击 [!UICONTROL **迭代视图**]. 计划外的信息卡会显示在他们自己的组中。

要编辑现有信息卡，请在列表中选择该信息卡并单击 [!UICONTROL **编辑**].

要删除某个信息卡，请在列表中选择该信息卡并单击 [!UICONTROL **删除**].

### 过滤卡片

信息卡只能从迭代展示板存档。 存档信息卡时，除非您进行筛选以显示存档的信息卡，否则它不会显示在信息卡列表中。 有关存档信息卡的信息，请参阅 [从展示板中删除或存档信息卡](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. 访问工作流的卡列表。
1. 单击 [!UICONTROL **筛选**] 并选择 [!UICONTROL **全部**]， [!UICONTROL **活动信息卡**]，或 [!UICONTROL **已存档的信息卡**].

   当在信息卡列表上应用默认以外的过滤器时，过滤器图标上会显示指示器 ![已应用筛选器](assets/boards-filterapplied-30x30.png).

### 在信息卡列表中搜索

1. 访问工作流的卡列表。
1. 单击 [!UICONTROL **Search**] 并键入搜索词。 然后，按Enter。

   将显示包含搜索词的所有卡片。
单击X清除搜索。

   ![在展示板中搜索卡片](assets/boards-searchbox.png)

## 将信息卡添加到迭代

>[!NOTE]
>
>必须先创建迭代，然后才能向其添加卡片。 有关信息，请参阅 [在工作流中创建迭代](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. 访问工作流的卡列表。
1. 选择 [!UICONTROL **迭代视图**] 查看哪些信息卡已分配给开发周期，哪些是计划外的。
1. 在列表中选择一个未计划的卡片并单击 [!UICONTROL **编辑**].
1. 选择迭代 [!UICONTROL **迭代**] 字段。
1. 如果您使用故事点，请在 [!UICONTROL **估计**] 字段。
1. 单击&#x200B;[!UICONTROL **保存**]。

   信息卡会被移动到迭代，迭代量度反映信息卡和点的数量。

   您还可以将信息卡从“未计划的信息卡”组拖放到开发周期中，或单击 [!UICONTROL **添加信息卡**] 以向开发周期中添加新信息卡。

>[!TIP]
>
>如果已创建迭代流程展示板，则信息卡列表中的所有未计划信息卡都会显示在 [!UICONTROL 积压] 列。 将信息卡移动到另一列时，它将成为活动迭代的一部分。 添加到信息卡列表中迭代的信息卡会根据其状态添加到列。
