---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum展示板上查看和编辑故事信息
description: 在Kanban展示板上查看故事拼贴时，某些信息可用于直接从故事拼贴内联编辑。
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 在[!UICONTROL Scrum]展示板上查看和编辑故事信息

## 了解可以查看和编辑哪些信息

在故事板上查看故事拼贴时，下表中的信息可用。 您可以直接从“故事”拼贴内联编辑大多数信息。

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
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>带有直接指向项目的链接的项目名称<br>当在开发周期上使用敏捷视图时，此链接仅显示在故事中（父任务而非子任务）；当在项目上使用敏捷视图时，不显示此链接。</p> </td> 
   <td>✓ {\f13 } </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>文章的完成点数或小时数以及分配给文章的点数或小时数<br>这些数字用于计算并显示每个文章的[！UICONTROL完成百分比]。</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p>每个故事和问题的[！UICONTROL完成百分比]。<br>迭代的[！UICONTROL完成百分比]是根据每个故事的[！UICONTROL完成百分比]计算的。</p> <p>更新故事或问题的[！UICONTROL完成百分比]时，您可以选择介于0和100之间的任意数字。</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p>故事被分派到的用户</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p>图块的颜色或类别</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p>可能已通过修改Agile视图而添加到Agile视图的任何其他字段（包括自定义字段），如[！UICONTROL Adobe Workfront]</a>中的<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">视图概述中的“创建和自定义[！UICONTROL Agile]视图”中所述。</p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>编辑对任务或问题的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 查看和编辑文章拼贴上的信息

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 团队]**。

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。

1. 转到[!UICONTROL Scrum]敏捷故事板。
1. 展开[!UICONTROL 文章]拼贴以查看与文章关联的所有字段。

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. （可选）要编辑字段，请单击该字段，然后进行任何更改。

   您必须对任务或问题具有[!UICONTROL 编辑]权限才能编辑故事拼贴。

>[!NOTE]
>
>要更改[!UICONTROL 完成百分比]，必须键入一个介于0和100之间的数字。 该字段不是可移动的滑块。
