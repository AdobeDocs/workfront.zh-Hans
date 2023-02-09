---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：永久编辑列的宽度
description: 您可以通过拖放列的边距以匹配所需的宽度，来临时修改列的宽度。 有关更多信息，请参阅修改列宽和顺序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 查看：永久编辑列的宽度

您可以通过拖放列的边距以匹配所需的宽度，来临时修改列的宽度。 有关更多信息，请参阅 [修改列宽和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

在编辑视图时，您可以使用列中的文本模式永久更改任何视图的任何列的宽度。

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

## 永久编辑列的宽度

>[!IMPORTANT]
>
>如果按照文章中“临时修改列的宽度和顺序”一节中的所述手动修改列的宽度 [修改列宽和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改列宽后，将根据手动调整大小来保留列宽，并会覆盖根据以下步骤更新的列宽。 清除缓存或从其他浏览器登录后，您可以根据以下步骤中定义的宽度来查看列。

1. 转到对象列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列** 添加新列。

   或

   单击任何现有列的列标题。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 将以下代码添加到列的文本模式：

   ```
   width=200
   usewidths=true
   ```

   对于 **宽度** 行中，指定表示您希望列在视图中显示的宽度的任意数字（以像素为单位）。

1. 单击 **保存**，则 **保存视图**.
