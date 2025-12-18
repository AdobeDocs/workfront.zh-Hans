---
product-area: requests
navigation-topic: create-requests
title: 在请求区域创建视图
description: 如果您使用的是新的请求体验，则可以创建和保存请求区域的视图。
author: Becky
feature: Work Management
source-git-commit: d2e938cabc5123a89335a42ed06bccaa77fcad83
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 2%

---

# 在请求区域创建或编辑视图

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

如果您使用的是新的请求体验，则可以创建和保存请求区域的视图。 这些视图包括筛选器和列安排。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何 </p> </td> 
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
  <tr> 
   <td role="rowheader"> 产品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必须拥有Adobe Workfront Planning才能查看Planning请求或请求表单</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在请求区域创建视图

{{step1-to-requests}}

1. （可选且视情况而定）如果以下各项适用于您的组织和Workfront实例，请选择屏幕右上角的&#x200B;**切换到新体验**&#x200B;设置：

   * 您的组织已购买Workfront包
   * 您的组织已载入到Adobe Unified Experience。
   * 您的管理员已向您授予Workfront Planning的访问权限
   * 您至少具有Workfront规划工作区的查看权限

   有关详细信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)

1. 单击&#x200B;**视图**&#x200B;下拉列表![视图下拉列表](assets/view-icon-requests.png)并选择&#x200B;**新视图**。

   ![新视图](assets/create-new-view.png)

1. 输入新视图的名称，然后单击&#x200B;**创建**。
1. 继续[在请求区域](#edit-a-view-in-the-requests-area)中编辑视图。

## 在请求区域中编辑视图

您可以编辑现有视图，包括刚刚创建的视图。

{{step1-to-requests}}

1. （可选且视情况而定）如果以下各项适用于您的组织和Workfront实例，请选择屏幕右上角的&#x200B;**切换到新体验**&#x200B;设置：

   * 您的组织已购买Workfront包
   * 您的组织已载入到Adobe Unified Experience。
   * 您的管理员已向您授予Workfront Planning的访问权限
   * 您至少具有Workfront规划工作区的查看权限

   有关详细信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)1。

1. （可选）要重命名视图，请单击&#x200B;**视图**&#x200B;下拉列表![视图下拉列表](assets/view-icon-requests.png)，然后单击视图旁边的三个点菜单，选择&#x200B;**重命名**，然后键入视图的新名称。
1. 单击&#x200B;**视图**&#x200B;下拉列表![视图下拉列表](assets/view-icon-requests.png)，然后选择要编辑的视图。
1. <span class="preview">要将自定义字段添加为列，请单击屏幕右侧附近的&#x200B;**添加列**&#x200B;图标![添加列](assets/add-column.png)，然后单击要作为列添加到视图的自定义表单字段旁边的加号图标。</span>

   <span class="preview">附加到列表中对象的表单上的自定义字段可以添加为列。</span>

   >[!TIP]
   >
   >您当前无法在生产环境中添加列。
1. （可选）单击&#x200B;**列**&#x200B;并隐藏、显示或重新排列请求列表中的列。

   ![列框](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >您当前无法在生产环境中添加任何其他列。

1. （可选）单击&#x200B;**筛选器**&#x200B;并开始为要在Planning选项卡中查看的请求添加条件。

   ![在Planning请求选项卡中编辑筛选器](assets/filters-editing-box-in-requests-planning-tab.png)

   您可以按以下字段进行筛选：

   * **Workspace**：与请求表单关联的工作区。
   * **记录类型**：与请求表单关联的记录类型。
   * **输入日期**：提交请求的日期。
   * **请求表单**：用于提交请求的请求表单的名称。
   * **状态**：请求的状态。
   * **输入者**：添加请求的用户的名称。 如果请求是由Workfront之外的人员添加的，则&#x200B;**输入者**&#x200B;字段显示`N/A`。

   <span class="preview">在“预览”环境中，您还可以按已添加到视图的任何自定义字段进行筛选。</span>

   您可以有多个&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;加入的筛选器。
在添加筛选条件时，将自动筛选请求列表。



>[!IMPORTANT]
>
> * 对视图的更改会自动保存。
> * 对视图的更改对使用该视图的任何人都可见。

## 将视图添加到布局模板。

Workfront管理员可以将新视图添加到布局模板。

有关说明，请参阅[使用布局模板自定义筛选器、视图和分组](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。
