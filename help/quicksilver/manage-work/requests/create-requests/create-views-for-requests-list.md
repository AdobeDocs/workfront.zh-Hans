---
product-area: requests
navigation-topic: create-requests
title: 在请求区域创建和管理视图
description: 如果您使用的是新的请求体验，则可以创建和保存请求区域的视图。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 2%

---


# 在请求区域创建和管理视图

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


如果您在Adobe Workfront中使用新的请求体验，则可以创建和保存请求区域的视图。 这些视图包括筛选器和列安排。

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* 此功能仅在请求区域的新请求体验中可用。
>* 查看设置也可在主页的“我的请求”小组件中找到。 但是，请求区域中的视图与我的请求小组件中的视图是分开的。
>* 请求区域中的请求列表使用Workfront中的增强列表。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

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

## 创建请求视图

使用新的请求体验时，您可以在Workfront的请求区域中创建视图。

1. 要访问请求列表，请执行以下操作：

   {{step1-to-requests}}

1. 确保已打开&#x200B;**使用新体验**&#x200B;设置。

1. 在&#x200B;**请求**&#x200B;列表中，单击&#x200B;**视图**&#x200B;下拉菜单![视图下拉菜单](assets/view-icon-requests.png)，然后单击&#x200B;**新建视图**。

   ![新视图](assets/create-new-view.png)

1. 输入新视图的名称，然后单击&#x200B;**创建**。
1. 继续[在请求区域](#edit-a-view-in-the-requests-area)中编辑视图。

## 编辑请求视图

您可以编辑现有视图，包括之前在Workfront的“请求”区域中创建的视图。

通过在请求区域中编辑视图，可以更改视图的以下元素：

* 名称
* 过滤器
* 列

您对视图所做的更改对您共享该视图的所有用户都可见。

1. 要在请求中访问请求列表，请执行以下操作：

   {{step1-to-requests}}

1. 确保已打开&#x200B;**使用新体验**&#x200B;设置。
1. 在&#x200B;**请求**&#x200B;列表中，从&#x200B;**视图**&#x200B;下拉菜单![视图下拉菜单](assets/view-icon-requests.png)中找到要编辑的视图。

1. 单击&#x200B;**视图**&#x200B;下拉列表![视图下拉列表](assets/view-icon-requests.png)并单击视图旁边的三个点菜单，选择&#x200B;**重命名**，然后键入视图的新名称。
1. 按Enter键保存新名称。
1. 单击&#x200B;**视图**&#x200B;下拉列表![视图下拉列表](assets/view-icon-requests.png)，然后选择要编辑的视图。
1. 要将字段添加为列，请单击列表右上角的&#x200B;**添加列**&#x200B;图标![添加列](assets/add-column.png)。

   **列管理器**&#x200B;打开。
1. 单击要作为列添加到视图的字段旁边的加号图标，然后单击&#x200B;**保存**。

   与列表中对象关联的字段可添加为列。<!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >添加到列的字段必须先存在，然后才能在&#x200B;**列管理器**&#x200B;中使用。

1. （可选）单击&#x200B;**列**&#x200B;以打开&#x200B;**字段可见性和顺序**&#x200B;框。
1. 打开要在列表中显示的每个字段的设置，关闭它以隐藏它，或以不同的顺序拖放字段。

1. （可选）单击&#x200B;**筛选器**，然后开始为要查看的请求添加条件。

   您可以按以下请求字段进行筛选：

   * **Workspace**：与请求表单关联的工作区。
   * **对象类型**：与请求表单关联的记录类型。
   * **输入日期**：提交请求的日期。
   * **请求表单**：用于提交请求的请求表单的名称。
   * **状态**：请求的状态。
   * **输入者**：添加请求的用户的名称。 如果请求是由Workfront之外的人员添加的，则&#x200B;**输入者**&#x200B;字段显示`N/A`。

   您还可以按已添加到视图的任何字段对该视图中可见的任何对象进行过滤。

   您可以有多个&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;加入的筛选器。
在添加筛选条件时，将自动筛选请求列表。


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 对视图的更改会自动保存。
> * 对视图的更改对使用该视图的任何人都可见。
> * 在任何以用户作为值的字段中使用&#x200B;**Me（已登录的用户）**&#x200B;筛选器通配符。

## 将请求视图添加到布局模板。

Workfront管理员可以将新视图添加到布局模板。

有关说明，请参阅[使用布局模板自定义筛选器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 共享视图

您可以与其他用户、团队或组共享您创建的视图。

1. 要在请求中访问请求列表，请执行以下操作：

   {{step1-to-requests}}

1. 确保已打开&#x200B;**使用新体验**&#x200B;设置。
1. 在&#x200B;**请求**&#x200B;列表中，找到要共享的视图。
1. 将鼠标悬停在要共享的视图上，单击视图名称右侧的三个圆点菜单，然后单击&#x200B;**共享**。
1. 在&#x200B;**共享**&#x200B;框中，输入要与其共享视图的人员、团队、角色、组或公司，然后在它们出现时从列表中选择它们。
1. 单击&#x200B;**保存**。

   视图将与您指定的实体共享。 用户可以在共享视图之前查看您为该视图编辑的更新视图元素。 <span class="preview">如果他们更新视图，其他人将无法看到他们的更改，除非他们制作同一视图的副本并在共享副本之前保留其更改。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。</span>
