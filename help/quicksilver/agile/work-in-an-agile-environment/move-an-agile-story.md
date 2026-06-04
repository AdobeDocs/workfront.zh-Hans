---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 移动敏捷故事
description: 您可以将敏捷故事移动到不同的迭代（对于Scrum团队）或积压（对于Kanban和Scrum团队）。
author: Courtney
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/gVEWRh4iiYdy6CwzLubaY3GZ4EE5C5diJ-RvsYFFtE4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 343
ht-degree: 6%

---

# 移动敏捷故事

您可以将敏捷故事移动到不同的迭代（对于Scrum团队）或积压（对于Kanban和Scrum团队）。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作版或更高版本</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理对故事的访问</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将故事从迭代或Kanban展示板移动到积压

1. 转到包含要移至积压的项目故事的迭代或Kanban展示板。
1. 单击页面顶部的迭代标题。
1. 在&#x200B;**[!UICONTROL 故事]**&#x200B;选项卡上，选择要移动的故事。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 移至]**。 显示&#x200B;**[!UICONTROL 移至]**&#x200B;对话框。

   ![移动故事对话框](assets/iteration-story-move.png)

1. 选择&#x200B;**team_name的积压**。 在上例中，团队名称为&#x200B;**营销**。

1. 单击&#x200B;**[!UICONTROL 移动]**。

## 将故事移动到其他迭代

如果您是系统管理员或小版本关联的团队的成员，则可以将故事移动到Scrum团队的其他小版本。

>[!NOTE]
>
> **[!UICONTROL 移至]**&#x200B;选项不适用于开发周期中的父故事。 您只能将子任务移动到另一个迭代。


1. 转到包含要移动的故事的迭代。
1. 单击页面顶部的迭代标题。
1. 在&#x200B;**[!UICONTROL 故事]**&#x200B;选项卡上，选择要移动的故事。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 移至]**。 显示&#x200B;**[!UICONTROL 移至]**&#x200B;对话框。

   ![移动故事对话框](assets/iteration-story-move.png)

1. 选择&#x200B;**[!UICONTROL 另一个迭代]**。
1. 在出现的下拉菜单中，选择要将文章移动到的小版本。

   >[!NOTE]
   >
   >工作项[!UICONTROL 计划开始日期]和[!UICONTROL 计划完成日期]受[!UICONTROL 编辑团队]页面上的设置影响。 有关信息，请参阅[配置Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[[!UICONTROL 配置]将工作项添加到迭代时，日期的应用方式](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)部分。

1. 单击&#x200B;**[!UICONTROL 移动]**。
