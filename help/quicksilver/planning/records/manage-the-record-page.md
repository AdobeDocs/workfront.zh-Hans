---
title: 管理记录页面布局
description: 您可以在Adobe Workfront Planning中编辑记录预览和页面的布局。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '2434'
ht-degree: 1%

---


# 管理记录页面布局

<span class="preview">此页面上突出显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中编辑记录预览和页面的布局。

记录预览是记录类型视图中显示的记录页面的较小视图。

当您更改记录预览和页面的布局时，更改会影响相同类型的所有记录的预览框和详细信息页面。

本文介绍了如何更改记录预览框或记录页面的布局和外观。 有关编辑记录的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

必须先创建记录类型和记录，然后才能开始编辑记录页。

有关信息，请参阅以下文章：

* [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)

* [创建记录](/help/quicksilver/planning/records/create-records.md)

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
<p>任何</p>
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
   <td>
   <p>标准</p>
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
   <td>
   <p>为工作区和记录类型</a>贡献或更高权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> 
  </td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 有关编辑记录页面的注意事项

* 默认情况下，记录的详细信息和预览页面显示与该记录关联的所有字段。

* 您不能在预览或详细信息页面中为记录添加新字段。 您必须在表格视图中添加新字段，才能在预览和详细信息页面中显示它们。

* 您可以将部分添加到记录预览或详细信息页面，以按通用标准组织信息并使其更易于查找。

* 以下更改将影响同一类型的所有记录，并且访问这些记录的所有用户都可以看到这些更改：

   * 重新排列字段
   * 添加或删除部分

* 显示在记录预览中所做的更改会立即显示在记录详细信息页面中。 在记录页面中所做的更改也会显示在记录预览框中。

* 向记录添加封面图像或缩略图不是记录预览或页面整体布局的一部分。 您可以为每个记录添加唯一的封面图像或缩略图。 有关信息，请参阅[将封面图像添加到记录](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)和[将缩略图添加到记录](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

## 向记录预览或页面添加分区

向记录页添加节时，请考虑以下事项：

* 一个页面上可以具有的节数没有限制。
* 分区不能为空。 在一个部分中，必须至少有一个字段。
* 可以将字段从一个区域拖放到另一个区域。 有关详细信息，请参阅本文中记录预览或详细信息页面中的[重新排列字段](#rearrange-fields-in-the-record-preview-or-details-page)部分。
* 从分区中删除所有字段时，该分区将自动删除且无法恢复。

要将节添加到记录预览或页面，请执行以下操作：

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录的名称

   或

   从表格视图中，单击第一列中的&#x200B;**打开详细信息**&#x200B;图标![在表格名称字段](assets/open-details-icon-in-table-name-field.png)中打开详细信息图标。

   记录的预览将在视图中打开。

   ![详细信息框](assets/details-box.png)

1. （可选）单击记录预览右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)以在新标签中打开记录页面。

   此时将打开记录页面。 默认情况下，将打开“详细信息”选项卡。

   ![详细信息页面](assets/details-page.png)

1. 在记录预览或页面的&#x200B;**详细信息**&#x200B;选项卡中，将鼠标悬停在字段左侧的空格上，然后单击&#x200B;**添加节**&#x200B;图标![添加节图标](assets/add-section-icon.png)以添加节。
1. 单击该节的名称并用名称替换&#x200B;**无标题节**，然后单击Enter。 在部分下显示的字段自动成为新部分的一部分。
1. 开始将字段拖放到新部分，如本文中记录预览或详细信息页面[中的](#rearrange-fields-in-the-record-preview-or-details-page)重新排列字段部分所述。

1. （可选）将鼠标悬停在节名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。

   记录页面![上节的](assets/more-menu-options-for-section-on-record-page.png)更多菜单选项
1. （可选）执行以下操作之一以编辑部分：

   * 单击&#x200B;**重命名**&#x200B;以重命名该节

     >[!TIP]
     >
     > 通过单击名称，可以内联重命名截面。

   * 单击&#x200B;**上移**&#x200B;将分区上移一个位置

     或

     单击&#x200B;**下移**&#x200B;以将节下移一个位置。
部分中的所有字段都会随部分一起移动。

   * 单击&#x200B;**删除**&#x200B;以删除该节。 该部分已被删除，无法恢复。 访问此类型记录的所有用户将不再查看已删除的分区。

1. 单击区域名称左侧的向下箭头可将其折叠，单击向右箭头可将其展开。
默认情况下，所有部分都处于扩展状态。

1. （可选）单击节名称左侧的&#x200B;**抓取**&#x200B;图标![抓取图标](assets/grab-icon.png)，然后将其拖放到所需位置。

   对于查看记录的所有用户，相同类型的所有记录的预览和页面中的区段新位置都会更新。

   对部分和字段顺序的所有更改都将自动保存。

1. （可选）单击记录详细信息页面&#x200B;**中的**&#x200B;导出![菜单](assets/export-icon-in-record-details-page.png)导出图标，以将“详细信息”选项卡导出到Word或PDF文件。 有关详细信息，请参阅[导出记录的详细信息](/help/quicksilver/planning/records/export-the-record-page.md)。

1. （可选）单击&#x200B;**详细信息**&#x200B;选项卡旁边的&#x200B;**连接**&#x200B;选项卡。 在单击“**连接**”选项卡之前，您可能必须单击“**更多**”。

   连接到选定记录的所有记录或对象都显示在记录类型或它们所属应用程序的名称下。

   Workfront Planning中记录的![连接选项卡](assets/connections-tab-on-record-in-workfront-planning.png)

1. （可选）选择“连接”选项卡右上角的&#x200B;**显示所有记录**&#x200B;设置。 所有连接的记录类型都会显示，包括尚未连接任何记录的类型。 默认情况下，此切换处于取消选中状态，并且隐藏没有连接记录的记录类型。

1. （可选）单击&#x200B;**连接**&#x200B;以将更多记录添加到连接的记录类型。 有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

1. （可选）将鼠标悬停在记录卡片上，单击断开连接记录图标&#x200B;**-**，然后单击&#x200B;**断开连接**。 <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
出现以下情况：
   * 记录不再连接到Workfront对象。
   * Workfront对象也将从Workfront Planning中的记录的“已连接”字段中删除。
   * 连接到Planning记录的Workfront查找字段的值也会被删除。

## 重新排列记录详细信息选项卡中的字段

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. 从任何类型的视图中，单击记录的名称

   或

   从表格视图中，单击第一列中的&#x200B;**打开详细信息**&#x200B;图标![在表格名称字段](assets/open-details-icon-in-table-name-field.png)中打开详细信息图标。

   记录的预览将在视图中打开。

   ![详细信息框](assets/details-box.png)

1. （可选）单击记录预览右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签图标中打开详细信息框](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->以在新标签中打开记录页面。

   默认情况下将打开记录的&#x200B;**详细信息**&#x200B;选项卡。

   ![详细信息页面](assets/details-page.png)

1. 在记录&#x200B;**详细信息**&#x200B;选项卡中，单击字段名称左侧的&#x200B;**抓取**&#x200B;图标![抓取图标](assets/grab-icon.png)，然后将其拖放到所需位置。

   >[!TIP]
   >
   >您可以将字段拖放到另一区域。
   >在一个部分中，必须至少有一个字段。
   >

   对于查看记录的所有用户，字段的新位置会在相同类型的所有记录的预览和页面中更新。

   自动对记录预览或页面保存布局所做的所有更改。

## 将“连接的记录”页面添加到记录

通过将“连接的记录”页面的选项卡添加到记录，可以查看来自连接的记录或对象的信息。

可以在表格视图中编辑来自连接记录的信息。 来自从其他应用程序连接的对象的信息在表视图中不可编辑。

将“连接的记录”页面添加到记录时，请考虑以下事项：

* 在将记录或对象类型从记录类型的表格视图连接到记录类型后，可以将“连接的记录”页添加到记录中。

* 在“生产”环境中，无法从记录的预览添加“连接的记录”页面。

  <span class="preview">您可以从“预览”环境中记录的预览添加“连接的记录”页面。</span>

* “连接的记录”页在表格视图中仅显示一个对象或记录类型中的连接对象或记录。 该页不会在表视图中显示该类型的所有记录。

* 根据您使用的环境，您可能会注意到以下内容：

   * 在“生产”环境中，将“连接的记录”页面添加到记录后，“页面”选项卡从记录的预览区域可见，但为空。 您必须转到整页以查看所连接记录的表视图。
   * <span class="preview">在“预览”环境中，“连接的记录”页面在记录的预览区域和浏览器选项卡中均可见。</span>

* 可以为以下连接的记录或对象类型添加“连接的记录”页：

   * Workfront Planning记录类型
   * Workfront项目、项目、项目组合、组或公司。 您可以查看连接的Workfront对象，即使您无权在Workfront中访问它们。

  >[!NOTE]
  >
  >   无法为连接的AEM Assets记录添加“连接的记录”页面。

要添加“连接的记录”页，请执行以下操作：

1. 单击记录名称以将其打开。
1. 从以下区域之一单击&#x200B;**添加页面**：

   * <span class="preview">记录的预览窗口</span>
   * 记录的详细信息页面，在单击预览页面右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)之后。

   将打开&#x200B;**创建页面**&#x200B;框。

   ![添加连接的记录页面模式](assets/add-connection-view-page-modal.png)

1. 添加&#x200B;**页面名称**，单击&#x200B;**连接的记录页面**，然后单击&#x200B;**创建**。

   新选项卡将添加到记录的页面。
1. 在列表中搜索或单击连接的记录或对象类型的名称。
所选记录类型的表格视图将显示在新页面中，连接的记录将显示在表格视图中。
已连接记录的所有字段都显示在已连接记录选项卡的表视图中。

   默认情况下，将显示连接的记录表中的前五个字段。 默认情况下，不显示查找字段。

   在营销活动详细信息下![受众连接的表视图](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （可选）在连接的记录的表视图中，执行以下任一操作：

   * 单击记录名称。 这将在新选项卡中打开记录页面。

     这将打开记录的预览页面。 单击右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开](assets/open-details-in-a-new-tab-icon.png)以打开连接的记录的页面。

   * 单击&#x200B;**连接**&#x200B;以连接更多记录，然后单击连接框外部以关闭它。 新记录将自动添加到表中。
   * 在表视图中编辑来自连接记录的任何信息。

   * 将鼠标悬停在已连接记录的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下选项之一：
      * 视图
      * 复制链接
      * 编辑缩略图
      * 复制
      * 在上方或下方插入记录
      * 删除
   * 选择其中一个记录，然后单击屏幕底部蓝色栏中的以下选项之一：
      * 视图
      * 复制链接
      * 编辑缩略图
      * 复制
      * 删除。 删除是选择多个记录时唯一可用的选项。

     有关编辑表视图中的记录的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

   * 在“连接的记录”页上的表中内联编辑任何记录。

     在“生产”环境中，所有Workfront对象都以只读表格视图显示，您无法对其进行编辑。

     <span class="preview">在“预览”环境中，您可以在连接的记录页面中内联编辑项目。</span>

1. <span class="preview">（视情况而定）在查看连接的项目列表时，执行以下任一操作：</span>

   * <span class="preview">单击已连接记录页面右上角的&#x200B;**连接记录**&#x200B;以连接现有项目。</span>
   * <span class="preview">在表中内联编辑项目信息。</span>
   * <span class="preview">单击&#x200B;**新行**&#x200B;以创建没有模板的项目。</span>

     有关详细信息，请参阅将Workfront对象连接到记录时[从Workfront Planning创建对象](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * <span class="preview">将鼠标悬停在项目上并单击&#x200B;**更多**&#x200B;菜单[更多](assets/more-menu.png)，然后单击以下任一项：</span>
      * <span class="preview">**删除**&#x200B;以删除项目。 删除项目会断开它与记录的连接，并将其移至Workfront回收站。</span>
      * <span class="preview">**断开连接**&#x200B;以断开项目与记录的连接。 正在断开项目</span>的连接

1. （可选）双击“连接的记录”页选项卡的名称

   或

   将鼠标悬停在该选项卡的名称上，然后单击&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**重命名**&#x200B;以重命名为新的“连接的视图”选项卡。
1. （可选）使用工具栏中的以下任意视图元素来管理表格视图：

   * 过滤器
   * 排序
   * 分组
   * 字段，用于显示、隐藏或重新排列字段

   有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >   不能在已连接记录选项卡的表视图中创建、编辑或删除字段。
   >

1. （视情况而定）要连接多个记录或对象，请执行下列操作之一：

   * 单击表底部的&#x200B;**连接**&#x200B;以添加或删除记录或除项目之外的任何Workfront对象<span class="preview">。</span>
   * <span class="preview">在“预览”环境中，单击“连接的记录”页面右上角的&#x200B;**连接记录**&#x200B;以连接现有项目，或者单击表底部的&#x200B;**新行**&#x200B;以创建项目并自动将它们连接到当前记录。</span>

   有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. （可选）将鼠标悬停在“连接的记录”页选项卡的名称上，单击&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以移至“选项卡”。




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



