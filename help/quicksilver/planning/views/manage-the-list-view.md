---
title: 在Adobe Workfront Planning中管理列表视图
description: 在Adobe Workfront Planning的记录的“连接的记录”页面中访问对象时，您可以在列表视图中显示对象及其字段。 本文介绍了如何在记录的“连接的记录”页面中创建或编辑列表视图。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: 973a095e8ff08e382010247d9ed38e48d4b2c564
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 0%

---


# 在Adobe Workfront Planning中管理列表视图

<span class="preview">此页面上突出显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning的记录的“连接的记录”页面中访问对象时，您可以在列表视图中显示对象及其字段。

本文介绍了如何在记录的“连接的记录”页面中创建或编辑列表视图，以及如何编辑视图中的对象。

## 访问权限要求

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
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何Workfront和任何Planning包</p>
<p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 用于创建和删除视图的标准</p>
   <p>更新视图元素的参与者或更高版本</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置或复制它</p> </td> 
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

## 有关列表视图的注意事项

* 您不能在列表视图的记录类型页中查看记录。 在记录的“连接的记录”页中查看下列对象时，只能在列表视图中显示这些对象：

   * Workfront项目

  有关创建连接的记录页面的信息，请参阅[将连接的记录页面添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。
* 在记录的已连接记录页面中查看列表视图之前，您必须将Workfront项目与Planning记录类型连接。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 列表视图与增强型列表类似。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。


## 管理列表视图 {#manage-a-list-view}

有关在Workfront中管理列表视图的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

{{step1-to-planning}}

1. 单击工作区信息卡，然后单击记录类型信息卡。
1. 从任何视图中，单击记录的名称以打开记录的预览或详细信息页面。
1. 为已连接项目添加&#x200B;**已连接记录页**，如文章[将已连接记录页添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)中所述。

   “连接的记录”页面在列表视图中显示与记录连接的项目。

   <!--add new screen shot when they release Conditional formatting MVP -->

   ![列表视图中已连接记录页上的项目](assets/projects-on-connected-records-page-list-view.png)

1. （可选）执行以下操作之一以修改列表视图：

   1. 展开列表右上角的下拉视图菜单以选择其他视图，或单击&#x200B;**新建视图**&#x200B;并创建另一个视图。

      视图在整个系统中共享。 如果您为一个记录类型创建项目视图，则可以在显示所连接项目的其他记录类型上查看该视图。

   1. 将鼠标悬停在现有视图的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击下列选项之一：
      * **重命名**，为视图提供一个新名称
      * **共享**，以与他人共享视图
      * **删除**，以删除该视图。

      >[!NOTE]
      >
      >* 您必须对视图具有管理权限才能编辑、共享或删除该视图。
      >
      >* 不能修改系统视图。
      >
      >* <span class="preview">您可以在修改视图以恢复其原始首选项后，重置与您共享的视图，也可以随更改一起复制并共享副本。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。</span>

   1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-icon.png)将筛选器添加到视图。 结果会立即在列表中过滤。 您无法保存并命名筛选器。 在将来的访问页面时，将会记住过滤器，并且这些过滤器是共享视图的一部分。
   1. 单击&#x200B;**列**&#x200B;图标![列图标](assets/columns-icon.png)以选择要显示或隐藏的列。
   1. 将鼠标悬停在列名上，单击该列名左侧的向下箭头，然后单击下列选项之一：
      * **重命名**，为列添加&#x200B;**自定义标签**。 Workfront中原始字段的名称不会更改。
      * **排序**，按所选字段对列表进行排序。 在列标题中添加了表示排序方向的排序图标。
   1. 单击列表右上角的&#x200B;**+**&#x200B;图标在列表中添加或删除列，然后单击&#x200B;**保存**。

      **列管理器**&#x200B;打开。

      您只能将现有字段添加到列表视图。
不能删除第一列中显示的列表视图中的主字段。


   1. <span class="preview">单击&#x200B;**格式化单元格**&#x200B;图标![格式化单元格图标](assets/format-cells-icon.png)。 **格式**&#x200B;框打开。</span> <!--change the name of the box when they update it-->
      <span class="preview">执行以下操作：</span>

      <div class="preview">

      1. 在&#x200B;**If**&#x200B;行中，单击&#x200B;**添加条件**，然后选择要作为格式化依据的字段并选择字段值。

         >[!TIP]
         >
         >只有列表视图中可见的字段可用于条件格式。

      1. （可选）单击&#x200B;**If**&#x200B;行中的&#x200B;**添加条件**&#x200B;以将更多条件添加到同一规则。

         >[!TIP]
         >
         >在一个条件规则中最多可添加10个条件，一个字段最多可有20个规则。

      1. 单击条件之间的&#x200B;**Or**&#x200B;连接器以更改为&#x200B;**And**，并指示必须同时满足多个条件。 **或**&#x200B;是默认连接器。
      1. 在&#x200B;**格式**&#x200B;行中，选择一个字段以指示将设置哪一列的格式。<!--edit this area, if it changes names??-->
      1. （可选）单击所选字段旁边的&#x200B;**颜色圆圈**&#x200B;图标![颜色圆圈图标](assets/color-circle.png)以展开该字段并选择其他颜色。
      1. 打开&#x200B;**应用到行**&#x200B;设置以将格式应用到满足条件的字段的整行。
      1. （可选）在&#x200B;**格式**&#x200B;框中单击&#x200B;**添加条件**&#x200B;为其他字段添加其他规则并重复上述步骤。
      1. （可选）单击&#x200B;**全部清除**&#x200B;以删除所有格式。
      1. 单击&#x200B;**格式**&#x200B;框外部以将其关闭。

         这会将您返回到列表视图。
格式设置将立即应用于列表视图。
**设置单元格格式**&#x200B;图标旁有一个蓝点，表示该视图应用了特殊格式。

      </div>

1. （可选）在列表右上角的搜索框中添加关键字以搜索项目。

   与搜索词匹配的项目会在列表中突出显示。

1. （可选）要将更多项添加到列表并自动将它们连接到所选记录，请执行下列操作之一：

   * 单击列表右上角的&#x200B;**连接记录**&#x200B;以添加现有项。
   * 单击列表底部的&#x200B;**新行**&#x200B;以添加新项。
1. 单击列表中已连接项目的名称，以在其他浏览器选项卡中将其打开。
1. 双击列表中的单元格以编辑字段信息，然后按Enter保存更改。

   某些字段为只读。 例如，项目的完成百分比是由系统计算的字段，您无法手动进行编辑。

1. 将鼠标悬停在列表中项目的名称上，然后单击&#x200B;**更多**&#x200B;菜单[更多菜单](assets/more-menu.png)，然后单击&#x200B;**查看**&#x200B;以在其他选项卡中打开项目

   或

   选择一个或多个项目，并注意列表底部的操作栏，然后单击以下项之一：

   * **删除**&#x200B;以删除项目。 删除项目会断开它与记录的连接，并将其移到Workfront的回收站。 Workfront管理员最多可以在删除项目后30天内恢复这些已删除的项目。
   * **断开连接**&#x200B;以断开项目与记录的连接。 断开项目连接会将其及其查找字段的所有值从当前记录中删除。

   “连接的记录”页面列表视图中的![操作栏](assets/actions-bar-connected-records-page-list-view.png)

