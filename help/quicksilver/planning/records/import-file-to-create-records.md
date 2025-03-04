---
title: 通过从CSV或Excel文件导入信息创建记录
description: 记录是记录类型的单个实例，记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以通过从CSV或Excel文件导入信息来创建记录。
hide: true
hidefromtoc: true
source-git-commit: 9f17fcab210768923e866d2f1596f40ddf8a558e
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---


<!-- add the following in the metadata when live:

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog-->

# 通过从CSV或Excel文件导入信息创建记录

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

记录是记录类型的单个实例，记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以通过从CSV或Excel文件导入信息来创建记录。

有关创建记录的详细信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> 标准
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p> 
   <p>在将记录连接到要创建的对象类型（项目和项目组合）时，在Workfront中编辑对这些对象的访问权限。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理要向其中添加记录的工作区的权限。 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>管理Workfront对象（项目组合）的权限以添加子对象（项目）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于使用Excel或CSV文件导入记录类型的注意事项

* 每个工作表中的列标题将成为与记录关联的字段。
* 每个工作表中的每一行都成为关联的唯一记录。
* 如果Excel文件包含多个工作表，则只导入导入导入过程中所选择的一个工作表中的信息。
* 文件不应超过以下内容：
   * 10,000行
   * 500列
* 文件不应大于5MB。
* 不支持空工作表。
* 以下类型的字段不受支持，无法映射到导入工作表中的字段：
   * 已连接记录或已连接Workfront对象的查找字段
   * 公式字段
   * 创建日期，创建者
   * 上次修改日期，上次修改人
   * 人员
* 如果导入了多选或单选字段，并且该字段与Planning中的类似字段相比，具有更多选项，则在导入期间会创建附加选项。

## 通过导入CSV或Excel文件创建记录

{{step1-to-planning}}

1. 单击要在其中创建记录类型的工作区，

   或

   从工作区中，展开现有工作区名称右侧的向下箭头，搜索工作区，然后在工作区显示在列表中时将其选定。
1. 单击要导入记录的记录类型卡。
1. 单击屏幕右上角的&#x200B;**新建记录**。
1. 单击&#x200B;**从文件**&#x200B;上载，然后单击&#x200B;**继续**。
1. 拖放以前保存在您计算机上的Excel或CSV文件，或单击&#x200B;**选择CSV或Excel文件**&#x200B;以浏览一个。
1. 单击&#x200B;**预览和编辑**。
1. （视情况而定）如果导入的文件有多个工作表，请在&#x200B;**选择要导入的工作表**&#x200B;框中选中要导入的工作表的单选按钮，然后单击&#x200B;**下一步**。 否则，请继续执行下一步。

   ![选择要导入记录的工作表](assets/select-a-sheet-to-import-box.png)
1. 在&#x200B;**将Planning字段映射到列标题**&#x200B;中，选择与工作表的每个列中的信息最匹配的&#x200B;**Planning字段**。

   导入记录时![将Planning字段映射到列](assets/map-planning-fields-to-columns-when-importing-records.png)

   每一行表示一个新记录。 只有前10条记录会显示在“预览和编辑”框中。

1. （可选）选择屏幕左下角的&#x200B;**创建缺少的选项**。 启用后，将添加缺少的单选和多选字段选项。

   例如，如果选定的记录类型具有单选的“状态”字段，其中包含“新建”、“进行中”和“已关闭”选项，并且从文件导入的“状态”字段也具有“暂挂状态”选项，则还会添加“暂挂”状态选项

   <!--when we add connected records and the info icon in the tool changes, also add those items to this step-->

1. 单击&#x200B;**导入**。

   以下信息导入到Workfront Planning中：

   * 在所选记录类型的表格视图底部显示的新记录。
   * 与每个记录关联的现有字段的新字段值。
   * Planning中不存在的多选或单选字段的新选择。

   您可以在记录类型页面上开始管理字段和记录。

   有权访问Workfront Planning和工作区的每个人都现在可以查看和编辑导入的记录及其信息。