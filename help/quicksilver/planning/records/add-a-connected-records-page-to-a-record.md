---
title: 向记录添加“连接的记录”页
description: 通过将“连接的记录”页面的选项卡添加到记录，可以查看来自连接的记录或对象的信息。 这会将表视图中的连接记录添加到选项卡。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---


# 将“连接的记录”页面添加到记录

通过将“连接的记录”页面的选项卡添加到记录，可以查看来自连接的记录或对象的信息。 这会将表视图中的连接记录添加到选项卡。

将“连接的记录”页面添加到记录时，请考虑以下事项：

* 在将记录或对象类型从记录类型的表格视图连接到记录类型后，可以将“连接的记录”页添加到记录中。

* 您可以从记录的预览区域或记录的页面添加“连接的记录”页面。

* “连接的记录”页在表格视图中仅显示一个对象或记录类型中的连接对象或记录。 页面不显示该类型的所有记录。

* 可以为以下连接的记录或对象类型添加“连接的记录”页：

   * Workfront Planning记录类型
   * Workfront项目、项目、项目组合、组或公司。 您可以查看连接的Workfront对象，即使您无权在Workfront中访问它们。

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

1. 单击记录名称，从记录类型页面的任意视图中将其打开。
1. 从以下区域之一单击&#x200B;**添加页面**：

   * 记录的预览窗口
   * 记录的详细信息页面，在单击预览页面右上角的&#x200B;**在新标签中打开**&#x200B;图标![在新标签中打开详细信息](assets/open-details-in-a-new-tab-icon.png)之后。

   将打开&#x200B;**创建页面**&#x200B;框。

   ![添加连接的记录页面模式](assets/add-connection-view-page-modal.png)

1. 添加&#x200B;**页面名称**，单击&#x200B;**连接的记录页面**，然后单击&#x200B;**创建**。

   新的已连接记录页面将作为新选项卡添加到记录页面。

   连接到当前记录的记录将显示在表格视图中。

   >[!TIP]
   >
   >您必须在记录的表或详细信息区域中添加已连接的记录，然后才能在已连接的记录页面中显示它们。

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   默认情况下，将显示连接的记录的前五个字段。<!--No lookup fields display by default.-->

   在营销活动详细信息下![受众连接的表视图](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （可选）搜索或单击列表中连接的记录或对象类型的名称。

1. （可选且有条件）在“连接的记录”页面的表视图中，在查看连接的Planning记录或除项目之外的任何Workfront对象时，执行以下任一操作： <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * 单击记录名称。 这将在新选项卡中打开记录页面。

   * 单击表视图底部的&#x200B;**连接**&#x200B;以连接更多记录，然后单击连接框外部将其关闭。 新记录将自动添加到表中。

     有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
   * 在表视图中内联编辑来自连接记录的任何信息。

   * 将鼠标悬停在已连接记录的名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)

     或

     选择其中一个记录，然后单击列表底部蓝色栏中的以下选项之一：

      * **查看**&#x200B;以在新选项卡中打开记录页面
      * **复制链接**&#x200B;以复制指向记录页面的链接
      * **编辑缩略图**&#x200B;以打开&#x200B;**记录缩略图**&#x200B;框并编辑记录的缩略图图像
      * **复制**&#x200B;以复制连接的记录。 重复记录也连接到当前记录。
      * **在上方或下方插入记录**&#x200B;以将新记录添加到连接的记录类型。 此处添加的新记录也将连接到当前记录。 在表中选择记录时，此选项在蓝色栏中不可用。
      * **删除**&#x200B;以删除记录。 删除已连接的记录会将其从记录类型以及连接记录的所有位置删除。

     有关编辑表视图中的记录的信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以选择多个记录或对象来删除它们。

   * 在“连接的记录”页面上的表中内联编辑任何Planning记录。

     所有其他Workfront对象都以只读表格视图显示，您无法对其进行编辑。

1. （可选且视情况而定）在“连接的记录”页面的表视图中，在查看连接的Workfront项目时执行以下任一操作：

   * 单击已连接记录页面右上角的&#x200B;**连接记录**&#x200B;以连接现有项目。

   有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。
   * 在表中内联编辑项目信息。
   * 单击&#x200B;**新建行**&#x200B;以创建没有模板的项目。 新项目立即连接到当前记录。

     有关详细信息，请参阅将Workfront对象连接到记录时[从Workfront Planning创建对象](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * 将鼠标悬停在项目上并单击&#x200B;**更多**&#x200B;菜单[更多](assets/more-menu.png)

     或

     选择一个或多个项目，并注意列表底部的蓝色栏，然后单击以下项之一：

      * **删除**&#x200B;以删除项目。 删除项目会断开它与记录的连接，并将其移到Workfront的回收站。
      * **断开连接**&#x200B;以断开项目与记录的连接。 断开项目连接会将其及其查找字段的所有值从当前记录中删除。

1. （可选）双击&#x200B;**连接的记录页**&#x200B;选项卡的名称

   或

   将鼠标悬停在该选项卡的名称上，然后单击&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**重命名**&#x200B;以重命名为新的“连接的视图”选项卡。
1. （可选）在连接的记录页面的工具栏中使用以下任何视图元素来管理表格视图：

   * 过滤器
   * 排序
   * 分组
   * 字段，用于显示、隐藏或重新排列字段
   * 行高
   * 搜索

   有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >不能在已连接记录选项卡的表视图中创建、编辑或删除字段。

1. （可选）将鼠标悬停在“连接的记录”页选项卡的名称上，单击&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以移至“选项卡”。