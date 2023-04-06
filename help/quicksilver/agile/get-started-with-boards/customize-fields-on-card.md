---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 自定义信息卡上显示的字段
description: 您可以通过禁用字段来自定义在信息卡上显示的字段，使其不会显示在完整信息卡或压缩视图中，或者隐藏压缩信息卡视图上的字段。
author: Lisa
feature: Agile
source-git-commit: 48dc1bcbaa5755888c45fdafbd6471c9ee073a45
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 自定义信息卡上显示的字段

默认情况下，所有可用字段都显示在信息卡上（在信息卡打开时显示在完整视图中）和信息卡板上的压缩卡片视图中。 您可以自定义显示哪些字段：

* 禁用字段，使其不会显示在任何视图中
* 在压缩的卡片视图中隐藏字段

如果字段包含值，并且您禁用了该字段，则当您稍后再次启用该字段时，将保留该值。

您还可以显示之前创建的自定义字段。 您无法在展示板中设计和创建新的自定义字段。

>[!NOTE]
>
>您所做的任何字段自定义仅应用于您正在使用的展示板。

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

## 配置信息卡 {#configure-cards}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 展示板]**.
1. 访问展示板。 有关信息，请参阅 [创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 单击 [!UICONTROL **配置**] 打开“配置”面板。
1. 展开 [!UICONTROL **卡片**].

   大多数字段默认处于启用状态。

1. 关闭字段可在两个卡片视图中禁用该字段。
1. 单击隐藏图标 ![隐藏图标](assets/eye-hide-icon.png) 字段旁边，以将其隐藏在缩合视图中。
1. 要显示两个视图中的所有字段，请单击 [!UICONTROL **将所有字段恢复为默认值**].
1. 单击 [!UICONTROL **隐藏配置**] 以关闭“配置”面板。

## 将自定义字段添加到信息卡

连接的信息卡上提供了自定义字段。 它们仅在完整卡片视图中可见，而不在展示板的压缩视图中可见。

>[!NOTE]
>
>在信息卡中添加自定义字段时，信息卡上的数据为只读。

1. 访问展示板并单击 [!UICONTROL **配置**] 打开“配置”面板。
1. 展开 [!UICONTROL **卡片**].
1. 在 [!UICONTROL 卡片字段]，单击 [!UICONTROL **添加自定义字段**].
1. 选择 [!UICONTROL **任务**] 或 [!UICONTROL **问题**].

   此时会显示任务或问题的可用字段类别。 展开类别可查看所有字段。 您还可以搜索字段。

   ![搜索自定义字段](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >以下字段类型无法添加到信息卡：Adobe XD、图像、PDF、视频。

1. 选择字段名称。
1. （可选）单击 **[!UICONTROL 字段值]** 字段来更改此自定义字段。
1. （可选）更改 **[!UICONTROL 字段标签]** 的字段名称。
1. 完成更改后，单击 [!UICONTROL **保存字段**].

   ![自定义字段值和标签](assets/save-custom-field-value-label.png)

   自定义字段将添加到可用字段列表，并且默认启用。 您可以按照 [配置信息卡](customize-fields-on-card.md#configure-cards) 编辑字段，或从所有信息卡中删除该字段。

