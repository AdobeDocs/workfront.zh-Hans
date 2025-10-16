---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 在工作流中创建迭代
description: 迭代是为完成工作而保留的设定时间。 某些Agile团队可能会将开发周期称为冲刺。
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 在工作流中创建迭代

>[!IMPORTANT]
>
>工作流仅适用于特定的客户组。

迭代是为完成工作而保留的设定时间。 某些Agile团队可能会将开发周期称为冲刺。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p>
   </td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作流中创建迭代

{{step1-to-boards}}

1. 打开要添加小版本的工作流。 要打开工作流，请单击&#x200B;[!UICONTROL **查看工作流**]。
1. 使用以下方法之一创建迭代：

   * 在“卡片列表”选项卡的迭代视图中，单击&#x200B;[!UICONTROL **创建迭代**]。
   * 在“卡片列表”选项卡的列表视图中，单击&#x200B;[!UICONTROL **创建迭代**]。
   * 在“展示板”选项卡上，单击&#x200B;[!UICONTROL **添加展示板**]&#x200B;并选择&#x200B;[!UICONTROL **迭代进程**]&#x200B;作为展示板模板。 然后，打开迭代展示板并单击&#x200B;[!UICONTROL **配置迭代**]。

1. 在“小版本详细信息”对话框中，添加以下信息：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL 迭代名称]</strong></td> 
      <td>迭代的名称，如“Sprint 1”。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL 迭代长度]</strong></td> 
      <td>迭代的长度，以天、周或月为单位。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 开始日期]</strong></td> 
      <td>迭代开始的日期。 根据迭代长度自动输入结束日期。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;[!UICONTROL **保存**]。

   迭代现在显示在卡片列表的迭代视图中，并显示在迭代展示板的量度区域中。

   要将信息卡添加到迭代，请参阅[使用信息卡列表](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)。

## 编辑现有迭代

1. 要打开工作流，请单击&#x200B;[!UICONTROL **查看工作流**]。
1. 使用以下方法之一打开迭代：

   * 在“信息卡列表”选项卡的迭代视图中，单击&#x200B;[!UICONTROL **迭代详细信息**]&#x200B;图标![迭代详细信息](assets/iteration-details-button.png)。
   * 在迭代展示板上，单击右上角量度区域中的&#x200B;[!UICONTROL **迭代详细信息**]&#x200B;图标![迭代详细信息](assets/iteration-details-button.png)。

1. 在[!UICONTROL 迭代配置]面板中，根据需要编辑迭代。
1. 要更改迭代名称，请展开&#x200B;[!UICONTROL **迭代详细信息**]。

   一旦迭代开始，您只能更改迭代名称，而不能更改日期或迭代长度。

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## 删除迭代

1. 单击工作流上的&#x200B;[!UICONTROL **卡片列表**]&#x200B;选项卡并打开迭代视图。
1. 单击迭代旁边的&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。
1. 单击确认消息上的&#x200B;[!UICONTROL **删除迭代**]。
