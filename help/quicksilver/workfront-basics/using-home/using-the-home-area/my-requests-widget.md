---
product-area: projects
navigation-topic: use-the-home-area
title: 使用我的请求小组件
description: 您可以在“我的请求”小组件中提交请求。 您还可以使用过滤器和列自定义构件。
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 3%

---

# 使用我的请求小组件


>[!IMPORTANT]
>
>本文介绍了新的My Requests构件。 您必须启用新的请求体验才能查看新的构件。
>&#x200B;>您可以在请求区域中启用新的请求体验。

“我的请求”小组件会显示已提交给贵组织的请求。 您可以筛选请求、搜索特定请求或调整列顺序和可见性。 您还可以从“我的请求”小组件创建新请求。

>[!NOTE]
>
>* 加载My Requests小组件后，它最多显示50个请求。 要显示更多请求，请向下滚动列表。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
    <tr> 
   <td role="rowheader"><strong>其他产品</strong></td> 
   <td> 您必须拥有Adobe Workfront Planning才能查看Planning请求或请求表单</td> 
  </tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>查看对您在对话中被标记或需要解决审批的任何对象（项目、任务、问题、文档）的访问权限或更高</p> </td> 
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

有关说明，请参阅从主页区域创建工作项和项目一文中的[创建请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request)。

## 筛选请求

我的请求小组件具有一个可自定义的筛选器，通过该筛选器，您可以控制哪些请求会显示在小组件中。 您可以为不同的字段和值配置此过滤器，也可以使用AND和OR来栈叠条件。

要在我的请求小组件中配置过滤器，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，查找&#x200B;**我的请求**。
1. 在“我的请求”小部件中，单击&#x200B;**筛选器**。
1. 在最左侧的字段中，选择要作为筛选依据的内容。 可用选项包括：

   * Workspace
   * 对象类型
   * 输入日期
   * 申请表
   * 状态
   * 输入者

1. 在下一个字段中，选择要用于此筛选条件的运算符。 可用的运算符取决于所选的字段。
1. （视情况而定）如果运算符右侧显示了字段，请选择要作为筛选依据的值。
1. （可选）要添加其他筛选条件，请单击&#x200B;**添加条件**&#x200B;并重复步骤4-6。
1. （可选且有条件）如果您有多个条件，请通过单击条件左侧的&#x200B;**And**&#x200B;或&#x200B;**Or**&#x200B;来切换And或Or值。

该过滤器将自动保存。

>[!TIP]
>
>如果贵组织已购买Workfront Planning，则“我的请求”小组件将包含Workfront和Workfront Planning请求。
> 
>* 要仅筛选Workfront请求，请将筛选器设置为&#x200B;**对象类型** > **具有任何** > **问题**。
>* 要仅筛选Workfront Planning请求，请将筛选器设置为&#x200B;**对象类型** > **不包含** > **问题**。

## 调整列

您可以选择哪些可用列出现在“我的请求”小部件上，并设置其顺序。

可用的列包括：

* 主题
* 已创建对象
* 对象类型
* 状态
* 申请表
* 输入日期
* 输入者

要调整“我的请求”小组件上的列，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，查找&#x200B;**我的请求**。
1. 在“我的请求”小部件中，单击&#x200B;**列**。
1. （可选）要重新排序列，请单击要移动的列的拖动手柄![拖动手柄](assets/drag-handle.png)，然后将其拖动到所需的位置。 列表顶部的列在“我的请求”小部件中显示为最左侧的列。
1. （可选）使用切换开关可控制某列是否显示在“我的请求”小部件中。

列首选项会自动保存。

## 搜索请求

要在“我的请求”小组件中搜索特定请求，请执行以下操作：

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）将&#x200B;**我的请求**&#x200B;构件添加到您的主屏幕。 单击&#x200B;**自定义**，查找&#x200B;**我的请求**。
1. 在我的请求小部件的右上角附近的搜索栏中，输入要搜索的术语。

   包含术语的请求以橙色突出显示。

1. （可选）要跳转到突出显示的请求，请单击搜索栏中的向上或向下箭头。
