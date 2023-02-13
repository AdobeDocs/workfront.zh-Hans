---
navigation-topic: use-lists
title: 修改列表的显示方式
description: 在 [!DNL Adobe Workfront]，您可以自定义列表的显示方式。 查看列表的其他用户看不到您所做的更改。
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 修改列表的显示方式

在 [!DNL Adobe Workfront]，您可以自定义列表的显示方式。 查看列表的其他用户看不到您所做的更改。

您可以进行以下自定义：

* 显示的项目数
* 列宽或顺序
* 是展开还是折叠分组

>[!NOTE]
>
>当您注销时，您所做的上述显示更改将会恢复 [!DNL Workfront] 或关闭浏览器。 这些更改也可能会在8小时后恢复。

除了上述临时自定义之外，您还可以调整列表排序依据的列， [!DNL Workfront] 保留，即使在您注销或关闭浏览器后也是如此。 但是，如果某人编辑列表视图中的排序选项，则不会保留以前的排序选项。

有关修改列表中显示的信息的信息，请参阅 [报表元素：过滤器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL视图]对列表所在区域的访问</p> <p>例如，要修改项目视图，您需要[!UICONTROL视图]对“项目”的访问权限。</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。<br>有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL视图]或对应用于列表的视图的更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 修改列表的显示方式

1. 转到 [!DNL Workfront] 要修改的选件。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. （可选和视情况而定）如果折叠了列表中的分组，并且您想要查看更多信息，请单击所需的分组以展开列表并显示其中列出的信息。

   或

   要展开所有分组，请单击列标题中复选框右侧的箭头。

   ![expand_groups__1_.png](assets/expand-groupings--1--350x227.png)

1. （可选和视情况而定）如果要在屏幕上显示特定数量的项目，请单击 **[!UICONTROL 显示]** 下角的下拉菜单，然后选择以显示 **100**, **250**, **500**, **[!UICONTROL 全部]**&#x200B;或 **2000年** 项目。

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >默认情况下，更新列表会显示2,000个项目，旧列表会显示100个项目。 如果列表包含的项目超过2,000个，则无法在一个页面上显示所有项目。
   >
   >
   >为了在对象包含格式化文本字段的大列表中获得最佳性能，我们建议将此数字限制为250。
   >
   >
   >有关2个列表类型的更多信息，请参阅部分 [更新列表与旧版列表之间的差异](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 在文章中 [开始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   对列表结果进行分页，以显示每页选定的项目数。 您可以通过单击向后和向前箭头或选择特定页面，访问其他页面上的结果。

1. 要调整列宽，请将鼠标悬停在分隔2列的线条上，然后单击以将其拖动到所需的宽度。

   在您在浏览器上清除缓存之前，或在您再次手动调整缓存大小之前，会调整列的大小。

1. 要对列表中的列重新排序，请将鼠标悬停在列标题上以显示抓手工具，然后单击以将列拖动到要显示的位置。

   列的位置会保存，直到您刷新页面为止。\
   有关自定义列表中列的宽度和顺序的详细信息，请参阅文章 [修改列宽和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. 要调整列表的排序顺序，请单击列标题以将其选中，然后按住CMD键(在 [!DNL Mac])或CTRL键(在 [!DNL Windows])，并选择最多2个附加的列标题以按它们进行排序。

   该列表按所选列的顺序进行排序。

   您对列表所做的所有修改会立即保存。

   >[!NOTE]
   >
   >如果您在 [!UICONTROL 群组] 区域 [!UICONTROL 设置]，则在更改列表排序方式时，组及其子组的层次结构视图不会被划分 — 子组将保留在其父组中。 列表首先按顶级组排序。 然后，在每个父组下，同一级别的子组列表将一起排序。
