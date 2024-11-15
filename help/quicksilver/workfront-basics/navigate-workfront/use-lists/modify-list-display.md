---
navigation-topic: use-lists
title: 修改列表的显示方式
description: 在 [!DNL Adobe Workfront]中，您可以自定义列表的显示方式。 查看列表的其他用户看不到您的更改。
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 修改列表的显示方式

<!--Audited: 11/2024-->

在[!DNL Adobe Workfront]中，您可以自定义列表的显示方式。 查看列表的其他用户看不到您的更改。

您可以进行以下自定义：

* 显示的项目数
* 列宽或顺序
* 分组是展开还是折叠

>[!NOTE]
>
>当您注销[!DNL Workfront]或关闭浏览器时，将还原您所做的上述显示更改。 这些更改也可能会在8小时后还原。

除了上述临时自定义之外，您还可以调整列表排序所依据的列，即使在您注销或关闭浏览器之后，[!DNL Workfront]仍会保留哪些列。 但是，如果有人编辑列表视图中的排序选项，则不会保留以前的排序选择。

有关修改列表中显示的信息的信息，请参阅[报表元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>参与者或更高版本 </p></li>
   </ul>

<p>当前：</p>
   <ul><li><p>请求或更高版本</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL视图]对列表所在区域的访问权限</p> <p>例如，要修改项目的视图，您需要具有[！UICONTROL视图]的项目访问权限。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL视图]或应用于列表的视图的更高权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改列表

1. 转到[!DNL Workfront]中要修改的列表。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. （可选且视情况而定）如果列表中的分组已折叠，并且您想查看更多信息，请单击所需分组以展开列表并显示其中列出的信息。

   或

   要展开所有分组，请单击列标题中复选框右侧的箭头。

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. （可选且有条件）如果要在屏幕上显示特定数量的项，请单击屏幕右下角的&#x200B;**[!UICONTROL Showing]**&#x200B;下拉菜单，然后选择以显示&#x200B;**100**、**250**、**500**、**[!UICONTROL All]**&#x200B;或&#x200B;**2000**&#x200B;项。

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >默认情况下，将为更新的列表显示2,000个项目，为旧版列表显示100个项目。 如果列表包含2,000多个项目，则无法在一个页面上显示所有项目。
   >
   >
   >为了在对象包含格式化文本字段的大型列表中获得最佳性能，我们建议将此数字限制为250。
   >
   >
   >有关2种列表类型的详细信息，请参阅[在 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)中开始使用列表[更新列表与旧列表之间的差异](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated)一节。

   列表的结果按页面分页，以显示每页选定的项目数。 通过单击向后和向前箭头或选择特定页面，您可以访问其他页面上的结果。

1. 要调整列宽，请将鼠标悬停在分隔两列的线条上，然后单击以将其拖动到所需的宽度。

   列会调整大小，直到您在浏览器上清除缓存或再次手动调整其大小为止。

1. 要重新排序列表中的列，请将鼠标悬停在列标题上以显示抓手工具，然后单击以将列拖动到要显示的位置。

   列的位置会一直保存，直到您刷新页面为止。

   有关自定义列表中列的宽度和顺序的更多信息，请参阅项目[修改列宽度和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

1. 要调整列表的排序顺序，请单击列标题将其选中，然后在键盘上按住CMD键（在[!DNL Mac]上）或CTRL键（在[!DNL Windows]上），并选择最多2个附加列标题以按它们排序。

   该列表按所选列的顺序排序。

   您对列表所做的所有修改都会立即保存。

   >[!NOTE]
   >
   >如果您在[!UICONTROL 设置]中的[!UICONTROL 组]区域对组进行排序，则在更改列表的排序方式时，组及其子组的层次结构视图不会分解，子组将与其父组保持一致。 该列表首先按顶级组排序。 然后，在每个父组下，位于同一级别的子组列表将一起排序。
