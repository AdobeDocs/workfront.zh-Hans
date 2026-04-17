---
title: 在Adobe Workfront Planning中管理列表视图
description: 在Adobe Workfront Planning的记录的“连接的记录”页面中访问对象时，您可以在列表视图中显示对象及其字段。 本文介绍了如何在记录的“连接的记录”页面中创建或编辑列表视图。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: a6c2bc4127a52fad209004995ea2262fa64c240d
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 1%

---


# 在Adobe Workfront Planning中管理列表视图

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

您可以在Workfront Planning的以下区域查看列表视图中的对象：

* 记录的详细信息区域中项目的已连接记录页面

  ![列表视图中已连接记录页上的项目](assets/projects-on-connected-records-page-list-view.png)

* 记录类型级别的请求表单列表

  ![在列表视图中请求表单](assets/request-forms-in-list-view.png)

本文介绍了如何在Workfront Planning中导航、创建或编辑列表视图。

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

* 对于连接的记录页面列表视图，请考虑以下事项：

   * 您只能在记录的已连接记录页面的列表视图中查看项目。 列表视图不适用于已连接记录页面中的任何其他对象或记录类型。

  有关创建连接的记录页面的信息，请参阅[将连接的记录页面添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。
   * 在记录的已连接记录页面中查看列表视图之前，您必须将Workfront项目与Planning记录类型连接。 有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
   * 您可以为记录的“连接的记录”页面中的项目创建多个列表视图。

* 对于请求表单列表视图，请考虑以下事项：

   * 不能为Planning请求表单创建或编辑其他列表视图。 Workfront为请求表单创建一个列表视图。<!--this will change-->

     有关申请表单的信息，请参阅[在Adobe Workfront计划中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。
* 根据显示的位置，并非每个列表视图都具有本文中描述的所有元素。

## 管理列表视图 {#manage-a-list-view}

Workfront Planning列表视图类似于Workfront的增强列表。 在Workfront Planning中，增强型视图中的大多数元素也存在于列表视图中。

有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. 转到以下区域之一的列表视图：

   * 记录的详细信息区域中项目的已连接记录页面
   * 记录类型的请求表单页面

1. （视情况而定）如果可用，请执行以下操作之一来修改列表视图：

   1. 展开列表左上角的下拉视图菜单以选择其他视图，或单击&#x200B;**新建视图**&#x200B;并创建另一个视图。

      >[!TIP]
      >
      >视图在整个系统中共享。 如果您为一个记录类型创建项目视图，则可以在显示所连接项目的其他记录类型上查看该视图。

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
      >* 在修改视图以恢复其原始首选项后，您可以重置与您共享的仅具有查看权限的视图，也可以复制该视图并共享副本。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

   1. 单击&#x200B;**筛选器**&#x200B;图标![筛选器图标](assets/filter-icon.png)将筛选器添加到视图。 结果会立即在列表中过滤。 您无法保存并命名筛选器。 在将来的访问页面时，将会记住过滤器，并且这些过滤器是共享视图的一部分。

      >[!TIP]
      >
      >要应用个性化过滤器，请为字段值选择以下选项之一：
      >
      >* **我（已登录的用户）**&#x200B;在引用用户的字段中引用已登录的用户。
      >
      >* **我的团队**&#x200B;或&#x200B;**我的主团队**&#x200B;在引用团队的字段中引用您的团队。
      >
      >* **我的群组**&#x200B;或&#x200B;**我的主群组**&#x200B;在引用群组的字段中引用您的群组。
      >
      >* **我的公司**&#x200B;在引用公司的字段中引用您的公司。
      > 
      >* **我的角色**&#x200B;或&#x200B;**我的主要角色**&#x200B;在引用角色的字段中引用您的工作角色。

   1. 单击&#x200B;**列**&#x200B;图标![列图标](assets/columns-icon.png)以选择要显示或隐藏的列。
   1. 将鼠标悬停在列名上，单击该列名左侧的向下箭头，然后单击下列选项之一：
      * **重命名**，为列添加&#x200B;**自定义标签**。 Workfront中原始字段的名称不会更改。
      * **排序**，按所选字段对列表进行排序。 在列标题中添加了表示排序方向的排序图标。
   1. 单击列表右上角的&#x200B;**+**&#x200B;图标在列表中添加或删除列，然后单击&#x200B;**保存**。

      **列管理器**&#x200B;打开。

      您只能将现有字段添加到列表视图。
不能删除第一列中显示的列表视图中的主字段。

   1. 单击&#x200B;**格式化单元格**&#x200B;图标![格式化单元格图标](assets/format-cells-icon.png)。 将打开&#x200B;**格式**&#x200B;框。 <!--change the name of the box when they update it-->
执行以下操作：

      1. 单击&#x200B;**添加条件**。
      1. 在&#x200B;**If**&#x200B;行中，选择一个字段并选择字段值并添加修饰符。 修改量会根据您选择的字段类型而发生更改。

         >[!TIP]
         >
         >只有列表视图中可见的字段可用于条件格式。

      1. （可选）单击&#x200B;**与另一个字段比较**&#x200B;图标![与另一个字段比较](assets/compare-to-another-field-icon.png)，而不是添加字段值，然后选择要将其值与选定字段的值进行比较的字段。 例如，您可以比较项目所有者和项目发起人字段。

         >[!TIP]
         >
         >只有列表视图中可见的字段可用于条件格式。 您比较的字段必须属于相同类型。

      1. （可选）单击&#x200B;**If**&#x200B;行中的&#x200B;**添加条件**&#x200B;以将更多条件添加到同一规则。

         >[!TIP]
         >
         >在一个条件规则中最多可添加10个条件，一个字段最多可有20个规则。

      1. 单击条件之间的&#x200B;**Or**&#x200B;连接器以更改为&#x200B;**And**，并指示必须同时满足多个条件。 **或**&#x200B;是默认连接器。
      1. 在&#x200B;**格式**&#x200B;行中，选择一个字段以指示将设置哪一列的格式。<!--edit this area, if it changes names??-->
      1. （可选）单击所选字段旁边的&#x200B;**颜色圆圈**&#x200B;图标![颜色圆圈图标](assets/color-circle.png)，展开该字段并在&#x200B;**单元格填充**&#x200B;区域中选择其他颜色以更改单元格中背景的颜色，或者从&#x200B;**文本颜色**&#x200B;区域中选择颜色以更改单元格中文本的颜色。
      1. 单击&#x200B;**文本格式**&#x200B;图标![文本格式图标](assets/text-format-icon.png)并从以下选项中选择以设置单元格中文本的格式：
         * 粗体
         * 斜体

      1. 打开&#x200B;**应用到行**&#x200B;设置以将格式应用到满足条件的字段的整行。
      1. （可选）在&#x200B;**格式**&#x200B;框中单击&#x200B;**添加条件**&#x200B;为其他字段添加其他规则并重复上述步骤。
      1. （可选）单击&#x200B;**全部清除**&#x200B;以删除所有格式。
      1. 单击&#x200B;**格式**&#x200B;框外部以将其关闭。

         这会将您返回到列表视图。
格式设置将立即应用于列表视图。
**设置单元格格式**&#x200B;图标旁有一个蓝点，表示该视图应用了特殊格式。

   1. （可选）单击&#x200B;**分组**&#x200B;图标![分组图标](assets/grouping-icon.png) <!--have they updated this to "Grouping"??-->以按公用字段对列表中的项进行分组。 选择一个选项，或使用搜索栏查找字段。

      该字段必须是列表中的列，然后才能按其分组。 并非所有字段类型都可用于分组。

   1. 单击&#x200B;**行高**&#x200B;图标![行高图标](assets/row-height-icon.png)可更新行的垂直长度。 从以下选项中进行选择：

      * 短
      * 标准。 这是默认选项。
      * 媒介
      * 高

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. （可选）在列表右上角的搜索框中添加关键字以搜索项目。

   与搜索词匹配的项目会在列表中突出显示。

1. （可选且有条件）在连接的项目<!--change projects to items here when more items will display in the Glist-->页面中，要向列表添加更多项并自动将其连接到所选记录，请执行下列操作之一：

   * 单击列表右上角的&#x200B;**连接记录**&#x200B;以添加现有项。
   * 单击列表底部的&#x200B;**新行**&#x200B;以添加新项。
1. 单击列表中已连接项目的名称，以在其他浏览器选项卡中将其打开。
1. 双击列表中的单元格以编辑字段信息，然后按Enter保存更改。

   某些字段为只读。 例如，项目的完成百分比是由系统计算的字段，您无法手动进行编辑。

1. 将鼠标悬停在列表中项目的名称上，然后单击&#x200B;**更多**&#x200B;菜单[更多菜单](assets/more-menu.png)，然后单击&#x200B;**查看**&#x200B;以在其他选项卡中打开项目

   或

   选择一个或多个项目，并注意列表底部的操作栏，然后单击下列选项之一（如果可用）。 根据您从哪个区域访问列表视图，单击以下选项之一：

   * **删除**&#x200B;以删除该项。 删除项目会断开它与记录的连接，并将其移到Workfront的回收站。 Workfront管理员最多可以在删除项目后30天内恢复这些已删除的项目。 删除表单不会删除提交表单时创建的请求或记录。
   * **断开连接**&#x200B;以断开项目与记录的连接。 断开项目连接会将其及其查找字段的所有值从当前记录中删除。

     <!--update screen shot at preview release-->

     “连接的记录”页面列表视图中的![操作栏](assets/actions-bar-connected-records-page-list-view.png)

   * **编辑表单**：打开Planning请求表单并允许您编辑它。
   * **取消发布**：取消发布请求表单。 这会从请求区域删除表单，并且用户无法再将请求添加到此记录类型。
   * **共享**：打开请求表单的“共享”框，您可以在其中与他人共享。
   * **复制链接**：复制指向Planning请求表单的链接，以便与其他用户共享。 如果表单已公开共享，则您可以与Workfront Planning以外的人员共享该链接。

     Planning请求列表中的![操作栏](assets/actions-bar-in-inake-forms-list.png)



