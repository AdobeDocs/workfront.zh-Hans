---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在讨论区中添加或删除成员
description: 用户必须先作为成员添加到展示板，然后才能查看展示板并分配到信息卡。
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: 03768a0d3a63c7f6adcd11a6cd2e4d093b24f214
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 在讨论区中添加或删除成员

必须将人员和团队作为成员添加到讨论区，然后才能查看讨论区。

默认情况下，展示板的创建者是所有者。 讨论区所有者是唯一可以在“配置”面板中删除该讨论区或更新其筛选器的人员。 只有系统管理员或当前讨论区所有者才能更改讨论区所有者。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> 
   <p>新文档： [！UICONTROL Contributor]或更高版本</p> 
   <p>或</p>
   <p>当前： [！UICONTROL Request]或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将成员添加到讨论区

{{step1-to-boards}}

1. 创建新展示板或编辑现有展示板。 有关信息，请参阅[创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 单击&#x200B;**[!UICONTROL 添加成员]**&#x200B;图标![添加成员](assets/boards-addmember-spectrum-25x25.png)。
1. 在&#x200B;**[!UICONTROL 添加成员]**&#x200B;框中，开始键入名称，然后当名称显示在列表中时将其选定。

   您可以选择单个成员或团队。 如果选择团队，则团队本身会添加到展示板中。

   >[!NOTE]
   >
   >单个用户必须在其团队的访问级别中设置&#x200B;**[!UICONTROL 查看]**&#x200B;或&#x200B;**[!UICONTROL 编辑]**&#x200B;选项，否则他们将无法查看讨论区。


   ![将成员添加到讨论区](assets/boards-add-members.png)

## 从展示板中移除成员

{{step1-to-boards}}

1. 创建新展示板或编辑现有展示板。 有关信息，请参阅[创建或编辑展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 单击&#x200B;**[!UICONTROL 添加成员]**&#x200B;图标![添加成员](assets/boards-addmember-spectrum-25x25.png)。
1. 在&#x200B;**[!UICONTROL 添加成员]**&#x200B;框中，单击人员或团队名称旁边的X以将其从展示板中删除。

   ![从讨论区中删除成员](assets/boards-remove-member-from-board-350x367.png)

   从展示板中移除成员时，不会从分配给他们的任何信息卡中移除成员。 对于连接的信息卡，分配也会在[!DNL Workfront]任务或问题中更新。

   成员只会从此讨论区中移除。 它们不会从属于的其他展示板中删除。

   >[!NOTE]
   >
   >您无法删除讨论区所有者。

## 更改讨论区所有者

>[!NOTE]
>
>只有系统管理员或当前讨论区所有者才能更改讨论区所有者。 一个展示板只能有一个所有者。
>
>可以在基本、追溯和Kanban展示板上更改展示板所有者，但不能更改动态展示板。

1. 访问展示板。
1. 单击讨论区名称旁边的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多菜单](assets/more-icon-spectrum.png)，然后选择&#x200B;**[!UICONTROL 更改讨论区所有者]**。
1. 在“更改展示板所有者”对话框中，搜索并选择想要成为该所有者的用户。

   您无法搜索已经是讨论区成员的用户。 要使现有成员成为所有者，必须先将其从展示板中移除。 将用户设为展示板所有者，会将其添加到展示板。

   只有用户才能成为讨论区所有者。 团队不能是所有者。

1. 单击&#x200B;[!UICONTROL **更新**]。
