---
product-area: projects
navigation-topic: use-the-home-area
title: 使用我的请求小组件
description: 您可以在“我的请求”小组件中提交请求。 您还可以使用过滤器和列自定义构件。
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# 使用我的请求小组件

>[!IMPORTANT]
>
>本文介绍了新的My Requests构件。 您必须启用新的请求体验才能查看新的构件。
>您可以在请求区域中启用新的请求体验。

“我的请求”小组件会显示您已提交的请求。 您可以筛选请求、搜索特定请求或调整列顺序和可见性。 您还可以从“我的请求”小组件创建新请求。

>[!NOTE]
>
>* 加载My Requests小组件后，它最多显示50个请求。 要显示更多请求，请向下滚动列表。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何Workfront或工作流包</p>
   <p>用于访问Workfront Planning请求及其创建的对象的任何Workfront Planning包</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>查看或拥有对您在对话中被标记或需要解决审批的任何对象（项目、任务、问题、文档）的更高访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL 查看]对项目、任务、问题和文档的权限或更高，在这些项目、任务、问题和文档中，您被标记在对话中或需要解决审批问题</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建请求

您可以直接从“我的请求”小组件创建请求。

有关说明，请参阅文章[从主页区域创建工作项和项目](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request)中的[创建请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)部分。

## 复制请求

您可以在“我的请求”小部件中复制请求，对其进行编辑，然后将其作为新请求提交。

有关说明，请参阅[复制并提交请求](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 在“我的请求”小组件中管理请求列表中的信息

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. 单击左上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/lines-main-menu.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. （可选）要管理信息在请求列表中的显示方式，请更新列表的以下视图元素：

   * 视图
   * 筛选条件
   * 列

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   有关管理请求列表中的信息的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。


<!--
 Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>如果贵组织除了Adobe Workfront之外还购买了Workfront Planning，则“我的请求”小组件将同时包含Workfront和Workfront Planning请求。
> 
>* 要仅筛选Workfront请求，请将筛选器设置为&#x200B;**对象类型** > **具有任何** > **问题**。
>* 要仅筛选Workfront Planning请求，请将筛选器设置为&#x200B;**对象类型** > **不包含** > **问题**。

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## 搜索请求

要在“我的请求”小组件中搜索特定请求，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. 在我的请求小部件的右上角附近的搜索栏中，输入要搜索的术语。

   包含术语的请求以橙色突出显示。

1. （可选）要跳转到突出显示的请求，请单击搜索栏中的向上或向下箭头。

## 转至请求创建的对象

您可以在“我的请求”小组件中找到由请求创建的对象。

>[!NOTE]
>
>只有在请求本身创建了对象的情况下，新请求体验中才提供指向已创建对象的链接，以供Planning请求使用。 如果Workfront请求转换为项目或其他对象，则指向该转换对象的链接在新请求体验的请求列表中不可用。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. 找到创建对象的请求。
1. 单击该请求的&#x200B;**创建对象**&#x200B;列中的对象名称。

   将打开对象的页面。

