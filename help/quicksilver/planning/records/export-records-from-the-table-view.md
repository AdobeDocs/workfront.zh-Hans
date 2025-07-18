---
title: 从表视图中导出记录
description: 您可以将记录及其信息从表格视图导出到CSV或Excel文件。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: ee366e05097518a4618dd11ed5807b8766465d94
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---

# 从表视图中导出记录

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中将记录及其信息从表格视图导出到Excel或CSV文件。

## 访问要求

+++ 展开以查看访问要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置、复制或导出它。</p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从表视图中导出记录

导出表视图时，请考虑以下事项：

* 导出到Excel文件中的信息将保留应用于Workfront Planning中的表格视图的筛选器、分组和排序。 分组在CSV文件中不可见。

* 导出的文件不支持缩略图和自定义行颜色。

* 仅导出在Workfront界面中可见的字段。 隐藏字段不导出。

要从表格视图或记录类型导出信息，请执行以下操作：

1. 转到记录类型页面，然后单击表格视图选项卡。
1. 执行下列操作之一：

   * 将鼠标悬停在表视图选项卡的名称上，然后单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**导出**。

   视图上的![更多菜单](assets/view-more-menu-with-duplicate-option.png)

   * 单击&#x200B;**共享** > **导出当前视图**。 此选项仅在显示表格视图时可用。

   ![具有记录类型和视图共享选项的“共享”按钮](assets/share-button-with-record-type-and-view-sharing-options.png)

1. 选择以下格式之一：

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >当在屏幕上显示不同的视图时，不能从表格视图导出信息。 要访问“更多”菜单中的“导出”选项，必须显示要导出的表格视图。

   文件已下载到您的计算机。

1. （可选）转到计算机上的下载文件夹并找到下载的文件。

   导出文件的名称遵循以下格式：

   `Name of the view - name of the record type`

   例如，促销活动记录类型的表视图会生成一个名为`Table view - Campaigns`的文件。

   文件显示以下信息：

   * 在Excel文件中，列标题以黑色突出显示
   * 在Workfront界面中可见的所有字段，均按相同的标准进行排序和过滤
   * 分组将保留在Excel文件中

   您现在可以与其他人共享导出的文件，或将其附加到任何通信。

</div>
