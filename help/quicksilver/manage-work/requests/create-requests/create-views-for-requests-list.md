---
product-area: requests
navigation-topic: create-requests
title: 在请求区域创建和管理视图
description: 如果您使用的是新的请求体验，则可以创建和保存请求区域的视图。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 3%

---


# 在请求区域创建和管理视图

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

如果您在Adobe Workfront中使用新的请求体验，则可以创建和保存请求区域的视图。 这些视图包括筛选器、列排列和分组。

>[!IMPORTANT]
>
>* 此功能仅在请求区域的新请求体验中可用。
>* 查看设置也可在主页的“我的请求”小组件中找到。 但是，请求区域中的视图与我的请求小组件中的视图是分开的。
>* 请求区域和我的工作小组件中的请求列表使用Workfront中的增强列表。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何Workfront或工作流包</p>
   <p>任何Workfront Planning许可证，用于在请求列表中查看Workfront Planning请求</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p>  <p>您必须是Workfront管理员才能将视图添加到布局模板</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 请求的系统视图

除了您可以自己创建的视图之外，Workfront还在主页为请求区域以及我的请求小组件提供以下系统视图：

* **所有请求**：您或其他人在队列或工作区中提交的、您有权查看的所有请求。 这对“我的请求”小组件不可用。
* **我的请求**：您提交的请求，不考虑状态。
* **我的未结请求**：您提交的请求仍然未结。
* **我的草稿**：您的请求草稿尚未提交。
* **打开请求**：您或其他人在队列中提交的请求，或者您有权查看的工作区仍在打开的请求。 这对“我的请求”小组件不可用。

不能编辑系统视图。 您可以修改其元素，然后复制视图并编辑或共享副本。

## 创建请求视图

使用新的请求体验时，您可以在Workfront的请求区域中创建视图。 启用和新请求体验后，您还可以在“主页”中为“我的请求”小组件创建视图。

1. 要访问&#x200B;**请求**&#x200B;列表，请执行以下操作：

   {{step1-to-requests}}

   1. 确保已打开&#x200B;**使用新体验**&#x200B;设置。

1. 要在主页中访问&#x200B;**我的请求**&#x200B;构件，请执行以下操作：

   {{step1-to-home}}

   1. 添加或转到&#x200B;**我的请求**&#x200B;构件。

1. 在请求列表中，单击&#x200B;**视图**&#x200B;下拉菜单![视图下拉菜单](assets/view-icon-requests.png)，然后单击&#x200B;**新视图**。

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. 输入新视图的名称，然后单击&#x200B;**创建**。
1. 继续[编辑请求](#edit-a-view-for-requests)的视图。

## 编辑请求视图

您可以编辑现有视图，包括您刚刚在请求区域创建的视图或主页中的我的请求构件。

通过编辑视图，可以更改视图的以下元素：

* 名称
* 过滤器
* 列
* 分组
* 设置单元格的格式
* 行高

有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 对视图的更改会自动保存。
> * 只有在对视图进行更改后共享该视图的新副本时，使用该视图的任何人都可以看到对视图的更改。
> * 在任何以用户作为值的字段中使用&#x200B;**Me（已登录的用户）**&#x200B;筛选器通配符。

## 将请求视图添加到布局模板

Workfront管理员可以为请求区域的布局模板添加新视图。

有关说明，请参阅[使用布局模板自定义筛选器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共享视图

您可以与其他用户、团队、组或公司共享您创建的视图。

共享视图后，其他用户可以在共享视图之前查看您为该视图编辑的更新视图元素。

如果他们更新视图，则其他人将无法看到他们的更改，除非他们制作同一视图的副本并在共享副本之前保留其更改。

有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->