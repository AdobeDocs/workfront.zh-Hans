---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：隐藏列的内容'
description: 您可能希望隐藏视图列中的信息。 可以通过修改列的文本模式来实现此目的。
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 视图：隐藏列的内容

<!--Audited: 11/2024-->

您可能希望隐藏视图列中的信息。 可以通过修改列的文本模式来实现此目的。

>[!NOTE]
>
>* 您可以使用隐藏列按不希望显示在视图中的特定对象进行排序。\
>  例如，您可以按任务视图中的任务编号进行排序，然后在视图中隐藏任务编号信息。 在这种情况下，列中引用的对象有助于对视图进行排序，但该对象的信息不会显示在视图中。
>* 隐藏列时，请注意，该列中的信息是隐藏的，但该列仍然存在于视图中。
>

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：<ul><li>修改视图的参与者</li><li>用于修改报告的标准</li></ul></p><p>或</p>当前：<ul><li>请求修改视图</li><li>计划修改报告</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 示例：在任务视图中排序并隐藏任务编号列：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**&#x200B;并开始在&#x200B;**显示在此列**&#x200B;字段中键入“任务编号”，然后当它显示在列表中时将其选中。

1. 单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   此代码中使列隐藏的重要更改包括：

   * `displayname=`：此行必须为空。
   * `valuefield=`：此项已被`value`取代，必须为空。
   * `width=`：根据字段，该值必须为&#x200B;**0**&#x200B;或&#x200B;**1**。

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。
