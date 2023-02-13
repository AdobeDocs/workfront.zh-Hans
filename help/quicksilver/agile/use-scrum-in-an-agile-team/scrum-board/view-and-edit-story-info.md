---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum展示板上查看和编辑文章信息
description: 在看板板上查看文章拼贴时，某些信息可直接从文章拼贴内联编辑。
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# 在 [!UICONTROL Scrum] 展示板

## 了解哪些信息可以查看和编辑

在文章板上查看文章拼贴时，可以查看下表中的信息。 您可以直接从文章拼贴中在内联编辑大多数信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>信息</strong> </th> 
   <th><strong>可见</strong> </th> 
   <th><strong>可编辑的内联</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>带有直接指向任务或问题的链接的文章名称</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>带有直接指向项目的链接的项目名称<br>当对迭代使用敏捷视图时，此链接仅在文章（父任务，而非子任务）中显示；在项目上使用敏捷视图时，不会显示该视图。</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>文章完成的点数或小时数以及分配给文章的点数或小时数<br>这些数字用于计算和显示每个文章的[!UICONTROL完成百分比]。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>每个故事和问题对应的[!UICONTROL完成百分比]。<br>小版本的[!UICONTROL百分比完成]是根据每个文章的[!UICONTROL百分比完成]计算的。</p> <p>在更新文章或问题的[!UICONTROL完成百分比]时，您可以选择介于0到100之间的任意数字。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>将故事分配给谁</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>图块的颜色或类别</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>通过修改敏捷视图可能已添加到敏捷视图的任何其他字段（包括自定义字段），如 <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!UICONTROL Adobe Workfront]中的视图概述</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>编辑对任务或问题的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 查看和编辑文章拼贴中的信息

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

1. 在左侧面板中，选择 **[!UICONTROL 迭代]** 选择特定小版本，或选择 **[!UICONTROL 当前迭代]**.

1. 转到 [!UICONTROL Scrum] 敏捷故事板。
1. 展开 [!UICONTROL 故事] 拼贴可查看与文章关联的所有字段。

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. （可选）要编辑字段，请单击该字段，然后进行任何更改。

   您必须 [!UICONTROL 编辑] 任务或问题的权限，以编辑文章拼贴。

>[!NOTE]
>
>要更改 [!UICONTROL 完成百分比]，则必须键入一个介于0到100之间的数字。 该字段不是可移动的滑块。
