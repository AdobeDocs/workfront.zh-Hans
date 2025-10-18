---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 编辑故事信息
description: 在Kanban展示板上查看故事拼贴时，某些信息可用于直接从故事拼贴内联编辑。
author: Jenny
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 编辑故事信息

## 了解可以查看和编辑哪些信息 {#understand-what-information-can-be-viewed-and-edited}

在[!UICONTROL Kanban]展示板上查看故事拼贴时，下表中的信息可用。 您可以直接从“故事”拼贴内联编辑大多数信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>信息</strong> </th> 
   <th><strong>可见</strong> </th> 
   <th><strong>可编辑内联</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>带有直接指向任务或问题的链接的故事名称</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>带有直接项目链接的项目名称</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>文章的完成点数或小时数以及分配给文章的点数或小时数<br>这些数字用于计算和显示每个文章的完成百分比。</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>每个故事和问题的[!UICONTROL 完成百分比]。<br>[!UICONTROL 迭代的完成百分比]是根据每个故事的[!UICONTROL 完成百分比]计算的。<br></p> <p>更新故事或问题的[!UICONTROL 完成百分比]时，您可以选择介于0和100之间的任意数字。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>故事被分派到的用户</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>图块的颜色或类别</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>通过修改Agile视图可能已添加到Agile视图的任何其他字段（包括自定义字段），如<a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">中的[!DNL Adobe Workfront]</a>视图概述中的“创建和自定义Agile视图”中所述</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作或更高</p> </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看和编辑文章拼贴上的信息

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Kanban团队或在搜索栏中搜索团队。

1. 转到[!UICONTROL Kanban]展示板。
1. 展开文章拼贴可查看与文章关联的所有字段。

   ![故事卡](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. （可选）要编辑字段，请单击该字段，然后进行任何更改。
您必须对任务或问题具有[!UICONTROL 编辑]权限才能编辑故事拼贴。
有关每个字段及其是否可以编辑的详细信息，请参阅[了解可以查看和编辑哪些信息](#understand-what-information-can-be-viewed-and-edited)。

>[!NOTE]
>
>要更改[!UICONTROL 完成百分比]，必须键入一个介于0和100之间的数字。 该字段不是可移动的滑块。
