---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 在工作流中创建迭代
description: 迭代是为完成工作而保留的设定时间。 某些敏捷团队可能会将开发周期称为冲刺。
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 563e0f443ecef9ee99e9f9bfb5a0d579aa50cef4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 在工作流中创建迭代

{{highlighted-preview}}

迭代是为完成工作而保留的设定时间。 某些敏捷团队可能会将开发周期称为冲刺。

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

## 在工作流中创建迭代

{{step1-to-boards}}

1. 打开要添加小版本的工作流。 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 使用以下方法之一创建迭代：

   * 在“信息卡列表”选项卡的迭代视图中，单击 [!UICONTROL **创建迭代**].
   * 在“卡片列表”选项卡的列表视图中，单击 [!UICONTROL **创建迭代**].
   * 在“展示板”选项卡上，单击 [!UICONTROL **添加展示板**] 并选择 [!UICONTROL **迭代过程**] 作为展示板模板。 然后，打开迭代板并单击 [!UICONTROL **配置迭代**].

1. 在“小版本详细信息”对话框中，添加以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[！UICONTROL迭代名称]</strong></td> 
      <td>迭代的名称，如“Sprint 1”。</td> 
     </tr> 
     <tr> 
      <td><strong>[！UICONTROL迭代长度]</strong></td> 
      <td>迭代的长度，以天、周或月为单位。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL开始日期]</strong></td> 
      <td>迭代开始的日期。 根据迭代长度自动输入结束日期。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;[!UICONTROL **保存**]。

   迭代现在显示在卡片列表的迭代视图中，并显示在迭代展示板上的量度区域中。

   要将信息卡添加到迭代，请参阅 [使用卡片列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## 编辑现有迭代

1. 要打开工作流，请单击 [!UICONTROL **查看工作流**].
1. 使用以下方法之一打开迭代：

   * 在“卡片列表”选项卡的迭代视图中，单击 [!UICONTROL **迭代详细信息**] 图标 ![迭代详细信息](assets/iteration-details-button.png).
   * 在迭代板上，单击 [!UICONTROL **迭代详细信息**] 图标 ![迭代详细信息](assets/iteration-details-button.png) 在右上角的量度区域中。

1. 在 [!UICONTROL 迭代配置] 面板，根据需要编辑小版本。
1. 要更改迭代名称，请展开 [!UICONTROL **迭代详细信息**].

   迭代开始后，您只能更改迭代名称，而不能更改日期或迭代长度。

1. <span class="preview">要将目标添加到迭代，请展开 [!UICONTROL **目标**].</span>
1. <span class="preview">单击 [!UICONTROL **添加目标**]，并键入目标名称。</span>

   <span class="preview">当目标在迭代过程中完成时，您可以选中复选框以将其标记为完成，或单击 **删除** 图标 ![“删除”图标](assets/delete.png) 以删除目标。 迭代右上角的量度区域显示了存在多少个目标和已完成的目标数。</span>

<!--
<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## 删除迭代

1. 单击 [!UICONTROL **信息卡列表**] 选项卡，并打开开发周期视图。
1. 单击 **删除** 图标 ![“删除”图标](assets/delete.png) 在迭代旁边。
1. 单击 [!UICONTROL **删除迭代**] 确认消息上。
