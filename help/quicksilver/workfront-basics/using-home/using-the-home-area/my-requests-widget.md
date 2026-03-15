---
product-area: projects
navigation-topic: use-the-home-area
title: 使用我的请求小组件
description: You can submit requests in the My Requests widget. You can also customize the widget with filters and columns.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 3%

---

# 使用我的请求小组件

>[!IMPORTANT]
>
>This article describes the new My Requests widget. You must have the new requesting experience enabled to see the new widget.
>您可以在“请求”区域中启用新的请求体验。

“My Requests”小组件会显示您提交的请求。 您可以筛选请求、搜索特定请求或调整列顺序和可见性。 您也可以从“我的请求”小组件创建新请求。

>[!NOTE]
>
>* 加载My Requests小组件时，它最多显示50个请求。 要显示更多请求，请向下滚动列表。

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

## Create a request

You can create a request directly from the My Requests widget.

For instructions, see the section [Create a request](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) in the article [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## 复制请求

You can copy a request in the My Requests widget, edit it, and submit it as a new request.

有关说明，请参阅[复制并提交请求](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 筛选请求

My Requests小组件中有一个可自定义的过滤器，允许您控制哪些请求要显示在小组件中。 您可以为不同的字段和值配置此过滤器，也可以使用AND和OR运算符栈叠条件。

要在“我的请求”小组件中配置过滤器，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]**![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. 在&#x200B;**我的请求**&#x200B;小组件中，单击&#x200B;**筛选器**。
1. 选择要作为筛选依据的字段。 可用选项包括：

   * Workspace
   * 对象类型
   * 输入日期
   * 申请表
   * 状态
   * 输入者
   * 来自请求或来自创建对象的自定义字段

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.

The filter is saved automatically.

>[!TIP]
>
>如果您的组织除了Adobe Workfront之外还购买了Workfront Planning，则My Requests小组件将同时包含Workfront和Workfront Planning请求。
> 
>* 要仅筛选Workfront请求，请将筛选器设置为&#x200B;**对象类型** > **具有任何** > **问题**。
>* 要仅筛选Workfront Planning请求，请将筛选器设置为&#x200B;**对象类型** > **不包含** > **问题**。

## 调整或添加列

您可以选择哪些可用列出现在“我的请求”小部件上，并设置其顺序。

可用的列包括：

* 主题
* 已创建对象
* 对象类型
* 状态
* 申请表
* 输入日期
* 输入者

To adjust the columns on the My Requests widget:

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. 在&#x200B;**我的请求**&#x200B;小组件中，单击&#x200B;**列**。
1. （可选）要对列重新排序，请单击要移动的列的拖动手柄![拖动手柄](assets/drag-handle.png)，然后将其拖动到所需位置。 列表顶部的列在“我的请求”小组件中显示为第一列。
1. （可选）使用切换功能隐藏或显示请求列表中的列。
1. 要将自定义字段添加为列，请单击列表右上角的&#x200B;**添加列**&#x200B;图标![添加列](assets/add-column.png)，然后单击要作为列添加到小组件中的自定义字段旁边的加号图标。

   附加到列表中对象的表单上的自定义字段可以添加为列。

列首选项会自动保存。

## 创建视图

您可以在“我的请求”小组件中创建视图，以更改信息在请求列表中的显示方式。

使用我的请求小组件中的视图时，请考虑以下事项：

* 我的请求小组件中的视图包含应用于该视图的列和筛选器。
* 您可以创建视图并将其与他人共享。 在共享视图之前为视图选择的筛选器和列将包含在共享视图中。
* 以下是您无法编辑、共享或删除的系统视图：

   * 构件统一请求默认视图
* 在我的请求小部件中创建和编辑视图类似于增强列表。 有关信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

## 搜索请求

To search for specific requests in the My Requests widget:

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. In the search bar near the upper-right of the My Requests widget, enter the term that you want to search for.

   包含术语的请求以橙色突出显示。

1. （可选）要跳转到突出显示的请求，请单击搜索栏中的向上或向下箭头。

## 转到由请求创建的对象

可在“我的请求”小组件中查找由请求创建的对象。

>[!NOTE]
>
>只有在请求本身创建了对象的情况下，才能在新的Planning请求体验中找到指向已创建对象的链接。 如果Workfront请求被转换为项目或其他对象，则在新的请求体验中，指向转换后的对象的链接在请求列表中不可用。

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]**![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，找到&#x200B;**我的请求**，然后单击它以将其添加到&#x200B;**主页**。
1. 找到创建对象的请求。
1. 单击该请求的&#x200B;**创建对象**&#x200B;列中的对象名称。

   将打开对象的页面。

