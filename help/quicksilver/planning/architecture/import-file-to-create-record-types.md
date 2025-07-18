---
title: 通过从CSV或Excel文件导入信息创建记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，通过从CSV或Excel文件导入信息，说明组织生命周期中所需的工作项。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# 通过从CSV或Excel文件导入信息创建记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以创建自定义记录类型，通过从CSV或Excel文件导入信息，说明组织生命周期中所需的工作项。

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
   <td><p> 标准</p>
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
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>

</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 关于使用Excel或CSV文件导入记录类型的注意事项

* Excel文件的每一页都变为记录类型。 工作表的名称将成为记录类型的名称。
* 如果只有一个工作表，或者导入CSV文件，则文件的名称将成为记录类型的名称。
* 每个工作表中的列标题成为与每个记录类型关联的字段。
* 字段对于其各自的记录类型是唯一的。
* 每个工作表中的每一行都成为与其各自记录类型相关联的唯一记录。
* Excel文件的每一页不应超过以下内容：
   * 25,000行
   * 500列
* 文件不应大于5MB。
* 不支持空工作表。
* 以下类型的字段不受支持，无法映射到导入工作表中的字段：

   * 将字段连接到Workfront和AEM Assets对象类型。
   * 从连接的Planning记录或Workfront和AEM Assets对象查找字段
   * 公式字段
   * 创建日期，创建者
   * 上次修改日期，上次修改人
   * <span class="preview">批准日期，批准者：</span>
   * 人员

要使用Excel或CSV文件导入记录类型，请执行以下操作：

{{step1-to-planning}}

1. 单击要在其中创建记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。
1. 单击&#x200B;**添加记录类型**。
1. 单击&#x200B;**从文件**&#x200B;上载。
1. 拖放以前保存在您计算机上的Excel或CSV文件，或单击&#x200B;**选择CSV或Excel文件**&#x200B;以浏览该文件，然后选择该文件。
1. 单击&#x200B;**预览和编辑**。

   显示&#x200B;**预览和编辑**&#x200B;框并显示以下信息：

   * 工作表或未来记录类型的名称显示在左侧面板中。 默认情况下，Workfront Planning会为每个新记录类型选择一个图标和一种颜色。
   * 选择第一个工作表或记录类型，并且与其关联的字段的名称显示为列标题。 默认情况下，会选择每个字段的类型。
   * 每一行表示一个新记录。 只有前10条记录会显示在“预览和编辑”框中。

   ![预览和编辑框](assets/preview-and-edit-box.png)

1. （可选）单击左侧面板中每个页面的名称以查看其中包含的信息。

   >[!NOTE]
   >
   >不支持空的页面，这些页面将呈灰显状态。

1. （可选）从左侧面板中取消选择不想导入的工作表。

   ![选择要导入的工作表且未选择的工作表](assets/select-sheets-to-import-drop-down-with-unselected.png)

   取消选择的工作表显示有灰色背景。

1. （可选）单击列标题右侧的向下箭头，在&#x200B;**字段**&#x200B;选项卡中执行以下操作之一：

   记录类型映射导入框上的![字段选项卡](assets/field-tab-on-record-type-import-mapping-box.png)

   * 重命名其中一个字段
   * 更改&#x200B;**字段类型**
   * 更新字段&#x200B;**描述**

1. （可选）单击&#x200B;**连接**&#x200B;选项卡以将列中的信息映射到来自其他记录类型的已连接字段。

   ![记录类型导入映射框上的“连接”选项卡](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >您只能映射到Workfront Planning连接记录中的字段。 您无法从Workfront或AEM Assets连接映射到字段。 有关详细信息，请参阅本文中关于使用Excel或CSV文件导入记录类型的注意事项[部分。](#considerations-about-importing-record-types-using-an-excel-or-csv-file)

1. （视情况而定）更新字段相关信息后，单击&#x200B;**保存**。

1. 准备导入文件时，请单击&#x200B;**导入**。

   以下信息导入到Workfront Planning中：

   * 新记录类型
   * 与每个记录类型关联的新字段
   * 与每个记录类型关联的新记录

   您可以开始管理记录类型页面上的字段和记录。

   有权访问Workfront Planning和工作区的每个人都现在可以查看和编辑导入的记录类型及其信息。
