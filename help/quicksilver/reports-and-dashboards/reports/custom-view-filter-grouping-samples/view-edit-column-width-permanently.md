---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：永久编辑列的宽度'
description: 可通过拖放栏的边距以匹配所需宽度来临时修改栏的宽度。 有关详细信息，请参阅修改列宽和顺序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 视图：永久编辑列的宽度

<!-- Audited: 1/2024 -->

可通过拖放栏的边距以匹配所需宽度来临时修改栏的宽度。 有关更多信息，请参阅 [修改列宽和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

要永久更改任何视图的任何列的宽度，编辑视图时必须在列中使用文本模式。

## 访问要求

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

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 永久编辑列的宽度

>[!IMPORTANT]
>
>如果按照一节所述手动修改列的宽度 [临时修改列的宽度和顺序](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) 在文章中 [修改列宽和顺序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改列的宽度后，将根据手动调整大小保留列的宽度。 在这种情况下，将覆盖根据以下步骤更新的列宽。 清除缓存或从其他浏览器登录后，您可以根据以下步骤中定义的宽度查看列。
>
>有关在使用文本模式界面时自定义列宽的其他信息，请参阅 [Adobe Workfront术语表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. 转到对象列表。
1. 从 **视图** 下拉菜单，单击 **新建视图**.

1. 单击 **添加列** 以添加新列。

   或

   单击任何现有列的列标题。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 将以下代码添加到列的文本模式中：

   ```
   width=200
   usewidths=true
   ```

   对于 **宽度** 行，指定任意数字（以像素为单位）来表示您希望列在视图中显示的宽度。

1. 单击 **保存**，则 **保存视图**.


