---
title: 向记录添加“连接的记录”页
description: 通过将“连接的记录”页面的选项卡添加到记录，可以查看来自连接的记录或对象的信息。 这会将表视图中的连接记录添加到选项卡。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '2745'
ht-degree: 0%

---


# 将“连接的记录”页面添加到记录

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

通过在Adobe Workfront Planning中将已连接记录页面的选项卡添加到记录，可以查看已连接记录或对象中的信息。 这会将表视图中的连接记录添加到选项卡。

将“连接的记录”页面添加到记录时，请考虑以下事项：

* 将记录或对象类型从其表格视图连接到记录类型后，可以将“连接的记录”页添加到记录。

* 您可以从记录的预览区域或记录的页面添加“连接的记录”页面。

* <span class="preview">对于特定记录类型，只能有一个连接的记录页面。</span>

  <span class="preview">例如，如果为营销活动创建了一个连接的记录页面，并且要显示其连接的角色，则只能有一个连接的角色记录页面。</span>

* “连接的记录”页面仅显示来自一个对象或记录类型的连接的对象或记录。 页面不显示该类型的所有记录。

* 根据在连接的记录页面中显示的对象或记录类型，可以使用以下视图显示它们：

   * 您可以在以下视图中显示连接的Planning记录：
      * 表
      * <span class="preview">时间线</span>
      * <span class="preview">日历</span>
   * 您可以在列表视图中显示连接的Workfront项目。


<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

* 可以为以下连接的记录或对象类型添加“连接的记录”页：

   * Workfront Planning记录类型
   * Workfront项目

     即使您无权在Workfront中访问连接的Workfront项目，也可以查看这些项目。

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
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> 除了Adobe Workfront之外，如果要为来自以下应用程序的对象添加连接的记录页面，还必须具有下列功能：</p>
   <ul><li><p>Adobe Experience Manager Assets许可证以及AEM Assets与Workfront之间的集成，用于连接AEM资源与Planning记录类型。</p>
   <p>有关信息，请参阅适用于Experience Manager Assets和Assets Essentials的<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront：文章索引</a>。 </p></li>
   <li><p> 用于连接记录类型与GenStudio Brands的Adobe GenStudio for Performance Marketing许可证</p>
   <p>有关信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketing入门</a>。</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <p>向工作区和记录类型提供或更高权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> 
  </td>
  </tr>   
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 将“连接的记录”页面添加到记录

在将连接的记录页面添加到记录之前，必须先将记录类型与其他记录类型或Workfront项目连接起来。

1. 单击记录名称，从记录类型页面的任意视图中将其打开。
1. 从以下区域之一单击&#x200B;**添加页面**：

   * 记录的预览窗口
   * 记录的详细信息页面，在单击预览页面右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)之后。

   将打开&#x200B;**创建页面**&#x200B;框。

   ![添加连接的记录页面模式](assets/add-connection-view-page-modal.png)

1. 添加&#x200B;**页面名称**，为&#x200B;**页面类型**&#x200B;单击&#x200B;**连接的记录页面**，然后单击&#x200B;**创建**。
1. （可选）单击列表中已连接的记录或对象类型的名称，或搜索该记录或对象类型，然后在列表中显示该记录或对象类型时单击该名称，以创建该记录或对象类型的页面。

   >[!TIP]
   >
   ><span class="preview">您可以为每个记录类型创建一个连接的记录页。 如果连接的记录类型已具有页面，则该页面不再显示为选项。</span>


1. （可选且有条件）如果要为显示构建页面的记录或对象类型有多个已连接字段，请从&#x200B;**选择引用字段**&#x200B;列表中单击要在已连接记录页面中显示其记录或对象的字段。

   ![选择引用字段列表](assets/select-reference-field-list-on-connected-records-page.png)

   以下页面之一将添加到“连接的记录”页面：

   * 记录类型的表格视图
   * 项目对象类型的列表视图

   连接到当前记录的记录或项目将显示在表或列表视图中。

   >[!TIP]
   >
   >您必须在记录的表或详细信息区域中添加已连接的记录，然后才能在已连接的记录页面中显示它们。 否则，表或列表为空。

   默认情况下，将显示连接的记录的前五个字段。<!--No lookup fields display by default.-->

   在营销活动详细信息下![受众连接的表视图](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （视情况而定）根据在连接的记录页面中显示的记录类型，执行以下操作之一：

   * 管理规划记录
有关信息，请参阅本文中的[管理Planning记录的连接的记录页面](#manage-the-connected-records-page-for-planning-records)部分。
   * 管理Workfront项目
有关信息，请参阅本文中的[管理Workfront项目的连接记录页面](#manage-the-connected-records-page-for-workfront-projects)部分。

1. （可选）双击&#x200B;**连接的记录页**&#x200B;选项卡的名称

   或

   将鼠标悬停在该选项卡的名称上，然后单击&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**重命名**&#x200B;以重命名为新的连接记录页面选项卡。


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. （可选）将鼠标悬停在“连接的记录”页选项卡的名称上，单击“**更多**”![“更多”菜单](assets/more-menu.png)，然后单击“**删除”**&#x200B;以移至“选项卡”。

### 管理Planning记录的“连接的记录”页面

根据您使用的环境，管理Planning记录的已连接记录页面会有所不同。

#### 管理生产环境中Planning记录的“连接的记录”页面

在生产环境中为连接的Planning记录创建连接的记录页面时，请执行以下操作： <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. 转到记录类型页面并单击记录名称。 这将打开记录的预览页面。
1. 单击显示Planning记录的已连接记录页的标签。
连接到所选记录的记录将显示在表格视图中。
1. 单击表视图底部的&#x200B;**连接**&#x200B;以连接现有记录，从连接框中选择它们，然后单击框外部将其关闭。 记录会自动添加到表中，并连接到您选择的记录。 在添加记录之前，这些记录必须存在。

   有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. 在表视图中内联编辑来自连接记录的任何信息。
1. 将鼠标悬停在已连接记录的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)

   或

   选择其中一个记录，然后单击列表底部蓝色栏中的以下选项之一：

   * **查看**&#x200B;以在新选项卡中打开记录页面
   * **复制链接**&#x200B;以复制指向记录页面的链接
   * **编辑缩略图**&#x200B;以打开&#x200B;**记录缩略图**&#x200B;框并编辑记录的缩略图图像
   * **复制**&#x200B;以复制连接的记录。 重复记录也连接到当前记录。
   * **在上方或下方插入记录**&#x200B;以将新记录添加到连接的记录类型。 此处添加的新记录也将连接到当前记录。 在表中选择记录时，此选项在蓝色栏中不可用。
   * **删除**&#x200B;以删除记录。 删除已连接的记录会将其从记录类型以及连接记录的所有位置删除。 删除的记录移至其记录类型的&#x200B;**最近删除的**&#x200B;个框。

     有关编辑表视图中的记录的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以选择多个记录或对象来删除它们。

1. 在“连接的记录”页面上的表中内联编辑任何记录。
1. 在连接的记录页面的工具栏中使用以下任何视图元素来管理表格视图：

   * **过滤器**
   * **排序**
   * **分组**
   * **字段**，用于显示、隐藏或重新排列字段
   * **行高**
   * **搜索**

   有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >不能在已连接记录选项卡的表视图中创建、编辑或删除字段。

<div class="preview">

#### 在“预览”环境中管理Planning记录的“连接的记录”页面

在“预览”环境中为连接的Planning记录创建连接的记录页面时，请执行以下操作：<!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. 转到记录类型页面并单击记录名称。 这将打开记录的预览页面。
1. 单击显示Planning记录的已连接记录页的标签。
连接到所选记录的记录将显示在表格视图中。
1. 单击已连接记录页面右上角的&#x200B;**连接记录**&#x200B;以连接现有记录，从连接框中选择这些记录，然后单击框外部将其关闭。 记录会自动添加到表中，并连接到您选择的记录。 在添加记录之前，这些记录必须存在。

   有关详细信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. 单击表底部的&#x200B;**新行**&#x200B;以添加新记录。 新记录将自动连接到您选择的记录。
1. 在表视图中内联编辑来自连接记录的任何信息。
1. 将鼠标悬停在已连接记录的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)

   或

   选择其中一个记录，然后单击列表底部蓝色栏中的以下选项之一：

   * **查看**&#x200B;以在新选项卡中打开记录页面
   * **复制链接**&#x200B;以复制指向记录页面的链接
   * **编辑缩略图**&#x200B;以打开&#x200B;**记录缩略图**&#x200B;框并编辑记录的缩略图图像
   * **复制**&#x200B;以复制连接的记录。 重复记录也连接到当前记录。
   * **在上方或下方插入记录**&#x200B;以将新记录添加到连接的记录类型。 此处添加的新记录也将连接到当前记录。 在表中选择记录时，此选项在蓝色栏中不可用。
   * **删除**&#x200B;以删除记录。 删除已连接的记录会将其从记录类型以及连接记录的所有位置删除。 删除的记录移至其记录类型的&#x200B;**最近删除的**&#x200B;个框。

     有关编辑表视图中的记录的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以选择多个记录或对象来删除它们。

1. 在“连接的记录”页面上的表中内联编辑任何记录。
1. 在连接的记录页面的工具栏中使用以下任何视图元素来管理表格视图：

   * **过滤器**
   * **排序**
   * **分组**
   * **字段**，用于显示、隐藏或重新排列字段
   * **行高**
   * **搜索**

   有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >不能在已连接记录选项卡的表视图中创建、编辑或删除字段。
1. 单击“视图”下拉菜单，然后单击&#x200B;**新建视图**&#x200B;以添加该页面的新视图，然后执行以下操作：
   1. 添加&#x200B;**视图名称**。
   1. 从&#x200B;**视图类型**&#x200B;区域，选择以下视图类型之一：

      * 表
有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)
      * 时间线
有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
      * 日历
有关信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

        有关详细信息，请参阅本文中[从连接的记录页面](#manage-multiple-views-from-the-connected-records-page)管理多个视图。

   1. 单击&#x200B;**创建**。
视图下拉菜单中添加了新视图。
   1. （可选）将鼠标悬停在您创建的视图的名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下选项之一：
      * **重命名**，为视图添加新名称。
      * **共享**


        有关详细信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。

        >[!NOTE]
        >
        >您无法共享Workfront创建的系统视图。

      * **删除**
有关信息，请参阅[删除记录视图](/help/quicksilver/planning/views/delete-record-views.md)。

        ![](assets/view-more-menu-projects-connected-records-page.png)

</div>


<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->

### 管理Workfront项目的“连接的记录”页面

在为连接的Workfront项目创建“连接的记录”页面时，请执行以下操作：

1. 转到记录类型页面并单击记录名称。 这将打开记录的预览页面。
1. 单击显示Workfront项目的已连接记录页面的选项卡。
与所选记录连接的项目将显示在列表视图中。
1. 单击已连接记录页面右上角的&#x200B;**连接记录**&#x200B;以连接现有项目。

   有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
1. 在表中内联编辑项目信息。
1. 单击&#x200B;**新建行**&#x200B;以创建没有模板的项目。 新项目将自动连接到当前记录。

   有关详细信息，请参阅将Workfront对象连接到记录时[从Workfront Planning创建对象](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
1. 将鼠标悬停在列表中的项目名称上，然后单击&#x200B;**更多**&#x200B;菜单[更多](assets/more-menu.png)

   或

   选择一个或多个项目，并注意列表底部的蓝色栏，然后单击以下项之一：

   * **删除**&#x200B;以删除项目。 删除项目会断开它与记录的连接，并将其移到Workfront的回收站。 Workfront管理员最多可以在删除项目后30天内恢复这些已删除的项目。
   * **断开连接**&#x200B;以断开项目与记录的连接。 断开项目连接会将其及其查找字段的所有值从当前记录中删除。

     >[!TIP]
     >
     >您可以选择多个项目来断开它们的连接或删除它们。
1. 单击“视图”下拉菜单，然后单击&#x200B;**新建视图**&#x200B;以添加该页面的新视图，然后执行以下操作：
   1. 添加&#x200B;**视图名称**。
   1. 从&#x200B;**视图类型**&#x200B;区域中选择&#x200B;**列表**。
   1. 单击&#x200B;**创建**。
新的列表视图将添加到视图下拉菜单中。

      有关详细信息，请参阅本文中[从连接的记录页面](#manage-multiple-views-from-the-connected-records-page)管理多个视图。

   1. （可选）将鼠标悬停在您创建的视图的名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下选项之一：
      * **重命名**，为视图添加新名称。
      * <span class="preview">**共享**</span>

        有关详细信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。

        >[!NOTE]
        >
        >您无法共享Workfront创建的系统视图。

      * **删除**
有关信息，请参阅[删除记录视图](/help/quicksilver/planning/views/delete-record-views.md)。

        ![](assets/view-more-menu-projects-connected-records-page.png)

   1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-icon.png)，然后使用该筛选器显示特定项目。

      >[!TIP]
      >
      ><span class="preview">对于人员类型字段，如&#x200B;**所有者**&#x200B;或&#x200B;**发起人**，您可以使用通配符显示登录用户分配给这些角色的项目。</span>
      >
      >![使用用户通配符筛选已连接项目的记录页](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. 单击&#x200B;**列**&#x200B;图标![列图标](assets/columns-icon.png)可隐藏或显示列表中的列。
   1. 单击表格视图右上角的&#x200B;**+**&#x200B;图标以将现有字段添加到表格中。 字段必须先存在，然后才能添加它们。

      将打开&#x200B;**列管理器**&#x200B;框。 执行以下操作：

      1. 在&#x200B;**可用**&#x200B;列中搜索现有对象字段，然后单击该字段名称右侧的&#x200B;**+**&#x200B;以将其添加到&#x200B;**已选定**&#x200B;列。

         您选择的字段将添加到已连接记录页的表视图中。
      1. 单击&#x200B;**Selected**&#x200B;列中某个字段右侧的&#x200B;**-**&#x200B;以将其从表视图中删除。
      1. 单击&#x200B;**保存**&#x200B;以保存连接的记录页表视图。


<div class="preview">

## 从“连接的记录”页面管理多个视图

您可以从记录的已连接记录页面添加和管理多个视图类型。

在记录类型的“连接的记录”页面中创建的视图在Workfront Planning中任何显示记录类型页面的位置都可用。 在Workfront Planning中的任何其他位置为同一记录类型创建的视图也可在该记录类型的所有连接记录页中访问。

要从连接的记录页面管理多个视图，请执行以下操作：

1. 在记录的已连接记录页面中，单击视图名称右侧的下拉菜单，然后单击&#x200B;**新建视图**&#x200B;以添加视图，然后从以下选项中选择：

   * **表**。 有关详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。
   * **时间线**。 有关详细信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
   * **日历**。 有关详细信息，请参阅[管理日历视图](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

1. （可选）将鼠标悬停在“连接的记录”页面中的视图名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下任一选项： *************&#x200B;检查以确保所有这些都可行&#x200B;*********

   * **重命名**
   * **共享**。 有关详细信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。

   >[!TIP]
   >
   >共享“连接的记录”页面中的视图可让Workfront Planning中显示视图的所有区域的用户访问这些视图。
   >此外，如果从Workfront Planning的任何其他区域共享视图，则该视图也在“连接的记录”页面中可供相同用户使用。

   * **导出**
   * **重复**。 有关详细信息，请参阅[重复记录视图](/help/quicksilver/planning/views/duplicate-record-views.md)。

     >[!TIP]
     >
     >从“连接的记录”页面中复制视图时，该视图可在Workforce计划的所有其他区域中使用，同时查看相同的记录类型。

</div>