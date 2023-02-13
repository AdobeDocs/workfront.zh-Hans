---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：隐藏列的内容”
description: 您可能希望隐藏视图列中的信息。 您可以通过修改列的文本模式来执行此操作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 查看：隐藏列的内容

您可能希望隐藏视图列中的信息。 您可以通过修改列的文本模式来执行此操作。

>[!TIP]
>
>* 您可以使用隐藏列按您不希望在视图中显示的特定对象进行排序。\
   >  例如，您可以在任务视图中按任务编号排序，并在视图中隐藏任务编号信息。 在这种情况下，列中引用的对象有助于对视图进行排序，但该对象的信息不会显示在视图中。
>* 隐藏列时，请注意列中的信息是隐藏的，但列仍存在于视图中。
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 示例：在任务视图中对“任务编号”列进行排序和隐藏：

1. 转到任务列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列** 并开始在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>此代码中可隐藏列的重要更改包括：

   ```
   displayname
   ```

   此行必须为空。

   ```
   valuefield
   ```

   已替换为 *值*，且必须为空。

   ```
   width
   ```

   :根据字段，此值必须为 *0* 或 *1*.

1. 单击 **保存**，则 **保存视图**.
