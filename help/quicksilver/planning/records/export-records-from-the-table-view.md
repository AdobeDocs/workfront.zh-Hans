---
title: 从表视图中导出记录
description: 您可以将记录及其信息从表格视图导出到CSV或Excel文件。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# 从表视图中导出记录

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中将记录及其信息从表格视图导出到Excel或CSV文件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>浅色或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>查看或更高权限的工作区和记录类型</p>   
   <p>查看或更高的视图权限</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Light or higher </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


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
